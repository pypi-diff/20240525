# Comparing `tmp/keras_nightly-3.3.3.dev2024052303.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024052403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.3.dev2024052303.tar", last modified: Thu May 23 03:20:56 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.3.dev2024052403.tar", last modified: Fri May 24 03:21:59 2024, max compression
```

## Comparing `keras_nightly-3.3.3.dev2024052303.tar` & `keras_nightly-3.3.3.dev2024052403.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.814804 keras_nightly-3.3.3.dev2024052303/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-23 03:20:56.814804 keras_nightly-3.3.3.dev2024052303/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.710804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.714804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.718804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-23 03:20:51.000000 keras_nightly-3.3.3.dev2024052303/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.722804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.726804 keras_nightly-3.3.3.dev2024052303/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.730804 keras_nightly-3.3.3.dev2024052303/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.734804 keras_nightly-3.3.3.dev2024052303/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.738804 keras_nightly-3.3.3.dev2024052303/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25341 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23651 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.738804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.742804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.742804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.746804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.750804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.750804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    48117 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.754804 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.758804 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.758804 keras_nightly-3.3.3.dev2024052303/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.758804 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.758804 keras_nightly-3.3.3.dev2024052303/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.758804 keras_nightly-3.3.3.dev2024052303/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.762804 keras_nightly-3.3.3.dev2024052303/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33373 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.762804 keras_nightly-3.3.3.dev2024052303/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.762804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.762804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.766804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.766804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.770804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42056 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    64242 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.770804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.774804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.774804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.778804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    42135 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27923 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.782804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.782804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.786804 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.786804 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.790804 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.790804 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.790804 keras_nightly-3.3.3.dev2024052303/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    70024 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.794804 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.794804 keras_nightly-3.3.3.dev2024052303/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.798804 keras_nightly-3.3.3.dev2024052303/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27019 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    37642 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    21256 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   196517 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.798804 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.802804 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.802804 keras_nightly-3.3.3.dev2024052303/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.802804 keras_nightly-3.3.3.dev2024052303/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.802804 keras_nightly-3.3.3.dev2024052303/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.802804 keras_nightly-3.3.3.dev2024052303/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/saving/keras_saveable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.802804 keras_nightly-3.3.3.dev2024052303/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.806804 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.806804 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.806804 keras_nightly-3.3.3.dev2024052303/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.814804 keras_nightly-3.3.3.dev2024052303/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-23 03:19:22.000000 keras_nightly-3.3.3.dev2024052303/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-23 03:20:54.000000 keras_nightly-3.3.3.dev2024052303/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:20:56.814804 keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-23 03:20:56.000000 keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-23 03:20:56.000000 keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:20:56.000000 keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 03:20:56.000000 keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 03:20:56.000000 keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:20:56.814804 keras_nightly-3.3.3.dev2024052303/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-23 03:20:54.000000 keras_nightly-3.3.3.dev2024052303/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.606277 keras_nightly-3.3.3.dev2024052403/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-24 03:21:59.606277 keras_nightly-3.3.3.dev2024052403/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.502278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.506278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.510278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-24 03:21:54.000000 keras_nightly-3.3.3.dev2024052403/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.514278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.518278 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.522277 keras_nightly-3.3.3.dev2024052403/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.526277 keras_nightly-3.3.3.dev2024052403/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.530278 keras_nightly-3.3.3.dev2024052403/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25341 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23651 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.530278 keras_nightly-3.3.3.dev2024052403/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.534278 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.534278 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.538277 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.542277 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.542277 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48087 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.546277 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.550277 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.550277 keras_nightly-3.3.3.dev2024052403/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.550277 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.550277 keras_nightly-3.3.3.dev2024052403/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.550277 keras_nightly-3.3.3.dev2024052403/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.550277 keras_nightly-3.3.3.dev2024052403/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33373 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.554277 keras_nightly-3.3.3.dev2024052403/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.554277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.554277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.554277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.558277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.562277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42056 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64242 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.562277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.562277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.566277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.570277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41996 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.574277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.574277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.578277 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.578277 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.578277 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.582277 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.582277 keras_nightly-3.3.3.dev2024052403/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70024 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.582277 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61530 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.586277 keras_nightly-3.3.3.dev2024052403/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.586277 keras_nightly-3.3.3.dev2024052403/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27019 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37642 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21256 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196517 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.590277 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.590277 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.590277 keras_nightly-3.3.3.dev2024052403/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.594277 keras_nightly-3.3.3.dev2024052403/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.594277 keras_nightly-3.3.3.dev2024052403/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.594277 keras_nightly-3.3.3.dev2024052403/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.594277 keras_nightly-3.3.3.dev2024052403/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.594277 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.598277 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.598277 keras_nightly-3.3.3.dev2024052403/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.602277 keras_nightly-3.3.3.dev2024052403/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-24 03:20:41.000000 keras_nightly-3.3.3.dev2024052403/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-24 03:21:57.000000 keras_nightly-3.3.3.dev2024052403/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:21:59.606277 keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-24 03:21:59.000000 keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-24 03:21:59.000000 keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:21:59.000000 keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 03:21:59.000000 keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 03:21:59.000000 keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 03:21:59.606277 keras_nightly-3.3.3.dev2024052403/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-24 03:21:57.000000 keras_nightly-3.3.3.dev2024052403/setup.py
```

### Comparing `keras_nightly-3.3.3.dev2024052303/PKG-INFO` & `keras_nightly-3.3.3.dev2024052403/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024052303
+Version: 3.3.3.dev2024052403
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024052303/README.md` & `keras_nightly-3.3.3.dev2024052403/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/activations/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/applications/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/backend/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/config/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/layers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/losses/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/ops/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/random/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/saving/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/tree/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/api/utils/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/activations/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/activations/activations.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/api_export.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/convnext.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/densenet.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/nasnet.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/resnet.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/vgg16.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/vgg19.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/applications/xception.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/common/variables.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/config.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/exports.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/core.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/image.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/math.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/random.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/core.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/image.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/math.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
 def ndim(x):
     x = convert_to_tensor(x)
     return x.ndim
 
 
 def nonzero(x):
     x = convert_to_tensor(x)
-    return tuple(cast(indices, "int32") for indices in torch.nonzero(x).T)
+    return cast(torch.nonzero(x).T, "int32")
 
 
 def not_equal(x1, x2):
     x1, x2 = convert_to_tensor(x1), convert_to_tensor(x2)
     return torch.not_equal(x1, x2)
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/random.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/callback.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/history.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/constraints/constraints.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/cifar.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/imdb.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/mnist.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/datasets/reuters.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/export/export_lib.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/initializers/initializer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/dense.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/identity.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/masking.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/input_spec.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/add.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/average.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.utils import argument_validation
 from keras.src.utils import backend_utils
 from keras.src.utils import numerical_utils
+from keras.src.utils import tf_utils
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 @keras_export("keras.layers.HashedCrossing")
 class HashedCrossing(Layer):
     """A preprocessing layer which crosses features using the "hashing trick".
 
@@ -134,15 +135,15 @@
 
         return tuple(input_shape[0])[:-1] + (self.num_bins,)
 
     def call(self, inputs):
         from keras.src.backend import tensorflow as tf_backend
 
         self._check_at_least_two_inputs(inputs)
-        inputs = [tf_backend.convert_to_tensor(x) for x in inputs]
+        inputs = [tf_utils.ensure_tensor(x) for x in inputs]
         self._check_input_shape_and_type(inputs)
 
         # Uprank to rank 2 for the cross_hashed op.
         rank = len(inputs[0].shape)
         if rank < 2:
             inputs = [tf_backend.numpy.expand_dims(x, -1) for x in inputs]
         if rank < 1:
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/hashing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.utils import backend_utils
 from keras.src.utils import numerical_utils
+from keras.src.utils import tf_utils
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 @keras_export("keras.layers.Hashing")
 class Hashing(Layer):
     """A preprocessing layer which hashes and bins categorical features.
 
@@ -207,15 +208,15 @@
         self._convert_input_args = False
         self._allow_non_tensor_positional_args = True
         self.supports_jit = False
 
     def call(self, inputs):
         from keras.src.backend import tensorflow as tf_backend
 
-        inputs = tf_backend.convert_to_tensor(inputs)
+        inputs = tf_utils.ensure_tensor(inputs)
         if self.output_mode == "one_hot" and inputs.shape[-1] == 1:
             # One hot only unpranks if the final dimension is not 1.
             inputs = tf_backend.numpy.squeeze(inputs, axis=-1)
         if isinstance(inputs, tf.SparseTensor):
             indices = tf.SparseTensor(
                 indices=inputs.indices,
                 values=self._hash_values_to_bins(inputs.values),
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/index_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 
 from keras.src import backend
 from keras.src.layers.layer import Layer
 from keras.src.utils import argument_validation
 from keras.src.utils import numerical_utils
+from keras.src.utils import tf_utils
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 class IndexLookup(Layer):
     """Maps values from a vocabulary to integer indices.
 
     This layer translates a set of arbitrary hashables into an integer output
@@ -561,44 +562,38 @@
             output_dtype = "int64"
         else:
             output_dtype = backend.floatx()
         output_shape = self.compute_output_shape(inputs.shape)
         return backend.KerasTensor(output_shape, dtype=output_dtype)
 
     def adapt(self, data, steps=None):
-        from keras.src.backend import tensorflow as tf_backend
-
         self.reset_state()
         if isinstance(data, tf.data.Dataset):
             if steps is not None:
                 data = data.take(steps)
             for batch in data:
                 self.update_state(batch)
         else:
-            data = tf_backend.convert_to_tensor(
-                data, dtype=self.vocabulary_dtype
-            )
+            data = tf_utils.ensure_tensor(data, dtype=self.vocabulary_dtype)
             if data.shape.rank == 1:
                 # A plain list of strings
                 # is treated as as many documents
                 data = tf.expand_dims(data, -1)
             self.update_state(data)
         self.finalize_state()
 
     def update_state(self, data):
-        from keras.src.backend import tensorflow as tf_backend
-
         if self._has_input_vocabulary:
             raise ValueError(
                 f"Cannot adapt layer '{self.name}' after setting a static "
                 "vocabulary via `vocabulary` argument or "
                 "`set_vocabulary()` method."
             )
 
-        data = tf_backend.convert_to_tensor(data, dtype=self.vocabulary_dtype)
+        data = tf_utils.ensure_tensor(data, dtype=self.vocabulary_dtype)
         if data.shape.rank == 0:
             data = tf.expand_dims(data, 0)
         if data.shape.rank == 1:
             # Expand dims on axis 0 for tf-idf. A 1-d tensor
             # is a single document.
             data = tf.expand_dims(data, 0)
 
@@ -704,15 +699,15 @@
             self.num_documents.assign(0)
 
     def call(self, inputs):
         from keras.src.backend import tensorflow as tf_backend
 
         self._ensure_known_vocab_size()
 
-        inputs = tf_backend.convert_to_tensor(inputs, dtype=self._key_dtype)
+        inputs = tf_utils.ensure_tensor(inputs, dtype=self._key_dtype)
         original_shape = inputs.shape
         # Some ops will not handle scalar input, so uprank to rank 1.
         if inputs.shape.rank == 0:
             inputs = self._expand_dims(inputs, -1)
 
         if isinstance(inputs, tf.SparseTensor):
             lookups = tf.SparseTensor(
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.layers.preprocessing.index_lookup import listify_tensors
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.saving import serialization_lib
 from keras.src.utils import argument_validation
 from keras.src.utils import backend_utils
+from keras.src.utils import tf_utils
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 @keras_export("keras.layers.TextVectorization")
 class TextVectorization(Layer):
     """A preprocessing layer which maps text features to integer sequences.
 
@@ -408,24 +409,22 @@
                 Total number of steps (batches of samples) to process.
                 If `data` is a `tf.data.Dataset`, and `steps` is `None`,
                 `adapt()` will run until the input dataset is exhausted.
                 When passing an infinitely
                 repeating dataset, you must specify the `steps` argument. This
                 argument is not supported with array inputs or list inputs.
         """
-        from keras.src.backend import tensorflow as tf_backend
-
         self.reset_state()
         if isinstance(data, tf.data.Dataset):
             if steps is not None:
                 data = data.take(steps)
             for batch in data:
                 self.update_state(batch)
         else:
-            data = tf_backend.convert_to_tensor(data, dtype="string")
+            data = tf_utils.ensure_tensor(data, dtype="string")
             if data.shape.rank == 1:
                 # A plain list of strings
                 # is treated as as many documents
                 data = tf.expand_dims(data, -1)
             self.update_state(data)
         self.finalize_state()
 
@@ -516,17 +515,15 @@
                 document frequency weights with equal length to vocabulary.
                 Must be set if `output_mode` is `"tf_idf"`.
                 Should not be set otherwise.
         """
         self._lookup_layer.set_vocabulary(vocabulary, idf_weights=idf_weights)
 
     def _preprocess(self, inputs):
-        from keras.src.backend import tensorflow as tf_backend
-
-        inputs = tf_backend.convert_to_tensor(inputs, dtype=tf.string)
+        inputs = tf_utils.ensure_tensor(inputs, dtype=tf.string)
         if self._standardize in ("lower", "lower_and_strip_punctuation"):
             inputs = tf.strings.lower(inputs)
         if self._standardize in (
             "strip_punctuation",
             "lower_and_strip_punctuation",
         ):
             inputs = tf.strings.regex_replace(
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/backend.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/layers.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/losses.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/losses/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/losses/loss.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/losses/losses.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/confusion_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,18 +660,15 @@
                 position, hence this tensor must have the same shape.
             predicate: A binary boolean functor to be applied to arguments
                 `constrained` and `self.value`, e.g. `ops.greater`.
 
         Returns:
             maximal dependent value, if no value satisfies the constraint 0.0.
         """
-        feasible = backend.convert_to_numpy(
-            ops.nonzero(predicate(constrained, self.value))
-        )
-
+        feasible = ops.nonzero(predicate(constrained, self.value))
         feasible_exists = ops.greater(ops.size(feasible), 0)
         max_dependent = ops.max(ops.take(dependent, feasible), initial=0)
 
         return ops.where(feasible_exists, max_dependent, 0.0)
 
 
 @keras_export("keras.metrics.SensitivityAtSpecificity")
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/metric.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/models/cloning.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/models/functional.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/models/model.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     There are three ways to instantiate a `Model`:
 
     ## With the "Functional API"
 
     You start from `Input`,
     you chain layer calls to specify the model's forward pass,
-    and finally you create your model from inputs and outputs:
+    and finally, you create your model from inputs and outputs:
 
     ```python
     inputs = keras.Input(shape=(37,))
     x = keras.layers.Dense(32, activation="relu")(inputs)
     outputs = keras.layers.Dense(5, activation="softmax")(x)
     model = keras.Model(inputs=inputs, outputs=outputs)
     ```
@@ -241,18 +241,19 @@
                 Defaults to `False`.
             show_trainable: Whether to show if a layer is trainable.
                 Defaults to `False`.
             layer_range: a list or tuple of 2 strings,
                 which is the starting layer name and ending layer name
                 (both inclusive) indicating the range of layers to be printed
                 in summary. It also accepts regex patterns instead of exact
-                name. In such case, start predicate will be the first element
-                it matches to `layer_range[0]` and the end predicate will be
-                the last element it matches to `layer_range[1]`.
-                By default `None` which considers all layers of model.
+                names. In this case, the start predicate will be
+                the first element that matches `layer_range[0]`
+                and the end predicate will be the last element
+                that matches `layer_range[1]`.
+                By default `None` considers all layers of the model.
 
         Raises:
             ValueError: if `summary()` is called before the model is built.
         """
         summary_utils.print_summary(
             self,
             line_length=line_length,
@@ -264,16 +265,16 @@
         )
 
     @traceback_utils.filter_traceback
     def save(self, filepath, overwrite=True, **kwargs):
         """Saves a model as a `.keras` file.
 
         Args:
-            filepath: `str` or `pathlib.Path` object. Path where to save
-                the model. Must end in `.keras`.
+            filepath: `str` or `pathlib.Path` object.
+                The path where to save the model. Must end in `.keras`.
             overwrite: Whether we should overwrite any existing model at
                 the target location, or instead ask the user via
                 an interactive prompt.
             save_format: The `save_format` argument is deprecated in Keras 3.
                 Format to use, as a string. Only the `"keras"` format is
                 supported at this time.
 
@@ -470,15 +471,15 @@
 
         Example:
 
         ```python
         # Create the artifact
         model.export("path/to/location")
 
-        # Later, in a different process / environment...
+        # Later, in a different process/environment...
         reloaded_artifact = tf.saved_model.load("path/to/location")
         predictions = reloaded_artifact.serve(input_data)
         ```
 
         If you would like to customize your serving endpoints, you can
         use the lower-level `keras.export.ExportArchive` class. The
         `export()` method relies on `ExportArchive` internally.
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/models/sequential.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/core.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/function.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/image.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/linalg.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/math.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/nn.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/node.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/numpy.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/operation.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adam.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/lion.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/random/random.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/random/seed_generator.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/saving/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/saving/keras_saveable.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/saving/keras_saveable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/saving/object_registration.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/saving/saving_api.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/testing/test_case.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/testing/test_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/trainers/trainer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/tree/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/tree/tree_api.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/__init__.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/code_stats.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/file_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/image_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/io_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/module_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/naming.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/progbar.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/python_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/tf_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from keras.src import backend
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 def get_tensor_spec(t, dynamic_batch=False, name=None):
     """Returns a `TensorSpec` given a single `Tensor` or `TensorSpec`."""
     if isinstance(t, tf.TypeSpec):
         spec = t
@@ -21,7 +22,19 @@
         return spec
 
     shape_list = shape.as_list()
     shape_list[0] = None
     shape = tf.TensorShape(shape_list)
     spec._shape = shape
     return spec
+
+
+def ensure_tensor(inputs, dtype=None):
+    """Ensures the input is a Tensor, SparseTensor or RaggedTensor."""
+    if not isinstance(inputs, (tf.Tensor, tf.SparseTensor, tf.RaggedTensor)):
+        if backend.backend() == "torch" and backend.is_tensor(inputs):
+            # Plain `np.asarray()` conversion fails with PyTorch.
+            inputs = backend.convert_to_numpy(inputs)
+        inputs = tf.convert_to_tensor(inputs, dtype)
+    if dtype is not None and inputs.dtype != dtype:
+        inputs = tf.cast(inputs, dtype)
+    return inputs
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras/src/utils/tracking.py` & `keras_nightly-3.3.3.dev2024052403/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024052303
+Version: 3.3.3.dev2024052403
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024052303/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.3.dev2024052403/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024052303/setup.py` & `keras_nightly-3.3.3.dev2024052403/setup.py`

 * *Files identical despite different names*

