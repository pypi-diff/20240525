# Comparing `tmp/Audyn-0.0.0.tar.gz` & `tmp/audyn-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Audyn-0.0.0.tar", last modified: Sat Oct 21 10:41:04 2023, max compression
+gzip compressed data, was "audyn-0.0.1.dev6.tar", last modified: Sat May 25 01:26:12 2024, max compression
```

## Comparing `Audyn-0.0.0.tar` & `audyn-0.0.1.dev6.tar`

### file list

```diff
@@ -1,19 +1,245 @@
-drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2023-10-21 10:41:04.113302 Audyn-0.0.0/
-drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2023-10-21 10:41:04.110779 Audyn-0.0.0/Audyn.egg-info/
--rw-r--r--   0 t-hasumi   (501) staff       (20)    14227 2023-10-21 10:41:04.000000 Audyn-0.0.0/Audyn.egg-info/PKG-INFO
--rw-r--r--   0 t-hasumi   (501) staff       (20)      266 2023-10-21 10:41:04.000000 Audyn-0.0.0/Audyn.egg-info/SOURCES.txt
--rw-r--r--   0 t-hasumi   (501) staff       (20)        1 2023-10-21 10:41:04.000000 Audyn-0.0.0/Audyn.egg-info/dependency_links.txt
--rw-r--r--   0 t-hasumi   (501) staff       (20)      152 2023-10-21 10:41:04.000000 Audyn-0.0.0/Audyn.egg-info/requires.txt
--rw-r--r--   0 t-hasumi   (501) staff       (20)        6 2023-10-21 10:41:04.000000 Audyn-0.0.0/Audyn.egg-info/top_level.txt
--rw-r--r--   0 t-hasumi   (501) staff       (20)    11343 2023-10-21 10:25:57.000000 Audyn-0.0.0/LICENSE
--rw-r--r--   0 t-hasumi   (501) staff       (20)      103 2023-10-21 10:25:57.000000 Audyn-0.0.0/MANIFEST.in
--rw-r--r--   0 t-hasumi   (501) staff       (20)    14227 2023-10-21 10:41:04.112754 Audyn-0.0.0/PKG-INFO
--rw-r--r--   0 t-hasumi   (501) staff       (20)      503 2023-10-21 10:25:57.000000 Audyn-0.0.0/README.md
-drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2023-10-21 10:41:04.110968 Audyn-0.0.0/audyn/
--rw-r--r--   0 t-hasumi   (501) staff       (20)      406 2023-10-21 10:25:57.000000 Audyn-0.0.0/audyn/__init__.py
-drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2023-10-21 10:41:04.108732 Audyn-0.0.0/cpp_extensions/
-drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2023-10-21 10:41:04.111162 Audyn-0.0.0/cpp_extensions/monotonic_align/
--rw-r--r--   0 t-hasumi   (501) staff       (20)     4245 2023-10-21 10:25:57.000000 Audyn-0.0.0/cpp_extensions/monotonic_align/monotonic_align.cpp
--rw-r--r--   0 t-hasumi   (501) staff       (20)      937 2023-10-21 10:25:57.000000 Audyn-0.0.0/pyproject.toml
--rw-r--r--   0 t-hasumi   (501) staff       (20)       38 2023-10-21 10:41:04.113370 Audyn-0.0.0/setup.cfg
--rw-r--r--   0 t-hasumi   (501) staff       (20)      962 2023-10-21 10:25:57.000000 Audyn-0.0.0/setup.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.450969 audyn-0.0.1.dev6/
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.448407 audyn-0.0.1.dev6/Audyn.egg-info/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    15672 2024-05-25 01:26:12.000000 audyn-0.0.1.dev6/Audyn.egg-info/PKG-INFO
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6960 2024-05-25 01:26:12.000000 audyn-0.0.1.dev6/Audyn.egg-info/SOURCES.txt
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        1 2024-05-25 01:26:12.000000 audyn-0.0.1.dev6/Audyn.egg-info/dependency_links.txt
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      294 2024-05-25 01:26:12.000000 audyn-0.0.1.dev6/Audyn.egg-info/requires.txt
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        6 2024-05-25 01:26:12.000000 audyn-0.0.1.dev6/Audyn.egg-info/top_level.txt
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    11343 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/LICENSE
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      130 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/MANIFEST.in
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    15672 2024-05-25 01:26:12.450349 audyn-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1586 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/README.md
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.385261 audyn-0.0.1.dev6/audyn/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1803 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.390313 audyn-0.0.1.dev6/audyn/criterion/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      118 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      879 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/autoregressive.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2840 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/base.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    21689 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/contrastive.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3908 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/distance.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4245 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/fastspeech.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2128 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/flow.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1318 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/gan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3058 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/glowtts.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2484 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/hifigan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      578 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/lsgan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2516 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/melspectrogram.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2712 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/rvqvae.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3304 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/ssast.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2758 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/criterion/vqvae.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.391683 audyn-0.0.1.dev6/audyn/functional/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       80 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/functional/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3848 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/functional/activation.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8160 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/functional/clustering.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3189 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/functional/vector_quantization.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.392910 audyn-0.0.1.dev6/audyn/metrics/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1826 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/metrics/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2770 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/metrics/base.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6852 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/metrics/crossmodal.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     5225 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/metrics/retrieval.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.402308 audyn-0.0.1.dev6/audyn/models/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1406 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    22863 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/ast.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    14966 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/encodec.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    24701 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/fastspeech.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      266 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/gan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    36953 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/glowtts.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    51571 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/hifigan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    14540 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/lextransformer.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8720 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/passt.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6217 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/pixelsnail.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    14811 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/roformer.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8581 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/rvqvae.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    24207 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/soundstream.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    36717 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/ssast.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    10205 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/text_to_wave.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      743 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/vae.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6003 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/vqvae.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    22598 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/waveglow.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    29209 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/models/wavenet.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.410090 audyn-0.0.1.dev6/audyn/modules/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    39619 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/activation.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     5823 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/duration_predictor.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    10135 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/encodec.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    12470 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/fastspeech.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2274 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/film.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6088 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/flow.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    11266 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/glow.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    26475 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/glowtts.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       53 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/normalization.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    19123 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/passt.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     9307 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/pixelcnn.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    17649 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/pixelsnail.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6179 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/positional_encoding.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     5656 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/rvq.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8804 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/soundstream.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    15116 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/vit.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8441 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/vq.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      106 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/vqvae.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8922 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/waveglow.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    21125 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/modules/wavenet.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.410908 audyn-0.0.1.dev6/audyn/optim/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     5818 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/optim/lr_scheduler.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    54359 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/optim/optimizer.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.414091 audyn-0.0.1.dev6/audyn/transforms/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      596 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6117 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/ast.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6497 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/birdclef.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    26255 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/cqt.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3199 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/hifigan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1585 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/hubert.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    16265 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/kaldi.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2910 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/transforms/librosa.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.414652 audyn-0.0.1.dev6/audyn/utils/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    23664 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.415261 audyn-0.0.1.dev6/audyn/utils/alignment/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1938 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/alignment/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2278 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/alignment/monotonic_align.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4846 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/clip_grad.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.420123 audyn-0.0.1.dev6/audyn/utils/data/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2698 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.422454 audyn-0.0.1.dev6/audyn/utils/data/audioset/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      125 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1310 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/_download.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       72 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/ast.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     7128 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/composer.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    15507 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/dataset.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3932 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/distributed.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3246 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/audioset/sampler.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.375138 audyn-0.0.1.dev6/audyn/utils/data/birdclef/
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.424086 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     5410 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      825 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/_download.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1757 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/collator.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    10889 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/composer.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     7292 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/dataset.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.424533 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/models/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1799 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/birdclef/birdclef2024/models/baseline.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.424870 audyn-0.0.1.dev6/audyn/utils/data/clotho/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1057 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/clotho/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.426056 audyn-0.0.1.dev6/audyn/utils/data/clotho/text/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3231 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/clotho/text/indexing.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      830 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/clotho/text/normalization.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      239 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/clotho/text/symbols.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      655 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/clotho/text/tokenization.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.426674 audyn-0.0.1.dev6/audyn/utils/data/cmudict/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4436 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/cmudict/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1000 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/cmudict/indexing.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3318 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/collator.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3321 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/composer.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     8715 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/dataloader.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     6603 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/dataset.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     9622 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/distributed.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    10325 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/postprocess.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4950 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/sampler.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.426941 audyn-0.0.1.dev6/audyn/utils/data/tacotron/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      823 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/tacotron/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.428247 audyn-0.0.1.dev6/audyn/utils/data/tacotron/text/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      826 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/tacotron/text/indexing.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3099 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/tacotron/text/normalization.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2552 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/tacotron/text/numbers.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1132 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/tacotron/text/symbols.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      726 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/tacotron/text/tokenization.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1336 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/data/webdataset.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.428533 audyn-0.0.1.dev6/audyn/utils/distributed/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3355 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/distributed/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.431357 audyn-0.0.1.dev6/audyn/utils/driver/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      497 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.431674 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      234 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/config.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.432380 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/criterion/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      353 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/criterion/cross_entropy.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      750 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/criterion/vqvae.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.432703 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/data/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       22 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/data/defaults.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.433348 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/lr_scheduler/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/lr_scheduler/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/lr_scheduler/none.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       86 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/lr_scheduler/transformer.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.434241 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/model/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/model/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       26 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/model/gan.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.435380 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/optimizer/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       27 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/optimizer/adam.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      159 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/optimizer/adam_ema.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       28 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/optimizer/adamw.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       26 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/optimizer/gan.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.436519 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/preprocess/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       97 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/preprocess/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       64 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/preprocess/ljspeech_text-to-feat.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       45 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/preprocess/text-to-feat.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       45 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/preprocess/text-to-wave.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.438277 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      138 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/cpu.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      144 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/cuda.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      143 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/cuda_amp.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      163 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/cuda_ddp.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      162 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/cuda_ddp_amp.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      133 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      138 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/system/mps.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.438773 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.439036 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/dataloader/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       79 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/dataloader/defaults.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.439604 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/dataset/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       54 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/dataset/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       90 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/dataset/torch.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      424 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      637 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/test/text_to_wave.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.440704 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.441197 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/clip_gradient/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/clip_gradient/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      138 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/clip_gradient/gan.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.441769 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataloader/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      162 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataloader/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      200 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataloader/sequential-batch.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.442855 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataset/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      115 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataset/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      207 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataset/sortable-torch.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      187 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataset/torch.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      225 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/dataset/webdataset.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      601 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      927 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/gan.yaml
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.443319 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/record/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/record/defaults.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1509 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/record/template.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      927 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/template.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      988 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_conf_template/train/text-to-feat+pretrained_feat-to-wave.yaml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      774 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/_decorator.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    98408 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/base.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2362 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/feat_to_wave.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    39990 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/gan.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    18325 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/text_to_feat.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4822 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/driver/text_to_wave.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.443574 audyn-0.0.1.dev6/audyn/utils/duration/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1339 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/duration/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.443810 audyn-0.0.1.dev6/audyn/utils/github/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     3474 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/github/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.444300 audyn-0.0.1.dev6/audyn/utils/hydra/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      440 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/hydra/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)    17292 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/hydra/utils.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.444631 audyn-0.0.1.dev6/audyn/utils/lab/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      374 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/lab/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.444881 audyn-0.0.1.dev6/audyn/utils/logging/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1375 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/logging/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.445161 audyn-0.0.1.dev6/audyn/utils/model/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     2269 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/model/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.445435 audyn-0.0.1.dev6/audyn/utils/music/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1397 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/music/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.445711 audyn-0.0.1.dev6/audyn/utils/parallel/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      663 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/parallel/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.445963 audyn-0.0.1.dev6/audyn/utils/tensorboard/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      630 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/tensorboard/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.447391 audyn-0.0.1.dev6/audyn/utils/text/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     7727 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/text/__init__.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      491 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/text/indexing.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)      467 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/text/normalization.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1292 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/text/pronunciation.py
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1398 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/text/tokenization.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.447653 audyn-0.0.1.dev6/audyn/utils/textgrid/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1185 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/audyn/utils/textgrid/__init__.py
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.380115 audyn-0.0.1.dev6/cpp_extensions/
+drwxr-xr-x   0 t-hasumi   (501) staff       (20)        0 2024-05-25 01:26:12.447923 audyn-0.0.1.dev6/cpp_extensions/monotonic_align/
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4436 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/cpp_extensions/monotonic_align/monotonic_align.cpp
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     1378 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/pyproject.toml
+-rw-r--r--   0 t-hasumi   (501) staff       (20)       38 2024-05-25 01:26:12.451053 audyn-0.0.1.dev6/setup.cfg
+-rw-r--r--   0 t-hasumi   (501) staff       (20)     4561 2024-05-25 01:20:33.000000 audyn-0.0.1.dev6/setup.py
```

### Comparing `Audyn-0.0.0/Audyn.egg-info/PKG-INFO` & `audyn-0.0.1.dev6/Audyn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Audyn
-Version: 0.0.0
+Version: 0.0.1.dev6
 Summary: A PyTorch toolkit for audio synthesis.
 Author: Takuya Hasumi
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,33 +205,44 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: url, https://github.com/tky823/Audyn
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib_resources<6.2; python_version == "3.8"
 Requires-Dist: omegaconf
 Requires-Dist: hydra-core
 Requires-Dist: matplotlib
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchtext
 Requires-Dist: torchvision
 Requires-Dist: tensorboard
+Requires-Dist: webdataset
+Requires-Dist: inflect
 Provides-Extra: recipes
 Requires-Dist: tqdm; extra == "recipes"
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 
 # Audyn
+[![codecov](https://codecov.io/gh/tky823/Audyn/graph/badge.svg?token=7R29QDGXLQ)](https://codecov.io/gh/tky823/Audyn)
+
 Audyn is PyTorch toolkit for audio synthesis.
 
 ## Installation
 You can install by pip.
 ```shell
 pip install git+https://github.com/tky823/Audyn.git
 ```
@@ -244,17 +255,48 @@
 
 If you need to run recipes, add `[recipes]` as follows:
 ```shell
 # In Audyn/
 pip install -e ".[recipes]"
 ```
 
+If you use MacOS, you may need to set `MACOSX_DEPLOYMENT_TARGET` during installation to build C++ related modules.
+
+### C++ extension
+We use [C++ extension](https://pytorch.org/tutorials/advanced/cpp_extension.html) to search monotonic alignment in some models (e.g. GlowTTS).
+To take full advantage of computational efficiency, set appropriate value of `OMP_NUM_THREADS` and `CXX` during installation:
+
+```shell
+# In Audyn/
+export CXX=<PATH/TO/CPP/COMPILER>  # e.g. /usr/bin/c++
+export OMP_NUM_THREADS=<SUITABLE/VALUE/FOR/ENVIRONMENT>
+pip install -e "."
+```
+
 ## Development
 ```shell
 # In Audyn/
 pip install -e ".[recipes,dev,tests]"
 ```
 
+## Build Documentation Locally (optional)
+To build the documentation locally, you have to include `docs` when installing `Audyn`.
+```shell
+pip install -e ".[docs]"
+```
+
+When you build the documentation, run the following command.
+```shell
+cd docs/
+make html
+```
+
+Or, you can build the documentation automatically using `sphinx-autobuild`.
+```shell
+# in Audyn/
+sphinx-autobuild docs docs/_build/html
+```
+
 ## Test
 ```shell
 pytest tests/package
 ```
```

### Comparing `Audyn-0.0.0/LICENSE` & `audyn-0.0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `Audyn-0.0.0/PKG-INFO` & `audyn-0.0.1.dev6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Audyn
-Version: 0.0.0
+Version: 0.0.1.dev6
 Summary: A PyTorch toolkit for audio synthesis.
 Author: Takuya Hasumi
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,33 +205,44 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: url, https://github.com/tky823/Audyn
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib_resources<6.2; python_version == "3.8"
 Requires-Dist: omegaconf
 Requires-Dist: hydra-core
 Requires-Dist: matplotlib
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchtext
 Requires-Dist: torchvision
 Requires-Dist: tensorboard
+Requires-Dist: webdataset
+Requires-Dist: inflect
 Provides-Extra: recipes
 Requires-Dist: tqdm; extra == "recipes"
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 
 # Audyn
+[![codecov](https://codecov.io/gh/tky823/Audyn/graph/badge.svg?token=7R29QDGXLQ)](https://codecov.io/gh/tky823/Audyn)
+
 Audyn is PyTorch toolkit for audio synthesis.
 
 ## Installation
 You can install by pip.
 ```shell
 pip install git+https://github.com/tky823/Audyn.git
 ```
@@ -244,17 +255,48 @@
 
 If you need to run recipes, add `[recipes]` as follows:
 ```shell
 # In Audyn/
 pip install -e ".[recipes]"
 ```
 
+If you use MacOS, you may need to set `MACOSX_DEPLOYMENT_TARGET` during installation to build C++ related modules.
+
+### C++ extension
+We use [C++ extension](https://pytorch.org/tutorials/advanced/cpp_extension.html) to search monotonic alignment in some models (e.g. GlowTTS).
+To take full advantage of computational efficiency, set appropriate value of `OMP_NUM_THREADS` and `CXX` during installation:
+
+```shell
+# In Audyn/
+export CXX=<PATH/TO/CPP/COMPILER>  # e.g. /usr/bin/c++
+export OMP_NUM_THREADS=<SUITABLE/VALUE/FOR/ENVIRONMENT>
+pip install -e "."
+```
+
 ## Development
 ```shell
 # In Audyn/
 pip install -e ".[recipes,dev,tests]"
 ```
 
+## Build Documentation Locally (optional)
+To build the documentation locally, you have to include `docs` when installing `Audyn`.
+```shell
+pip install -e ".[docs]"
+```
+
+When you build the documentation, run the following command.
+```shell
+cd docs/
+make html
+```
+
+Or, you can build the documentation automatically using `sphinx-autobuild`.
+```shell
+# in Audyn/
+sphinx-autobuild docs docs/_build/html
+```
+
 ## Test
 ```shell
 pytest tests/package
 ```
```

### Comparing `Audyn-0.0.0/cpp_extensions/monotonic_align/monotonic_align.cpp` & `audyn-0.0.1.dev6/cpp_extensions/monotonic_align/monotonic_align.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,96 @@
 // NOTE: Some utilities are defined in not 'torch', but 'at' (ATen).
 
 #include <torch/extension.h>
 
-torch::Tensor viterbi_monotonic_alignment(torch::Tensor probs,
-                                          bool take_log = false)
+torch::Tensor search_monotonic_alignment_by_viterbi(
+    torch::Tensor probs, torch::Tensor tgt_lengths, torch::Tensor src_lengths, bool take_log = false)
 {
     int64_t batch_size = probs.size(0);
     int64_t max_tgt_length = probs.size(1);
     int64_t max_src_length = probs.size(2);
 
+    int64_t num_threads = torch::get_num_threads();
+    int64_t grain_size = std::ceil((batch_size - 1) / num_threads) + 1;
+
     double_t inf = std::numeric_limits<double_t>::infinity();
     torch::TensorOptions float32options = probs.options();
-    torch::TensorOptions int64options =
-        torch::TensorOptions().dtype(torch::kInt64).device(probs.device());
+    torch::TensorOptions int64options = torch::TensorOptions().dtype(torch::kInt64).device(probs.device());
+
+    torch::Tensor log_probs;
+    std::vector<int64_t> flattened_hard_align(batch_size * max_tgt_length * max_src_length, 0);
 
-    torch::Tensor hard_align = torch::zeros(
-        {batch_size, max_tgt_length, max_src_length}, int64options);
+    if (take_log)
+    {
+        log_probs = torch::log(probs);
+    }
+    else
+    {
+        log_probs = probs;
+    }
 
     torch::parallel_for(
-        0, batch_size, torch::internal::GRAIN_SIZE,
+        0, batch_size, grain_size,
         [&](int64_t start, int64_t end)
         {
             for (int64_t batch_idx = start; batch_idx < end; batch_idx++)
             {
-                torch::Tensor prob = probs.index({batch_idx});
-                torch::Tensor log_prob, sum_prob;
-                torch::Tensor log_seq_prob, prev_log_seq_prob, log_p;
-
-                int64_t tgt_length, src_length;
-                int64_t tgt_idx, src_idx;
-                int64_t start_src_idx, end_src_idx;
-                int64_t min_src_idx, max_src_idx;
-                torch::indexing::Slice slice;
-
-                if (take_log)
-                {
-                    log_prob = torch::log(prob);
-                }
-                else
-                {
-                    log_prob = prob;
-                    prob = torch::exp(log_prob);
-                }
-
-                sum_prob = prob.sum(/*dim=*/1);
-                tgt_length = torch::count_nonzero(sum_prob).item<int64_t>();
+                torch::Tensor log_prob = log_probs.index({batch_idx}).contiguous();
+                int64_t tgt_length = tgt_lengths.index({batch_idx}).item<int64_t>();
+                int64_t src_length = src_lengths.index({batch_idx}).item<int64_t>();
+                int64_t tgt_idx, src_idx, start_src_idx, end_src_idx, min_src_idx, max_src_idx;
+
+                float *data_ptr = log_prob.data_ptr<float>();
+                std::vector<float> flattened_log_prob(max_tgt_length * max_src_length);
+                std::vector<float> log_seq_prob(max_tgt_length * max_src_length, -inf);
 
-                sum_prob = prob.sum(/*dim=*/0);
-                src_length = torch::count_nonzero(sum_prob).item<int64_t>();
+                flattened_log_prob.assign(data_ptr, data_ptr + max_tgt_length * max_src_length);
 
                 assert(tgt_length >= src_length);
 
-                log_seq_prob = torch::full({max_tgt_length, max_src_length},
-                                           /*fill_value=*/-inf, float32options);
-
                 // forward
-                log_seq_prob.index_put_({0, 0}, 0);
+                log_seq_prob[0 * max_src_length + 0] = 0;
 
                 for (tgt_idx = 1; tgt_idx < tgt_length; tgt_idx++)
                 {
-                    start_src_idx =
-                        std::max((int64_t)0, src_length - tgt_length + tgt_idx);
+                    start_src_idx = std::max((int64_t)0, src_length - tgt_length + tgt_idx);
                     end_src_idx = std::min(src_length, tgt_idx + 1);
 
-                    for (src_idx = start_src_idx; src_idx < end_src_idx;
-                         src_idx++)
+                    for (src_idx = start_src_idx; src_idx < end_src_idx; src_idx++)
                     {
                         min_src_idx = std::max((int64_t)0, src_idx - 1);
                         max_src_idx = std::min(tgt_idx - 1, src_idx);
 
-                        slice = torch::indexing::Slice(min_src_idx,
-                                                       max_src_idx + 1);
-                        prev_log_seq_prob =
-                            log_seq_prob.index({tgt_idx - 1, slice});
-                        log_p = torch::max(prev_log_seq_prob) +
-                                log_prob.index({tgt_idx, src_idx});
-                        log_seq_prob.index_put_({tgt_idx, src_idx}, log_p);
+                        auto slice_start = log_seq_prob.begin() + (tgt_idx - 1) * max_src_length + min_src_idx;
+                        auto slice_end = log_seq_prob.begin() + (tgt_idx - 1) * max_src_length + max_src_idx + 1;
+                        auto max_prev_log_seq_prob = std::max_element(slice_start, slice_end);
+                        log_seq_prob[tgt_idx * max_src_length + src_idx] = *max_prev_log_seq_prob + flattened_log_prob[tgt_idx * max_src_length + src_idx];
                     }
                 }
 
                 // back track
                 src_idx = src_length - 1;
-                hard_align.index_put_({batch_idx, tgt_length - 1, src_idx}, 1);
+                flattened_hard_align[batch_idx * max_tgt_length * max_src_length + (tgt_length - 1) * max_src_length + src_idx] = 1;
 
                 for (tgt_idx = tgt_length - 1; tgt_idx > 0; tgt_idx--)
                 {
                     min_src_idx = std::max((int64_t)0, src_idx - 1);
                     max_src_idx = std::min(tgt_idx - 1, src_idx);
-                    slice =
-                        torch::indexing::Slice(min_src_idx, max_src_idx + 1);
-                    prev_log_seq_prob =
-                        log_seq_prob.index({tgt_idx - 1, slice});
-                    src_idx = min_src_idx +
-                              torch::argmax(prev_log_seq_prob).item<int64_t>();
-                    hard_align.index_put_({batch_idx, tgt_idx - 1, src_idx}, 1);
+                    auto slice_start = log_seq_prob.begin() + (tgt_idx - 1) * max_src_length + min_src_idx;
+                    auto slice_end = log_seq_prob.begin() + (tgt_idx - 1) * max_src_length + max_src_idx + 1;
+                    auto max_prev_log_seq_prob = std::max_element(slice_start, slice_end);
+                    src_idx = std::distance(log_seq_prob.begin() + (tgt_idx - 1) * max_src_length, max_prev_log_seq_prob);
+                    flattened_hard_align[batch_idx * max_tgt_length * max_src_length + (tgt_idx - 1) * max_src_length + src_idx] = 1;
                 }
             }
         });
 
-    return hard_align;
+    torch::Tensor hard_align = torch::from_blob(flattened_hard_align.data(), {batch_size, max_tgt_length, max_src_length}, int64options);
+
+    return hard_align.clone();
 }
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m)
 {
-    m.def("viterbi_monotonic_alignment", &viterbi_monotonic_alignment,
+    m.def("search_monotonic_alignment_by_viterbi", &search_monotonic_alignment_by_viterbi,
           "Search monotonic alignment by Viterbi algorithm");
 }
```

