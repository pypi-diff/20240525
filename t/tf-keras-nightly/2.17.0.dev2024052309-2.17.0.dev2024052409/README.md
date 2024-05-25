# Comparing `tmp/tf_keras_nightly-2.17.0.dev2024052309.tar.gz` & `tmp/tf_keras_nightly-2.17.0.dev2024052409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_keras_nightly-2.17.0.dev2024052309.tar", last modified: Thu May 23 09:53:51 2024, max compression
+gzip compressed data, was "tf_keras_nightly-2.17.0.dev2024052409.tar", last modified: Fri May 24 09:49:46 2024, max compression
```

## Comparing `tf_keras_nightly-2.17.0.dev2024052309.tar` & `tf_keras_nightly-2.17.0.dev2024052409.tar`

### file list

```diff
@@ -1,868 +1,868 @@
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/
--rw-r--r--   0 kbuilder  (1035) kbuilder  (1036)     1637 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/PKG-INFO
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       38 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/setup.cfg
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3952 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/setup.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      911 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      671 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/backend/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      162 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/backend/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      176 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/losses/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      153 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/losses/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      181 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/models/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       99 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      167 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.943574 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/activations/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      791 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/activations/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1137 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      161 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2437 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/layers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      163 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/layers/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/rnn_cell/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      674 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/rnn_cell/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/activations/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      749 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/activations/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5425 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/convnext/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      469 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/convnext/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/densenet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      342 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/densenet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/efficientnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      701 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/efficientnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/efficientnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      673 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/efficientnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/imagenet_utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      177 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/imagenet_utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/inception_resnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      263 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/inception_resnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/inception_v3/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/inception_v3/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/mobilenet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/mobilenet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/mobilenet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/mobilenet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/mobilenet_v3/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      173 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/mobilenet_v3/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/nasnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      276 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/nasnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/regnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1505 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/regnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet50/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      215 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet50/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet_rs/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      586 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet_rs/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      346 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/vgg16/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/vgg16/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/vgg19/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/vgg19/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/xception/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      221 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/xception/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/backend/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6650 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/backend/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/callbacks/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      854 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/callbacks/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/callbacks/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/callbacks/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/constraints/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      767 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/constraints/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.947575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      408 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/boston_housing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/boston_housing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/cifar10/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/cifar10/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/cifar100/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       88 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/cifar100/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/fashion_mnist/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       93 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/fashion_mnist/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/imdb/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      138 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/imdb/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/mnist/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       85 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/mnist/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/reuters/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/datasets/reuters/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/estimator/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       89 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/estimator/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      409 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/export/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       92 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/export/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/initializers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1951 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/initializers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9377 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      385 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/experimental/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      632 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/experimental/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/losses/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2760 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/losses/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/metrics/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5143 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/metrics/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/mixed_precision/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      142 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/mixed_precision/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      625 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/models/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      820 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      577 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/schedules/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      804 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/schedules/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/image/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1060 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/image/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/sequence/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      285 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/sequence/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/text/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      329 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/text/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/regularizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      488 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/regularizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/saving/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      681 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/saving/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2231 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/utils/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      189 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/utils/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1180 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      755 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/backend/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      162 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/backend/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.951575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      176 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/losses/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      153 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/losses/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      181 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/models/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       99 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      167 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/activations/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      791 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/activations/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5425 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/convnext/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      469 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/convnext/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/densenet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      342 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/densenet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/efficientnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      701 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/efficientnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/efficientnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      673 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/efficientnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/imagenet_utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      177 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/imagenet_utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/inception_resnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      263 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/inception_resnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/inception_v3/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/inception_v3/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/mobilenet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/mobilenet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/mobilenet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/mobilenet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/mobilenet_v3/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      173 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/mobilenet_v3/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/nasnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      276 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/nasnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/regnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1505 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/regnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet50/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      215 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet50/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet_rs/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      586 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet_rs/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      346 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/vgg16/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/vgg16/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/vgg19/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/vgg19/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/xception/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      221 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/xception/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/backend/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6588 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/backend/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/backend/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      220 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/backend/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/callbacks/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      903 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/callbacks/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/callbacks/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      178 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/callbacks/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/constraints/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      767 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/constraints/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      408 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/boston_housing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/boston_housing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/cifar10/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/cifar10/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/cifar100/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       88 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/cifar100/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.955575 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/fashion_mnist/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       93 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/fashion_mnist/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/imdb/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      138 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/imdb/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/mnist/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       85 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/mnist/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/reuters/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/datasets/reuters/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/dtensor/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       91 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/dtensor/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/dtensor/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      156 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/dtensor/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/dtensor/experimental/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      331 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/dtensor/experimental/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/estimator/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      114 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/estimator/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      507 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/export/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       92 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/export/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/initializers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2333 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/initializers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10388 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      474 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/experimental/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1574 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/experimental/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/losses/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2737 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/losses/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/metrics/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5069 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/metrics/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/metrics/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/metrics/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/mixed_precision/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/mixed_precision/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      557 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/models/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/models/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      123 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/models/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      935 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      587 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      577 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/schedules/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      804 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/schedules/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      428 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/image/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1116 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/image/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/sequence/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      285 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/sequence/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/text/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      329 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/text/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/regularizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      634 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/regularizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/saving/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      681 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/saving/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2763 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       97 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      189 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5159 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/convnext/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      469 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/convnext/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.959576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/densenet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      342 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/densenet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/efficientnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      701 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/efficientnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/efficientnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      673 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/efficientnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/imagenet_utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      177 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/imagenet_utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/inception_resnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      263 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/inception_resnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/inception_v3/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/inception_v3/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/mobilenet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/mobilenet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/mobilenet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/mobilenet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/mobilenet_v3/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      173 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/mobilenet_v3/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/nasnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      276 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/nasnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/regnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1505 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/regnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet50/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      215 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet50/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet_rs/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      586 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet_rs/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet_v2/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      346 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet_v2/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/vgg16/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/vgg16/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/vgg19/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/vgg19/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/xception/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      221 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/xception/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/backend/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6574 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/backend/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/backend/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      220 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/backend/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/callbacks/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      889 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/callbacks/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/callbacks/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      178 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/callbacks/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/constraints/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      767 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/constraints/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      310 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/boston_housing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/boston_housing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/cifar10/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/cifar10/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/cifar100/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       88 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/cifar100/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/fashion_mnist/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       93 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/fashion_mnist/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/imdb/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      138 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/imdb/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/mnist/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       85 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/mnist/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/reuters/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/datasets/reuters/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/dtensor/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       77 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/dtensor/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/dtensor/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      142 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/dtensor/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.963576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/dtensor/experimental/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      331 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/dtensor/experimental/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/estimator/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      114 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/estimator/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      507 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/export/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       92 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/export/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/initializers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2333 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/initializers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10374 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      460 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/experimental/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1574 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/experimental/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/losses/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2737 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/losses/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/metrics/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5055 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/metrics/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/metrics/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/metrics/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/mixed_precision/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/mixed_precision/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      543 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/models/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/models/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      123 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/models/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      893 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      587 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      577 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/schedules/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      804 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/schedules/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      386 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/image/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1116 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/image/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/sequence/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      285 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/sequence/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/text/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      329 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/text/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/__init__.py
--r-xr-xr-x   0 kbuilder  (1035) kbuilder  (1036)     1821 2024-05-23 09:53:18.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/projector_config_pb2.py
--r-xr-xr-x   0 kbuilder  (1035) kbuilder  (1036)     1585 2024-05-23 09:53:17.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/saved_metadata_pb2.py
--r-xr-xr-x   0 kbuilder  (1035) kbuilder  (1036)     1119 2024-05-23 09:53:18.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/versions_pb2.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/regularizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      634 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/regularizers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.967576 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/saving/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      681 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/saving/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.971577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1502 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22630 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/activations.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.971577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3701 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    25610 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/convnext.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17402 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/densenet.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    26654 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/efficientnet.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    41435 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/efficientnet_v2.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16678 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/imagenet_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16214 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/inception_resnet_v2.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16330 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/inception_v3.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    20134 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/mobilenet.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22096 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/mobilenet_v2.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24602 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/mobilenet_v3.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32736 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/nasnet.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    55777 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/regnet.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22308 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/resnet.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    33458 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/resnet_rs.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6903 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/resnet_v2.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10113 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/vgg16.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10328 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/vgg19.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13648 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/xception.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   248504 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/backend.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4516 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/backend_config.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.971577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      714 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7669 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/benchmark_util.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6567 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/distribution_util.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2248 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/model_memory_profile.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   133627 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/callbacks.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22154 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/callbacks_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13949 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/constraints.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.975577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       51 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3391 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/boston_housing.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1394 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/cifar.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3767 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/cifar10.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3559 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/cifar100.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3635 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/fashion_mnist.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8290 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/imdb.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3085 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/mnist.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8309 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/reuters.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.975577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      734 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8547 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/dataset_creator_model_fit_test_base.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    29244 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distribute_coordinator_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6449 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distributed_file_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4726 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distributed_training_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    49035 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distributed_training_utils_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24084 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/keras_correctness_test_base.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1639 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/model_collection_base.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1406 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/model_combinations.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8902 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/multi_worker_testing_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5883 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/optimizer_combinations.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10323 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/saved_model_test_base.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3773 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/simple_models.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3101 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/strategy_combinations.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3642 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/test_example.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1462 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/tpu_strategy_test_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9202 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/worker_training_state.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.975577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      791 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5544 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/integration_test_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22627 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/layout_map.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9902 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/lazy_variable.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4572 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/test_util.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6441 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/utils.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.979577 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   156299 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_layer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    35795 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_layer_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   102488 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_layer_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12650 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_preprocessing_layer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    31757 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/compile_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    71752 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/data_adapter.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    70182 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/functional.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11048 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/functional_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18258 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/input_layer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12076 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/input_spec.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28858 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/keras_tensor.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13860 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/node.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4325 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/partial_batch_padding_handler.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      853 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/saving.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22974 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/sequential.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   193232 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30903 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_arrays_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32084 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_distributed_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15377 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_eager_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32773 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_generator_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8733 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    82703 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_utils_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   153046 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_v1.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/estimator/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17022 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/estimator/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/export/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      748 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/export/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    23707 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/export/export_lib.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8915 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/base_feature_layer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8008 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/dense_features.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6216 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/dense_features_v2.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7681 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/sequence_feature_column.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9049 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    42738 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/initializers.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18926 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/initializers_v1.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14613 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1097 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2174 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/elu.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2618 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/leaky_relu.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4431 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/prelu.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4281 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/relu.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4105 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/softmax.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2503 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/thresholded_relu.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.983578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      945 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7485 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/additive_attention.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8682 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/attention.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10814 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/base_dense_attention.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30279 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/multi_head_attention.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.987578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3355 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17565 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/base_conv.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9525 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/base_depthwise_conv.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10923 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/base_separable_conv.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7623 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11885 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv1d_transpose.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8613 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14496 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv2d_transpose.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8270 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15002 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv3d_transpose.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8930 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/depthwise_conv1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8759 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/depthwise_conv2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9393 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/separable_conv1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8928 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/separable_conv2d.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.987578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2426 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2248 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/activation.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12936 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/dense.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14007 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/einsum_dense.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13525 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/embedding.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1301 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/identity.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16481 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/lambda_layer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3340 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/masking.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21066 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/tf_op_layer.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.987578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/experimental/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10730 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/experimental/dynamic_embedding.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13720 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/experimental/dynamic_lookup.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11321 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/kernelized.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.987578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      925 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15039 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/locally_connected1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16660 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/locally_connected2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8489 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/locally_connected_utils.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.991578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1647 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3006 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/add.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3140 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/average.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9806 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/base_merge.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8609 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/concatenate.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8325 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/dot.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2905 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/maximum.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2212 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/minimum.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2868 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/multiply.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3125 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/subtract.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1141 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/noise.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.991578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    68515 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/batch_normalization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1191 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/batch_normalization_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10028 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/group_normalization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14013 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/layer_normalization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4984 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/spectral_normalization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2611 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/unit_normalization.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.991578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2590 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4998 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/average_pooling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5484 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/average_pooling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3809 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/average_pooling3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2712 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_global_pooling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2712 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_global_pooling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2724 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_global_pooling3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4122 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_pooling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4614 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_pooling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5173 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_pooling3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3686 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_average_pooling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3120 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_average_pooling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3051 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_average_pooling3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3197 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_max_pooling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3063 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_max_pooling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3021 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_max_pooling3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4451 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/max_pooling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6338 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/max_pooling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3786 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/max_pooling3d.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.995578 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.999579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2845 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/bucketized_column_dense_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2949 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_encoding_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2809 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_hash_dense_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2723 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_hash_varlen_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3588 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_dense_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3437 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_varlen_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2863 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_dense_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3169 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_dense_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3101 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_varlen_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2795 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_varlen_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3776 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/discretization_adapt_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2836 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/embedding_dense_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2831 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/embedding_varlen_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4814 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/feature_column_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2835 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/hashed_crossing_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3624 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/hashing_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5467 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/image_preproc_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4475 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_adapt_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4941 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_forward_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4420 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/normalization_adapt_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3324 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/weighted_embedding_varlen_benchmark.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9104 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/category_encoding.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17798 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/discretization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8617 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/hashed_crossing.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11401 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/hashing.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    67714 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/image_preprocessing.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    42580 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/index_lookup.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21005 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/integer_lookup.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16684 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/normalization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11363 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/preprocessing_stage.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7185 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/preprocessing_test_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5310 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/preprocessing_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19179 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/string_lookup.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30467 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/text_vectorization.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.999579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1369 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1942 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/activity_regularization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3800 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/alpha_dropout.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5019 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/dropout.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2906 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/gaussian_dropout.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2855 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/gaussian_noise.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2402 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/spatial_dropout1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3485 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/spatial_dropout2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3503 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/spatial_dropout3d.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:50.999579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1583 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3278 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/cropping1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8415 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/cropping2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11945 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/cropping3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4567 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/flatten.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2958 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/permute.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2242 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/repeat_vector.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5409 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/reshape.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2588 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/up_sampling1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5055 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/up_sampling2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4727 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/up_sampling3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3040 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/zero_padding1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5949 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/zero_padding2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6669 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/zero_padding3d.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.003579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3007 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4481 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/abstract_rnn_cell.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    25008 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_conv_lstm.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18539 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_conv_rnn.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5412 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_cudnn_rnn.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    41959 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_rnn.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3150 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_wrapper.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22580 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/bidirectional.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    26867 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/cell_wrappers.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8761 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/conv_lstm1d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8874 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/conv_lstm2d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8969 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/conv_lstm3d.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8625 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/cudnn_gru.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10114 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/cudnn_lstm.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7610 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/dropout_rnn_cell_mixin.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    50746 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/gru.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9922 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/gru_lstm_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15761 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/gru_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    25382 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/legacy_cell_wrappers.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    52845 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/legacy_cells.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    53482 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/lstm.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15790 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/lstm_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8180 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/rnn_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19937 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/simple_rnn.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8308 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/stacked_rnn_cells.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15573 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/time_distributed.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10216 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/serialization.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.003579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       77 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    26544 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/base.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    83036 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/convolutional.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19184 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/core.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4626 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/migration_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22264 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/normalization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    31913 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/pooling.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    45096 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/variable_scope_shim.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   110698 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/losses.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.007579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9699 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17514 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/accuracy_metrics.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    36498 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/base_metric.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    65973 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/confusion_metrics.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12000 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/f_score_metrics.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4132 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/hinge_metrics.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28530 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/iou_metrics.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12132 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/probabilistic_metrics.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7236 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/py_metric.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21098 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/regression_metrics.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.007579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1110 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22394 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/autocast_variable.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6252 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/device_compatibility_check.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    64122 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/loss_scale_optimizer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22734 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/policy.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8523 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/test_util.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.007579 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1823 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    36839 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/cloning.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7301 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/sharpness_aware_minimization.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.011580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13044 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6174 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adadelta.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8651 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adafactor.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5387 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adagrad.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9203 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adam.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6613 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adamax.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8861 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adamw.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9807 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/ftrl.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.011580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      690 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6588 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adadelta.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7189 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adagrad.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22176 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adam.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8123 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adamax.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12644 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/ftrl.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7965 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/gradient_descent.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9998 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/nadam.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    69599 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/optimizer_v2.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14732 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/rmsprop.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30051 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy_learning_rate_decay.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6157 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/lion.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7452 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/nadam.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    61536 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/optimizer.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32631 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/optimizer_v1.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7890 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/rmsprop.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.011580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/schedules/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1101 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/schedules/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    48113 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6763 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/sgd.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6157 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/utils.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.011580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      813 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8035 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/linear.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9921 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/wide_deep.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.011580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1711 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   104419 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/image.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13891 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/sequence.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22771 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/text.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16608 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/regularizers.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.015580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.015580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    42438 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/hdf5_format.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4140 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/model_config.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    23612 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/save.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.015580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5104 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/base_serialization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1779 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/constants.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1040 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/create_test_saved_model.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8056 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/json_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8418 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/layer_serialization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    57007 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/load.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1907 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/metric_serialization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2792 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/model_serialization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1180 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/network_serialization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3250 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/order_preserving_set.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6395 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/save.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    29751 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/save_impl.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15009 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/serialized_attributes.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9953 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13745 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saving_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22285 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/serialization.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7830 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/object_registration.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2605 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/pickle_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13152 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/saving_api.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24673 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/saving_lib.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30445 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/serialization_lib.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.015580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      690 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8092 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/keras_doctest_lib.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21736 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/test_combinations.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    40307 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/test_utils.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.019580 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15307 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/get_config_samples.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4638 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/keras_doctest.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10830 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/model_architectures.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5515 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/model_subclassing_test_util.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3129 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14818 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/audio_dataset.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4418 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/control_flow_util.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    20188 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/conv_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    38188 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/data_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4746 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/dataset_creator.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28016 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/dataset_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28868 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/feature_space.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19516 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/generic_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14792 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/image_dataset.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17840 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/image_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4027 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/io_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      882 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/keras_logging.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4517 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/kernelized_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7365 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/kpl_test_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    41764 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/layer_utils.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      923 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/legacy/__init__.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16919 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/losses_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    39803 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/metrics_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      856 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/mode_keys.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4805 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/np_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6879 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/object_identity.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18474 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/sidecar_evaluator.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9586 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/steps_per_execution_tuning.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11084 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/text_dataset.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1300 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/tf_contextlib.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14237 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/tf_inspect.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24082 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/tf_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5380 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/timed_threads.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10612 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/timeseries_dataset.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6335 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/traceback_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4925 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/version_utils.py
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19002 2024-05-23 09:53:46.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/vis_utils.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2735 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/experimental/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       97 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/experimental/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/legacy/
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      189 2024-05-23 09:53:49.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/legacy/__init__.py
-drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-23 09:53:51.023581 tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/
--rw-r--r--   0 kbuilder  (1035) kbuilder  (1036)     1637 2024-05-23 09:53:50.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/PKG-INFO
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28025 2024-05-23 09:53:50.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/SOURCES.txt
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-23 09:53:50.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/dependency_links.txt
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       23 2024-05-23 09:53:50.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/requires.txt
--rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        9 2024-05-23 09:53:50.000000 tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/top_level.txt
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/
+-rw-r--r--   0 kbuilder  (1035) kbuilder  (1036)     1637 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/PKG-INFO
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       38 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/setup.cfg
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3952 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/setup.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.201489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      911 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.201489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      671 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.201489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/backend/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      162 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/backend/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.201489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      176 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.201489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/losses/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      153 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/losses/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.201489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      181 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/models/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       99 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      167 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/activations/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      791 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/activations/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1137 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      161 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2437 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/layers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      163 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/layers/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/rnn_cell/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      674 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/rnn_cell/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/activations/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      749 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/activations/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5425 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/convnext/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      469 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/convnext/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/densenet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      342 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/densenet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/efficientnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      701 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/efficientnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/efficientnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      673 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/efficientnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/imagenet_utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      177 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/imagenet_utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/inception_resnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      263 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/inception_resnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/inception_v3/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/inception_v3/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/mobilenet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/mobilenet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/mobilenet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/mobilenet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/mobilenet_v3/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      173 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/mobilenet_v3/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/nasnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      276 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/nasnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/regnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1505 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/regnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet50/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      215 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet50/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet_rs/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      586 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet_rs/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      346 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/vgg16/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/vgg16/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.205489 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/vgg19/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/vgg19/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/xception/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      221 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/xception/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/backend/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6650 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/backend/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/callbacks/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      854 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/callbacks/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/callbacks/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/callbacks/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/constraints/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      767 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/constraints/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      408 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/boston_housing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/boston_housing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/cifar10/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/cifar10/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/cifar100/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       88 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/cifar100/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/fashion_mnist/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       93 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/fashion_mnist/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/imdb/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      138 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/imdb/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/mnist/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       85 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/mnist/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/reuters/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/datasets/reuters/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/estimator/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       89 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/estimator/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      409 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/export/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       92 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/export/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/initializers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1951 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/initializers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9377 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      385 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/experimental/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      632 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/experimental/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/losses/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2760 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/losses/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/metrics/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5143 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/metrics/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/mixed_precision/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      142 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/mixed_precision/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      625 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/models/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      820 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      577 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/schedules/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      804 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/schedules/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/image/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1060 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/image/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/sequence/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      285 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/sequence/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/text/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      329 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/text/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.209490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/regularizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      488 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/regularizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/saving/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      681 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/saving/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2231 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/utils/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      189 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/utils/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1180 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      755 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/backend/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      162 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/backend/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      176 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/losses/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      153 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/losses/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      181 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/models/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       99 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      167 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/activations/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      791 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/activations/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5425 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/convnext/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      469 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/convnext/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/densenet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      342 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/densenet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/efficientnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      701 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/efficientnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/efficientnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      673 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/efficientnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/imagenet_utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      177 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/imagenet_utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/inception_resnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      263 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/inception_resnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/inception_v3/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/inception_v3/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/mobilenet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/mobilenet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/mobilenet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/mobilenet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/mobilenet_v3/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      173 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/mobilenet_v3/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/nasnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      276 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/nasnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/regnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1505 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/regnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet50/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      215 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet50/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet_rs/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      586 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet_rs/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      346 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/vgg16/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/vgg16/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.213490 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/vgg19/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/vgg19/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/xception/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      221 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/xception/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/backend/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6588 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/backend/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/backend/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      220 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/backend/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/callbacks/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      903 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/callbacks/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/callbacks/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      178 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/callbacks/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/constraints/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      767 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/constraints/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      408 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/boston_housing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/boston_housing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/cifar10/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/cifar10/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/cifar100/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       88 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/cifar100/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/fashion_mnist/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       93 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/fashion_mnist/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/imdb/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      138 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/imdb/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/mnist/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       85 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/mnist/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/reuters/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/datasets/reuters/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/dtensor/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       91 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/dtensor/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/dtensor/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      156 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/dtensor/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/dtensor/experimental/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      331 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/dtensor/experimental/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/estimator/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      114 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/estimator/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      507 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/export/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       92 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/export/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/initializers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2333 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/initializers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10388 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      474 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/experimental/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1574 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/experimental/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/losses/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2737 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/losses/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/metrics/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5069 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/metrics/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/metrics/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/metrics/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/mixed_precision/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/mixed_precision/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      557 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/models/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/models/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      123 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/models/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      935 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.217491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      587 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      577 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/schedules/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      804 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/schedules/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      428 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/image/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1116 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/image/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/sequence/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      285 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/sequence/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/text/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      329 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/text/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/regularizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      634 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/regularizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/saving/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      681 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/saving/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2763 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       97 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      189 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5159 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/convnext/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      469 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/convnext/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/densenet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      342 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/densenet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/efficientnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      701 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/efficientnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/efficientnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      673 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/efficientnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/imagenet_utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      177 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/imagenet_utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/inception_resnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      263 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/inception_resnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/inception_v3/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/inception_v3/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/mobilenet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      225 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/mobilenet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/mobilenet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      236 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/mobilenet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/mobilenet_v3/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      173 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/mobilenet_v3/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/nasnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      276 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/nasnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/regnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1505 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/regnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet50/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      215 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet50/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet_rs/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      586 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet_rs/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet_v2/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      346 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet_v2/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/vgg16/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/vgg16/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/vgg19/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      209 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/vgg19/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/xception/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      221 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/xception/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.221491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/backend/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6574 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/backend/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/backend/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      220 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/backend/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/callbacks/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      889 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/callbacks/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/callbacks/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      178 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/callbacks/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/constraints/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      767 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/constraints/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      310 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/boston_housing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       94 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/boston_housing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/cifar10/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/cifar10/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/cifar100/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       88 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/cifar100/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/fashion_mnist/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       93 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/fashion_mnist/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/imdb/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      138 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/imdb/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/mnist/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       85 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/mnist/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/reuters/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      202 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/datasets/reuters/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/dtensor/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       77 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/dtensor/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/dtensor/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      142 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/dtensor/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/dtensor/experimental/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      331 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/dtensor/experimental/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/estimator/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      114 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/estimator/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      507 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/export/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       92 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/export/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/initializers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2333 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/initializers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10374 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      460 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/experimental/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1574 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/experimental/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/losses/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2737 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/losses/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/metrics/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5055 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/metrics/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/metrics/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       87 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/metrics/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/mixed_precision/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      325 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/mixed_precision/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      543 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/models/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/models/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      123 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/models/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      893 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      587 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      577 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/schedules/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      804 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/schedules/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.225491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      386 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/image/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1116 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/image/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/sequence/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      285 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/sequence/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/text/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      329 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/text/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/__init__.py
+-r-xr-xr-x   0 kbuilder  (1035) kbuilder  (1036)     1821 2024-05-24 09:49:17.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/projector_config_pb2.py
+-r-xr-xr-x   0 kbuilder  (1035) kbuilder  (1036)     1585 2024-05-24 09:49:17.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/saved_metadata_pb2.py
+-r-xr-xr-x   0 kbuilder  (1035) kbuilder  (1036)     1119 2024-05-24 09:49:17.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/versions_pb2.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/regularizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      634 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/regularizers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/saving/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      681 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/saving/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.229491 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1502 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22630 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/activations.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.233492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3701 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    25610 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/convnext.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17402 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/densenet.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    26654 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/efficientnet.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    41435 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/efficientnet_v2.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16678 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/imagenet_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16214 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/inception_resnet_v2.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16330 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/inception_v3.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    20134 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/mobilenet.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22096 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/mobilenet_v2.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24602 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/mobilenet_v3.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32736 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/nasnet.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    55777 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/regnet.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22308 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/resnet.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    33458 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/resnet_rs.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6903 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/resnet_v2.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10113 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/vgg16.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10328 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/vgg19.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13648 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/xception.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   248504 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/backend.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4516 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/backend_config.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.233492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      714 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7669 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/benchmark_util.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6567 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/distribution_util.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2248 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/model_memory_profile.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   133627 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/callbacks.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22154 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/callbacks_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13949 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/constraints.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.233492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       51 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3391 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/boston_housing.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1394 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/cifar.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3767 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/cifar10.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3559 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/cifar100.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3635 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/fashion_mnist.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8290 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/imdb.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3085 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/mnist.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8309 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/reuters.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.237492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      734 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8547 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/dataset_creator_model_fit_test_base.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    29244 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distribute_coordinator_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6449 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distributed_file_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4726 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distributed_training_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    49035 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distributed_training_utils_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24084 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/keras_correctness_test_base.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1639 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/model_collection_base.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1406 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/model_combinations.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8902 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/multi_worker_testing_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5883 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/optimizer_combinations.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10323 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/saved_model_test_base.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3773 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/simple_models.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3101 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/strategy_combinations.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3642 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/test_example.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1462 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/tpu_strategy_test_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9202 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/worker_training_state.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.237492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      791 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5544 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/integration_test_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22627 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/layout_map.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9902 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/lazy_variable.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4572 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/test_util.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6441 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/utils.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.241492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   156299 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_layer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    35795 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_layer_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   102488 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_layer_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12650 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_preprocessing_layer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    31757 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/compile_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    71752 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/data_adapter.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    70182 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/functional.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11048 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/functional_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18258 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/input_layer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12076 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/input_spec.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28858 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/keras_tensor.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13860 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/node.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4325 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/partial_batch_padding_handler.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      853 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/saving.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22974 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/sequential.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   193232 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30903 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_arrays_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32084 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_distributed_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15377 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_eager_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32773 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_generator_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8733 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    82703 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_utils_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   153046 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_v1.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.241492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/estimator/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17022 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/estimator/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.241492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/export/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      748 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/export/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    23707 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/export/export_lib.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.241492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8915 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/base_feature_layer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8008 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/dense_features.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6216 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/dense_features_v2.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7681 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/sequence_feature_column.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.241492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9049 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    42738 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/initializers.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18926 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/initializers_v1.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.245492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14613 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.245492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1097 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2174 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/elu.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2618 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/leaky_relu.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4431 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/prelu.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4281 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/relu.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4105 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/softmax.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2503 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/thresholded_relu.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.245492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      945 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7485 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/additive_attention.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8682 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/attention.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10814 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/base_dense_attention.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30279 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/multi_head_attention.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.245492 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3355 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17565 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/base_conv.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9525 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10923 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/base_separable_conv.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7623 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11885 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv1d_transpose.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8613 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14496 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv2d_transpose.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8270 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15002 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv3d_transpose.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8930 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8759 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9393 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/separable_conv1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8928 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/separable_conv2d.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.249493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2426 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2248 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/activation.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12936 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/dense.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14007 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/einsum_dense.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13525 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/embedding.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1301 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/identity.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16481 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/lambda_layer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3340 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/masking.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21066 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/tf_op_layer.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.249493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/experimental/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10730 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/experimental/dynamic_embedding.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13720 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/experimental/dynamic_lookup.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11321 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/kernelized.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.249493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      925 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15039 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/locally_connected1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16660 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/locally_connected2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8489 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/locally_connected_utils.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.249493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1647 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3006 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/add.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3140 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/average.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9806 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/base_merge.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8609 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/concatenate.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8325 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/dot.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2905 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/maximum.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2212 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/minimum.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2868 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/multiply.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3125 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/subtract.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1141 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/noise.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.253493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    68515 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/batch_normalization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1191 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/batch_normalization_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10028 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/group_normalization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14013 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/layer_normalization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4984 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/spectral_normalization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2611 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/unit_normalization.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.253493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2590 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4998 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/average_pooling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5484 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/average_pooling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3809 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/average_pooling3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2712 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_global_pooling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2712 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_global_pooling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2724 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_global_pooling3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4122 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_pooling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4614 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_pooling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5173 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_pooling3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3686 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_average_pooling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3120 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_average_pooling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3051 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_average_pooling3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3197 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_max_pooling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3063 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_max_pooling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3021 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_max_pooling3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4451 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/max_pooling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6338 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/max_pooling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3786 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/max_pooling3d.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.257493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.257493 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2845 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/bucketized_column_dense_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2949 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_encoding_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2809 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_hash_dense_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2723 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_hash_varlen_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3588 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_dense_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3437 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_varlen_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2863 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_dense_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3169 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_dense_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3101 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_varlen_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2795 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_varlen_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3776 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/discretization_adapt_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2836 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/embedding_dense_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2831 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/embedding_varlen_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4814 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/feature_column_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2835 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/hashed_crossing_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3624 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/hashing_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5467 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/image_preproc_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4475 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_adapt_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4941 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_forward_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4420 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/normalization_adapt_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3324 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/weighted_embedding_varlen_benchmark.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9104 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/category_encoding.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17798 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/discretization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8617 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/hashed_crossing.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11401 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/hashing.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    67714 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/image_preprocessing.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    42580 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/index_lookup.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21005 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/integer_lookup.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16684 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/normalization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11363 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/preprocessing_stage.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7185 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/preprocessing_test_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5310 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/preprocessing_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19179 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/string_lookup.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30467 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/text_vectorization.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.261494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1369 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1942 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/activity_regularization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3800 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/alpha_dropout.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5019 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/dropout.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2906 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/gaussian_dropout.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2855 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/gaussian_noise.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2402 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/spatial_dropout1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3485 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/spatial_dropout2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3503 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/spatial_dropout3d.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.261494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1583 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3278 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/cropping1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8415 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/cropping2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11945 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/cropping3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4567 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/flatten.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2958 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/permute.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2242 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/repeat_vector.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5409 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/reshape.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2588 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/up_sampling1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5055 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/up_sampling2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4727 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/up_sampling3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3040 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/zero_padding1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5949 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/zero_padding2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6669 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/zero_padding3d.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.265494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3007 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4481 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/abstract_rnn_cell.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    25008 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_conv_lstm.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18539 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_conv_rnn.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5412 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_cudnn_rnn.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    41959 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_rnn.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3150 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_wrapper.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22580 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/bidirectional.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    26867 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/cell_wrappers.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8761 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/conv_lstm1d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8874 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/conv_lstm2d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8969 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/conv_lstm3d.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8625 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/cudnn_gru.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10114 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/cudnn_lstm.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7610 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/dropout_rnn_cell_mixin.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    50746 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/gru.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9922 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/gru_lstm_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15761 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/gru_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    25382 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/legacy_cell_wrappers.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    52845 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/legacy_cells.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    53482 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/lstm.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15790 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/lstm_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8180 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/rnn_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19937 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/simple_rnn.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8308 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15573 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/time_distributed.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10216 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/serialization.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.265494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       77 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    26544 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/base.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    83036 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/convolutional.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19184 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/core.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4626 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/migration_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22264 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/normalization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    31913 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/pooling.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    45096 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/variable_scope_shim.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   110698 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/losses.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.269494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9699 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17514 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/accuracy_metrics.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    36498 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/base_metric.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    65973 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/confusion_metrics.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12000 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/f_score_metrics.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4132 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/hinge_metrics.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28530 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/iou_metrics.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12132 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/probabilistic_metrics.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7236 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/py_metric.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21098 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/regression_metrics.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.269494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1110 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22394 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/autocast_variable.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6252 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/device_compatibility_check.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    64122 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/loss_scale_optimizer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22734 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/policy.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8523 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/test_util.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.269494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1823 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    36839 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/cloning.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7301 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/sharpness_aware_minimization.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.273494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13044 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6174 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adadelta.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8651 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adafactor.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5387 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adagrad.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9203 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adam.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6613 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adamax.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8861 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adamw.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9807 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/ftrl.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.273494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      690 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6588 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adadelta.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7189 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adagrad.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22176 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adam.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8123 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adamax.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    12644 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/ftrl.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7965 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/gradient_descent.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9998 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/nadam.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    69599 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/optimizer_v2.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14732 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/rmsprop.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30051 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy_learning_rate_decay.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6157 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/lion.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7452 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/nadam.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    61536 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/optimizer.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    32631 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/optimizer_v1.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7890 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/rmsprop.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.273494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/schedules/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1101 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/schedules/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    48113 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6763 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/sgd.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6157 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/utils.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.273494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      813 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8035 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/linear.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9921 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/wide_deep.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.273494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1711 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)   104419 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/image.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13891 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/sequence.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22771 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/text.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16608 2024-05-24 09:49:40.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/regularizers.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.273494 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.277495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    42438 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/hdf5_format.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4140 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/model_config.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    23612 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/save.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.277495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5104 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/base_serialization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1779 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/constants.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1040 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/create_test_saved_model.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8056 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/json_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8418 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/layer_serialization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    57007 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/load.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1907 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/metric_serialization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2792 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/model_serialization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1180 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/network_serialization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3250 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/order_preserving_set.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6395 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/save.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    29751 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/save_impl.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15009 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/serialized_attributes.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9953 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13745 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saving_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    22285 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/serialization.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7830 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/object_registration.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2605 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/pickle_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    13152 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/saving_api.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24673 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/saving_lib.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    30445 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/serialization_lib.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.277495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      690 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     8092 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/keras_doctest_lib.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    21736 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/test_combinations.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    40307 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/test_utils.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.277495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    15307 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/get_config_samples.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4638 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/keras_doctest.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10830 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/model_architectures.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5515 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/model_subclassing_test_util.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     3129 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14818 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/audio_dataset.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4418 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/control_flow_util.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    20188 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/conv_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    38188 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/data_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4746 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/dataset_creator.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28016 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/dataset_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28868 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/feature_space.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19516 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/generic_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14792 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/image_dataset.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    17840 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/image_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4027 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/io_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      882 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/keras_logging.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4517 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/kernelized_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     7365 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/kpl_test_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    41764 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/layer_utils.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      923 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/legacy/__init__.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    16919 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/losses_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    39803 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/metrics_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      856 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/mode_keys.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4805 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/np_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6879 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/object_identity.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    18474 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/sidecar_evaluator.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     9586 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/steps_per_execution_tuning.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    11084 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/text_dataset.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     1300 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/tf_contextlib.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    14237 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/tf_inspect.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    24082 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/tf_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     5380 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/timed_threads.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    10612 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/timeseries_dataset.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     6335 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/traceback_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     4925 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/version_utils.py
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    19002 2024-05-24 09:49:41.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/vis_utils.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)     2735 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/experimental/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       97 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/experimental/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/legacy/
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)      189 2024-05-24 09:49:44.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/legacy/__init__.py
+drwxrwxr-x   0 kbuilder  (1035) kbuilder  (1036)        0 2024-05-24 09:49:46.285495 tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/
+-rw-r--r--   0 kbuilder  (1035) kbuilder  (1036)     1637 2024-05-24 09:49:46.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/PKG-INFO
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)    28025 2024-05-24 09:49:46.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/SOURCES.txt
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        1 2024-05-24 09:49:46.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/dependency_links.txt
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)       23 2024-05-24 09:49:46.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/requires.txt
+-rw-rw-r--   0 kbuilder  (1035) kbuilder  (1036)        9 2024-05-24 09:49:46.000000 tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/top_level.txt
```

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/PKG-INFO` & `tf_keras_nightly-2.17.0.dev2024052409/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf_keras-nightly
-Version: 2.17.0.dev2024052309
+Version: 2.17.0.dev2024052409
 Summary: Deep learning for humans.
 Home-page: https://keras.io/
 Download-URL: https://github.com/keras-team/tf-keras/tags
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache 2.0
 Keywords: keras,tensorflow,machine learning,deep learning
```

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/setup.py` & `tf_keras_nightly-2.17.0.dev2024052409/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             "You must fill the 'PACKAGE' and 'VERSION' "
             "tags before running setup.py. If you are trying to "
             "build a fresh package, you should be using "
             "`pip_build.py` instead of `setup.py`."
         )
 
 # pin version to that of tensorflow or tf_nightly.
-version = "2.17.0.dev2024052309".lower()
+version = "2.17.0.dev2024052409".lower()
 major_version, minor_version, *_ = version.split(".")
 next_minor_version = int(minor_version) + 1
 if "nightly" in "tf_keras-nightly":
     base_version = version.split(".dev")[0]  # 2.17.0.dev2024021419
     install_requires = [f"tf-nightly~={base_version}.dev"]
 elif "rc" in version:
     # 2.17.0rc0
@@ -57,15 +57,15 @@
         f"<{major_version}.{next_minor_version}"
     ]
 
 setuptools.setup(
     name="tf_keras-nightly",
     # Version strings with `-` characters are semver compatible,
     # but incompatible with pip. For pip, we will remove all `-`` characters.
-    version="2.17.0.dev2024052309",
+    version="2.17.0.dev2024052409",
     description="Deep learning for humans.",
     long_description=DESCRIPTION,
     url="https://keras.io/",
     download_url="https://github.com/keras-team/tf-keras/tags",
     author="Keras team",
     author_email="keras-users@googlegroups.com",
     packages=setuptools.find_packages(),
```

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from tf_keras import saving
 from tf_keras import utils
 from tf_keras.src.engine.input_layer import Input
 from tf_keras.src.engine.sequential import Sequential
 from tf_keras.src.engine.training import Model
 
 
-__version__ = "2.17.0.dev2024052309"
+__version__ = "2.17.0.dev2024052409"
```

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/__internal__/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/__internal__/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/activations/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/layers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/__internal__/legacy/rnn_cell/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/__internal__/legacy/rnn_cell/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/activations/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/efficientnet/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/efficientnet_v2/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/regnet/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/regnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/applications/resnet_rs/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/applications/resnet_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/backend/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/callbacks/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/constraints/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/initializers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/layers/experimental/preprocessing/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/layers/experimental/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/losses/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/metrics/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/models/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/legacy/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/optimizers/schedules/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/preprocessing/image/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/saving/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v1/keras/utils/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v1/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/__internal__/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/__internal__/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/activations/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/efficientnet/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/efficientnet_v2/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/regnet/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/regnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/applications/resnet_rs/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/applications/resnet_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/backend/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/callbacks/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/constraints/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/initializers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/layers/experimental/preprocessing/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/layers/experimental/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/losses/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/metrics/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/models/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/experimental/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/legacy/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/optimizers/schedules/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/preprocessing/image/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/regularizers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/saving/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/api/_v2/keras/utils/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/api/_v2/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/efficientnet/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/efficientnet_v2/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/regnet/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/regnet/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/applications/resnet_rs/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/applications/resnet_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/backend/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/callbacks/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/constraints/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/initializers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/layers/experimental/preprocessing/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/layers/experimental/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/losses/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/metrics/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/models/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/experimental/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/legacy/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/optimizers/schedules/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/preprocessing/image/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/projector_config_pb2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/projector_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/saved_metadata_pb2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/saved_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/protobuf/versions_pb2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/protobuf/versions_pb2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/regularizers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/saving/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/activations.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/activations.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/convnext.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/densenet.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/efficientnet.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/efficientnet_v2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/imagenet_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/inception_resnet_v2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/inception_v3.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/mobilenet.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/mobilenet_v2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/mobilenet_v3.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/nasnet.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/regnet.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/regnet.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/resnet.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/resnet_rs.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/resnet_rs.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/resnet_v2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/vgg16.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/vgg19.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/applications/xception.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/backend.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/backend.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/backend_config.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/backend_config.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/benchmark_util.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/benchmark_util.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/distribution_util.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/distribution_util.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/benchmarks/model_memory_profile.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/benchmarks/model_memory_profile.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/callbacks.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/callbacks.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/callbacks_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/callbacks_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/constraints.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/constraints.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/boston_housing.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/cifar.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/cifar10.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/cifar100.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/fashion_mnist.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/imdb.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/mnist.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/datasets/reuters.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/dataset_creator_model_fit_test_base.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/dataset_creator_model_fit_test_base.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distribute_coordinator_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distribute_coordinator_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distributed_file_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distributed_file_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distributed_training_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distributed_training_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/distributed_training_utils_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/distributed_training_utils_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/keras_correctness_test_base.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/keras_correctness_test_base.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/model_collection_base.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/model_collection_base.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/model_combinations.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/model_combinations.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/multi_worker_testing_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/multi_worker_testing_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/optimizer_combinations.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/optimizer_combinations.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/saved_model_test_base.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/saved_model_test_base.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/simple_models.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/simple_models.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/strategy_combinations.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/strategy_combinations.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/test_example.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/test_example.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/tpu_strategy_test_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/tpu_strategy_test_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/distribute/worker_training_state.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/distribute/worker_training_state.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/integration_test_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/layout_map.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/layout_map.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/lazy_variable.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/lazy_variable.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/test_util.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/test_util.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/dtensor/utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/dtensor/utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_layer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_layer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_layer_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_layer_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_layer_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_layer_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/base_preprocessing_layer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/base_preprocessing_layer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/compile_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/compile_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/data_adapter.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/data_adapter.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/functional.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/functional.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/functional_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/functional_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/input_layer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/input_layer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/input_spec.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/input_spec.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/keras_tensor.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/node.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/node.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/partial_batch_padding_handler.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/partial_batch_padding_handler.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/saving.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/saving.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/sequential.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_arrays_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_arrays_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_distributed_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_distributed_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_eager_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_eager_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_generator_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_generator_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_utils_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_utils_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/engine/training_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/engine/training_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/estimator/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/estimator/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/export/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/export/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/export/export_lib.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/base_feature_layer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/base_feature_layer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/dense_features.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/dense_features.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/dense_features_v2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/dense_features_v2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/feature_column/sequence_feature_column.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/feature_column/sequence_feature_column.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/initializers.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/initializers.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/initializers/initializers_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/initializers/initializers_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/elu.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/elu.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/leaky_relu.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/prelu.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/prelu.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/relu.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/relu.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/softmax.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/softmax.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/activation/thresholded_relu.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/activation/thresholded_relu.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/additive_attention.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/attention.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/base_dense_attention.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/base_dense_attention.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/attention/multi_head_attention.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/base_conv.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/base_depthwise_conv.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/base_separable_conv.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv1d_transpose.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv2d_transpose.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/conv3d_transpose.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/depthwise_conv1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/depthwise_conv2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/separable_conv1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/convolutional/separable_conv2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/activation.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/activation.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/dense.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/einsum_dense.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/embedding.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/identity.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/lambda_layer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/masking.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/core/tf_op_layer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/core/tf_op_layer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/experimental/dynamic_embedding.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/experimental/dynamic_embedding.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/experimental/dynamic_lookup.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/experimental/dynamic_lookup.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/kernelized.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/kernelized.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/locally_connected1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/locally_connected1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/locally_connected2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/locally_connected2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/locally_connected/locally_connected_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/locally_connected/locally_connected_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/add.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/average.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/base_merge.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/concatenate.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/dot.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/maximum.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/minimum.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/multiply.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/merging/subtract.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/noise.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/noise.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/batch_normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/batch_normalization_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/batch_normalization_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/group_normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/layer_normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/spectral_normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/normalization/unit_normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/average_pooling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/average_pooling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/average_pooling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_global_pooling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_global_pooling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_global_pooling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_global_pooling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_global_pooling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_global_pooling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_pooling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_pooling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_pooling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_pooling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/base_pooling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/base_pooling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_average_pooling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_average_pooling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_average_pooling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_max_pooling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_max_pooling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/global_max_pooling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/max_pooling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/max_pooling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/pooling/max_pooling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/bucketized_column_dense_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/bucketized_column_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_encoding_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_encoding_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_hash_dense_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_hash_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_hash_varlen_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_hash_varlen_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_dense_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_varlen_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_file_varlen_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_dense_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_dense_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_varlen_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_indicator_varlen_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_varlen_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/category_vocab_list_varlen_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/discretization_adapt_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/discretization_adapt_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/embedding_dense_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/embedding_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/embedding_varlen_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/embedding_varlen_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/feature_column_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/feature_column_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/hashed_crossing_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/hashed_crossing_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/hashing_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/hashing_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/image_preproc_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/image_preproc_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_adapt_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_adapt_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_forward_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/index_lookup_forward_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/normalization_adapt_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/normalization_adapt_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/benchmarks/weighted_embedding_varlen_benchmark.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/benchmarks/weighted_embedding_varlen_benchmark.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/category_encoding.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/discretization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/hashed_crossing.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/hashing.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/image_preprocessing.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/image_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/index_lookup.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/integer_lookup.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/preprocessing_stage.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/preprocessing_stage.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/preprocessing_test_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/preprocessing_test_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/preprocessing_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/string_lookup.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/preprocessing/text_vectorization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/activity_regularization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/alpha_dropout.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/dropout.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/gaussian_dropout.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/gaussian_noise.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/spatial_dropout1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/spatial_dropout1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/spatial_dropout2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/spatial_dropout2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/regularization/spatial_dropout3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/regularization/spatial_dropout3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/cropping1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/cropping2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/cropping3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/flatten.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/permute.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/repeat_vector.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/reshape.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/up_sampling1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/up_sampling2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/up_sampling3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/zero_padding1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/zero_padding2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/reshaping/zero_padding3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/abstract_rnn_cell.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/abstract_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_conv_lstm.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_conv_lstm.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_conv_rnn.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_conv_rnn.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_cudnn_rnn.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_cudnn_rnn.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_rnn.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_rnn.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/base_wrapper.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/bidirectional.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/cell_wrappers.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/cell_wrappers.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/conv_lstm1d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/conv_lstm2d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/conv_lstm3d.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/cudnn_gru.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/cudnn_gru.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/cudnn_lstm.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/cudnn_lstm.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/dropout_rnn_cell_mixin.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/dropout_rnn_cell_mixin.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/gru.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/gru_lstm_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/gru_lstm_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/gru_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/gru_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/legacy_cell_wrappers.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/legacy_cell_wrappers.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/legacy_cells.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/legacy_cells.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/lstm.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/lstm_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/lstm_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/rnn_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/rnn_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/simple_rnn.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/stacked_rnn_cells.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/rnn/time_distributed.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/layers/serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/layers/serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/base.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/base.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/convolutional.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/convolutional.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/core.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/core.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/migration_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/migration_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/normalization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/normalization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/pooling.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/pooling.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/legacy_tf_layers/variable_scope_shim.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/legacy_tf_layers/variable_scope_shim.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/losses.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/losses.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/accuracy_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/base_metric.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/base_metric.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/confusion_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/f_score_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/hinge_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/iou_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/probabilistic_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/py_metric.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/py_metric.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/metrics/regression_metrics.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/autocast_variable.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/autocast_variable.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/device_compatibility_check.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/device_compatibility_check.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/loss_scale_optimizer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/policy.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/policy.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/mixed_precision/test_util.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/mixed_precision/test_util.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/cloning.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/models/sharpness_aware_minimization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/models/sharpness_aware_minimization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adadelta.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adafactor.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adagrad.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adam.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adamax.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/adamw.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/ftrl.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adadelta.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adadelta.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adagrad.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adagrad.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adam.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adam.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/adamax.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/adamax.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/ftrl.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/ftrl.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/gradient_descent.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/nadam.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/nadam.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/optimizer_v2.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/optimizer_v2.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy/rmsprop.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy/rmsprop.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/legacy_learning_rate_decay.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/legacy_learning_rate_decay.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/lion.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/nadam.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/optimizer.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/optimizer_v1.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/optimizer_v1.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/rmsprop.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/schedules/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/schedules/learning_rate_schedule.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/sgd.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/optimizers/utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/linear.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/linear.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/premade_models/wide_deep.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/premade_models/wide_deep.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/image.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/sequence.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/preprocessing/text.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/regularizers.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/regularizers.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/hdf5_format.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/hdf5_format.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/model_config.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/model_config.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/save.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/save.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/base_serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/base_serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/constants.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/constants.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/create_test_saved_model.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/create_test_saved_model.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/json_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/json_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/layer_serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/layer_serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/load.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/load.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/metric_serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/metric_serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/model_serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/model_serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/network_serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/network_serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/order_preserving_set.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/order_preserving_set.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/save.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/save.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/save_impl.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/save_impl.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/serialized_attributes.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/serialized_attributes.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saved_model/utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saved_model/utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/saving_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/saving_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/legacy/serialization.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/legacy/serialization.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/object_registration.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/pickle_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/saving_api.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/saving_lib.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/saving/serialization_lib.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/keras_doctest_lib.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/keras_doctest_lib.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/test_combinations.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/test_combinations.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/testing_infra/test_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/testing_infra/test_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/get_config_samples.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/get_config_samples.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/keras_doctest.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/keras_doctest.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/model_architectures.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/model_architectures.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/tests/model_subclassing_test_util.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/tests/model_subclassing_test_util.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/audio_dataset.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/audio_dataset.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/control_flow_util.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/control_flow_util.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/conv_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/conv_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/data_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/dataset_creator.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/dataset_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/feature_space.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/feature_space.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/generic_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/image_dataset.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/image_dataset.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/image_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/io_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/keras_logging.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/keras_logging.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/kernelized_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/kernelized_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/kpl_test_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/kpl_test_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/layer_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/legacy/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/losses_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/losses_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/metrics_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/mode_keys.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/mode_keys.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/np_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/np_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/object_identity.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/object_identity.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/sidecar_evaluator.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/sidecar_evaluator.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/steps_per_execution_tuning.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/steps_per_execution_tuning.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/text_dataset.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/text_dataset.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/tf_contextlib.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/tf_contextlib.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/tf_inspect.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/tf_inspect.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/tf_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/timed_threads.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/timed_threads.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/timeseries_dataset.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/timeseries_dataset.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/traceback_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/version_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/src/utils/vis_utils.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/src/utils/vis_utils.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras/utils/__init__.py` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/PKG-INFO` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf_keras-nightly
-Version: 2.17.0.dev2024052309
+Version: 2.17.0.dev2024052409
 Summary: Deep learning for humans.
 Home-page: https://keras.io/
 Download-URL: https://github.com/keras-team/tf-keras/tags
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache 2.0
 Keywords: keras,tensorflow,machine learning,deep learning
```

### Comparing `tf_keras_nightly-2.17.0.dev2024052309/tf_keras_nightly.egg-info/SOURCES.txt` & `tf_keras_nightly-2.17.0.dev2024052409/tf_keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

