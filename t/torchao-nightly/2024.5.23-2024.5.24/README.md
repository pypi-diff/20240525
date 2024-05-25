# Comparing `tmp/torchao_nightly-2024.5.23-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/torchao_nightly-2024.5.24-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,110 +1,113 @@
-Zip file size: 415886 bytes, number of entries: 108
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao_nightly-2024.5.23.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao_nightly.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/csrc/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/dtypes/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/kernel/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/quantization/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/sparsity/
--rwxr-xr-x  2.0 unx   810656 b- defN 24-May-23 00:31 torchao/_C.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      426 b- defN 24-May-23 00:31 torchao/__init__.py
--rw-r--r--  2.0 unx     4792 b- defN 24-May-23 00:31 torchao/ops.py
--rw-r--r--  2.0 unx      860 b- defN 24-May-23 00:31 torchao/utils.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/csrc/cuda/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/csrc/fp6_llm/
--rw-r--r--  2.0 unx       74 b- defN 24-May-23 00:31 torchao/csrc/init.cpp
--rw-r--r--  2.0 unx      251 b- defN 24-May-23 00:31 torchao/csrc/nms.cpp
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/csrc/cuda/fp6_llm/
--rw-r--r--  2.0 unx     5554 b- defN 24-May-23 00:31 torchao/csrc/cuda/nms.cu
--rw-r--r--  2.0 unx     9437 b- defN 24-May-23 00:31 torchao/csrc/cuda/fp6_llm/fp6_linear.cu
--rw-r--r--  2.0 unx     9472 b- defN 24-May-23 00:31 torchao/csrc/cuda/fp6_llm/weight_quant.cu
--rw-r--r--  2.0 unx      479 b- defN 24-May-23 00:31 torchao/csrc/fp6_llm/fp6_llm.cpp
--rw-r--r--  2.0 unx     9210 b- defN 24-May-23 00:31 torchao/csrc/fp6_llm/weight_prepacking.cpp
--rw-r--r--  2.0 unx      136 b- defN 24-May-23 00:31 torchao/dtypes/__init__.py
--rw-r--r--  2.0 unx    33918 b- defN 24-May-23 00:31 torchao/dtypes/nf4tensor.py
--rw-r--r--  2.0 unx    12448 b- defN 24-May-23 00:31 torchao/dtypes/uint4.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/kernel/__init__.py
--rw-r--r--  2.0 unx     7389 b- defN 24-May-23 00:31 torchao/kernel/autotuner.py
--rw-r--r--  2.0 unx     3238 b- defN 24-May-23 00:31 torchao/kernel/intmm.py
--rw-r--r--  2.0 unx    11678 b- defN 24-May-23 00:31 torchao/kernel/intmm_triton.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/common/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/dora/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/galore/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/hqq/
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/prototype/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/prototype/common/__init__.py
--rw-r--r--  2.0 unx     7071 b- defN 24-May-23 00:31 torchao/prototype/common/profiling_tools.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/dora/kernels/
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/prototype/dora/__init__.py
--rw-r--r--  2.0 unx     6639 b- defN 24-May-23 00:31 torchao/prototype/dora/dora_layer.py
--rw-r--r--  2.0 unx     3972 b- defN 24-May-23 00:31 torchao/prototype/dora/dora_profile.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/prototype/dora/kernels/__init__.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-23 00:31 torchao/prototype/dora/kernels/common.py
--rw-r--r--  2.0 unx    15366 b- defN 24-May-23 00:31 torchao/prototype/dora/kernels/custom_autotune.py
--rw-r--r--  2.0 unx     7641 b- defN 24-May-23 00:31 torchao/prototype/dora/kernels/matmul.py
--rw-r--r--  2.0 unx    16439 b- defN 24-May-23 00:31 torchao/prototype/dora/kernels/smallk.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/galore/kernels/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/prototype/galore/optim/
--rw-r--r--  2.0 unx       23 b- defN 24-May-23 00:31 torchao/prototype/galore/__init__.py
--rw-r--r--  2.0 unx     3195 b- defN 24-May-23 00:31 torchao/prototype/galore/utils.py
--rw-r--r--  2.0 unx      210 b- defN 24-May-23 00:31 torchao/prototype/galore/kernels/__init__.py
--rw-r--r--  2.0 unx    10675 b- defN 24-May-23 00:31 torchao/prototype/galore/kernels/adam_downproj_fused.py
--rw-r--r--  2.0 unx     4722 b- defN 24-May-23 00:31 torchao/prototype/galore/kernels/adam_step.py
--rw-r--r--  2.0 unx    15180 b- defN 24-May-23 00:31 torchao/prototype/galore/kernels/custom_autotune.py
--rw-r--r--  2.0 unx    11641 b- defN 24-May-23 00:31 torchao/prototype/galore/kernels/matmul.py
--rw-r--r--  2.0 unx     5978 b- defN 24-May-23 00:31 torchao/prototype/galore/kernels/quant.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/prototype/galore/optim/__init__.py
--rw-r--r--  2.0 unx    15716 b- defN 24-May-23 00:31 torchao/prototype/galore/optim/galore_torch.py
--rw-r--r--  2.0 unx       50 b- defN 24-May-23 00:31 torchao/prototype/hqq/__init__.py
--rw-r--r--  2.0 unx     7658 b- defN 24-May-23 00:31 torchao/prototype/hqq/hqq_tinygemm_linear.py
--rw-r--r--  2.0 unx    14227 b- defN 24-May-23 00:31 torchao/prototype/hqq/kernels.py
--rw-r--r--  2.0 unx     5512 b- defN 24-May-23 00:31 torchao/prototype/hqq/mixed_mm.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/quantization/prototype/
--rw-r--r--  2.0 unx    50342 b- defN 24-May-23 00:31 torchao/quantization/GPTQ.py
--rw-r--r--  2.0 unx     1700 b- defN 24-May-23 00:31 torchao/quantization/__init__.py
--rw-r--r--  2.0 unx    19369 b- defN 24-May-23 00:31 torchao/quantization/autoquant.py
--rw-r--r--  2.0 unx     2747 b- defN 24-May-23 00:31 torchao/quantization/dynamic_quant.py
--rw-r--r--  2.0 unx     7110 b- defN 24-May-23 00:31 torchao/quantization/quant_api.py
--rw-r--r--  2.0 unx    32825 b- defN 24-May-23 00:31 torchao/quantization/quant_primitives.py
--rw-r--r--  2.0 unx     9159 b- defN 24-May-23 00:31 torchao/quantization/smoothquant.py
--rw-r--r--  2.0 unx    42347 b- defN 24-May-23 00:31 torchao/quantization/subclass.py
--rw-r--r--  2.0 unx      754 b- defN 24-May-23 00:31 torchao/quantization/unified.py
--rw-r--r--  2.0 unx     3169 b- defN 24-May-23 00:31 torchao/quantization/utils.py
--rw-r--r--  2.0 unx     2742 b- defN 24-May-23 00:31 torchao/quantization/weight_only.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/quantization/prototype/__init__.py
--rw-r--r--  2.0 unx    12816 b- defN 24-May-23 00:31 torchao/quantization/prototype/qat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/sparsity/prototype/
--rw-r--r--  2.0 unx      508 b- defN 24-May-23 00:31 torchao/sparsity/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 24-May-23 00:31 torchao/sparsity/sparse_api.py
--rw-r--r--  2.0 unx     1708 b- defN 24-May-23 00:31 torchao/sparsity/utils.py
--rw-r--r--  2.0 unx     4156 b- defN 24-May-23 00:31 torchao/sparsity/wanda.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/sparsity/prototype/pruner/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/sparsity/prototype/scheduler/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 00:31 torchao/sparsity/prototype/sparsifier/
--rw-r--r--  2.0 unx      843 b- defN 24-May-23 00:31 torchao/sparsity/prototype/__init__.py
--rw-r--r--  2.0 unx     9107 b- defN 24-May-23 00:31 torchao/sparsity/prototype/dynamic_quant_sparse.py
--rw-r--r--  2.0 unx     3388 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/FPGM_pruner.py
--rw-r--r--  2.0 unx      273 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/__init__.py
--rw-r--r--  2.0 unx    10873 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/base_structured_sparsifier.py
--rw-r--r--  2.0 unx     2050 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/lstm_saliency_pruner.py
--rw-r--r--  2.0 unx     1967 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/match_utils.py
--rw-r--r--  2.0 unx     1818 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/parametrization.py
--rw-r--r--  2.0 unx    18992 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/prune_functions.py
--rw-r--r--  2.0 unx     1327 b- defN 24-May-23 00:31 torchao/sparsity/prototype/pruner/saliency_pruner.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/sparsity/prototype/scheduler/__init__.py
--rw-r--r--  2.0 unx     6348 b- defN 24-May-23 00:31 torchao/sparsity/prototype/scheduler/base_scheduler.py
--rw-r--r--  2.0 unx     3873 b- defN 24-May-23 00:31 torchao/sparsity/prototype/scheduler/cubic_scheduler.py
--rw-r--r--  2.0 unx     2018 b- defN 24-May-23 00:31 torchao/sparsity/prototype/scheduler/lambda_scheduler.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 00:31 torchao/sparsity/prototype/sparsifier/__init__.py
--rw-r--r--  2.0 unx    13762 b- defN 24-May-23 00:31 torchao/sparsity/prototype/sparsifier/base_sparsifier.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-23 00:31 torchao/sparsity/prototype/sparsifier/nearly_diagonal_sparsifier.py
--rw-r--r--  2.0 unx     4786 b- defN 24-May-23 00:31 torchao/sparsity/prototype/sparsifier/utils.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-23 00:31 torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py
--rw-r--r--  2.0 unx     1453 b- defN 24-May-23 00:31 torchao_nightly-2024.5.23.dist-info/LICENSE
--rw-r--r--  2.0 unx     7128 b- defN 24-May-23 00:31 torchao_nightly-2024.5.23.dist-info/METADATA
--rw-r--r--  2.0 unx      148 b- defN 24-May-23 00:31 torchao_nightly-2024.5.23.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-23 00:31 torchao_nightly-2024.5.23.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8056 b- defN 24-May-23 00:31 torchao_nightly-2024.5.23.dist-info/RECORD
-108 files, 1378568 bytes uncompressed, 399954 bytes compressed:  71.0%
+Zip file size: 417669 bytes, number of entries: 111
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao_nightly-2024.5.24.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao_nightly.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/csrc/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/dtypes/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/kernel/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/quantization/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/sparsity/
+-rwxr-xr-x  2.0 unx   810656 b- defN 24-May-24 00:50 torchao/_C.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      426 b- defN 24-May-24 00:50 torchao/__init__.py
+-rw-r--r--  2.0 unx     4792 b- defN 24-May-24 00:50 torchao/ops.py
+-rw-r--r--  2.0 unx      860 b- defN 24-May-24 00:50 torchao/utils.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/csrc/cuda/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/csrc/fp6_llm/
+-rw-r--r--  2.0 unx       74 b- defN 24-May-24 00:50 torchao/csrc/init.cpp
+-rw-r--r--  2.0 unx      251 b- defN 24-May-24 00:50 torchao/csrc/nms.cpp
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/csrc/cuda/fp6_llm/
+-rw-r--r--  2.0 unx     5554 b- defN 24-May-24 00:50 torchao/csrc/cuda/nms.cu
+-rw-r--r--  2.0 unx     9437 b- defN 24-May-24 00:50 torchao/csrc/cuda/fp6_llm/fp6_linear.cu
+-rw-r--r--  2.0 unx     9472 b- defN 24-May-24 00:50 torchao/csrc/cuda/fp6_llm/weight_quant.cu
+-rw-r--r--  2.0 unx      479 b- defN 24-May-24 00:50 torchao/csrc/fp6_llm/fp6_llm.cpp
+-rw-r--r--  2.0 unx     9210 b- defN 24-May-24 00:50 torchao/csrc/fp6_llm/weight_prepacking.cpp
+-rw-r--r--  2.0 unx      136 b- defN 24-May-24 00:50 torchao/dtypes/__init__.py
+-rw-r--r--  2.0 unx    33918 b- defN 24-May-24 00:50 torchao/dtypes/nf4tensor.py
+-rw-r--r--  2.0 unx    12448 b- defN 24-May-24 00:50 torchao/dtypes/uint4.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/kernel/__init__.py
+-rw-r--r--  2.0 unx     7389 b- defN 24-May-24 00:50 torchao/kernel/autotuner.py
+-rw-r--r--  2.0 unx     3238 b- defN 24-May-24 00:50 torchao/kernel/intmm.py
+-rw-r--r--  2.0 unx    11678 b- defN 24-May-24 00:50 torchao/kernel/intmm_triton.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/common/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/dora/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/fp8/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/galore/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/hqq/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/prototype/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/prototype/common/__init__.py
+-rw-r--r--  2.0 unx     7071 b- defN 24-May-24 00:50 torchao/prototype/common/profiling_tools.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/dora/kernels/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/prototype/dora/__init__.py
+-rw-r--r--  2.0 unx     6639 b- defN 24-May-24 00:50 torchao/prototype/dora/dora_layer.py
+-rw-r--r--  2.0 unx     3972 b- defN 24-May-24 00:50 torchao/prototype/dora/dora_profile.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/prototype/dora/kernels/__init__.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-24 00:50 torchao/prototype/dora/kernels/common.py
+-rw-r--r--  2.0 unx    15366 b- defN 24-May-24 00:50 torchao/prototype/dora/kernels/custom_autotune.py
+-rw-r--r--  2.0 unx     7641 b- defN 24-May-24 00:50 torchao/prototype/dora/kernels/matmul.py
+-rw-r--r--  2.0 unx    16439 b- defN 24-May-24 00:50 torchao/prototype/dora/kernels/smallk.py
+-rw-r--r--  2.0 unx       38 b- defN 24-May-24 00:50 torchao/prototype/fp8/__init__.py
+-rw-r--r--  2.0 unx     3811 b- defN 24-May-24 00:50 torchao/prototype/fp8/splitk_gemm.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/galore/kernels/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/prototype/galore/optim/
+-rw-r--r--  2.0 unx       23 b- defN 24-May-24 00:50 torchao/prototype/galore/__init__.py
+-rw-r--r--  2.0 unx     3195 b- defN 24-May-24 00:50 torchao/prototype/galore/utils.py
+-rw-r--r--  2.0 unx      210 b- defN 24-May-24 00:50 torchao/prototype/galore/kernels/__init__.py
+-rw-r--r--  2.0 unx    10675 b- defN 24-May-24 00:50 torchao/prototype/galore/kernels/adam_downproj_fused.py
+-rw-r--r--  2.0 unx     4722 b- defN 24-May-24 00:50 torchao/prototype/galore/kernels/adam_step.py
+-rw-r--r--  2.0 unx    15180 b- defN 24-May-24 00:50 torchao/prototype/galore/kernels/custom_autotune.py
+-rw-r--r--  2.0 unx    11641 b- defN 24-May-24 00:50 torchao/prototype/galore/kernels/matmul.py
+-rw-r--r--  2.0 unx     5978 b- defN 24-May-24 00:50 torchao/prototype/galore/kernels/quant.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/prototype/galore/optim/__init__.py
+-rw-r--r--  2.0 unx    15716 b- defN 24-May-24 00:50 torchao/prototype/galore/optim/galore_torch.py
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 00:50 torchao/prototype/hqq/__init__.py
+-rw-r--r--  2.0 unx     7658 b- defN 24-May-24 00:50 torchao/prototype/hqq/hqq_tinygemm_linear.py
+-rw-r--r--  2.0 unx    14227 b- defN 24-May-24 00:50 torchao/prototype/hqq/kernels.py
+-rw-r--r--  2.0 unx     5512 b- defN 24-May-24 00:50 torchao/prototype/hqq/mixed_mm.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/quantization/prototype/
+-rw-r--r--  2.0 unx    50342 b- defN 24-May-24 00:50 torchao/quantization/GPTQ.py
+-rw-r--r--  2.0 unx     1700 b- defN 24-May-24 00:50 torchao/quantization/__init__.py
+-rw-r--r--  2.0 unx    19369 b- defN 24-May-24 00:50 torchao/quantization/autoquant.py
+-rw-r--r--  2.0 unx     2747 b- defN 24-May-24 00:50 torchao/quantization/dynamic_quant.py
+-rw-r--r--  2.0 unx     7110 b- defN 24-May-24 00:50 torchao/quantization/quant_api.py
+-rw-r--r--  2.0 unx    32825 b- defN 24-May-24 00:50 torchao/quantization/quant_primitives.py
+-rw-r--r--  2.0 unx     9159 b- defN 24-May-24 00:50 torchao/quantization/smoothquant.py
+-rw-r--r--  2.0 unx    42347 b- defN 24-May-24 00:50 torchao/quantization/subclass.py
+-rw-r--r--  2.0 unx      754 b- defN 24-May-24 00:50 torchao/quantization/unified.py
+-rw-r--r--  2.0 unx     3236 b- defN 24-May-24 00:50 torchao/quantization/utils.py
+-rw-r--r--  2.0 unx     2742 b- defN 24-May-24 00:50 torchao/quantization/weight_only.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/quantization/prototype/__init__.py
+-rw-r--r--  2.0 unx    12816 b- defN 24-May-24 00:50 torchao/quantization/prototype/qat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/sparsity/prototype/
+-rw-r--r--  2.0 unx      508 b- defN 24-May-24 00:50 torchao/sparsity/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 24-May-24 00:50 torchao/sparsity/sparse_api.py
+-rw-r--r--  2.0 unx     1708 b- defN 24-May-24 00:50 torchao/sparsity/utils.py
+-rw-r--r--  2.0 unx     4156 b- defN 24-May-24 00:50 torchao/sparsity/wanda.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/sparsity/prototype/pruner/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/sparsity/prototype/scheduler/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 00:50 torchao/sparsity/prototype/sparsifier/
+-rw-r--r--  2.0 unx      843 b- defN 24-May-24 00:50 torchao/sparsity/prototype/__init__.py
+-rw-r--r--  2.0 unx     9107 b- defN 24-May-24 00:50 torchao/sparsity/prototype/dynamic_quant_sparse.py
+-rw-r--r--  2.0 unx     3388 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/FPGM_pruner.py
+-rw-r--r--  2.0 unx      273 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/__init__.py
+-rw-r--r--  2.0 unx    10873 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/base_structured_sparsifier.py
+-rw-r--r--  2.0 unx     2050 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/lstm_saliency_pruner.py
+-rw-r--r--  2.0 unx     1967 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/match_utils.py
+-rw-r--r--  2.0 unx     1818 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/parametrization.py
+-rw-r--r--  2.0 unx    18992 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/prune_functions.py
+-rw-r--r--  2.0 unx     1327 b- defN 24-May-24 00:50 torchao/sparsity/prototype/pruner/saliency_pruner.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/sparsity/prototype/scheduler/__init__.py
+-rw-r--r--  2.0 unx     6348 b- defN 24-May-24 00:50 torchao/sparsity/prototype/scheduler/base_scheduler.py
+-rw-r--r--  2.0 unx     3873 b- defN 24-May-24 00:50 torchao/sparsity/prototype/scheduler/cubic_scheduler.py
+-rw-r--r--  2.0 unx     2018 b- defN 24-May-24 00:50 torchao/sparsity/prototype/scheduler/lambda_scheduler.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 00:50 torchao/sparsity/prototype/sparsifier/__init__.py
+-rw-r--r--  2.0 unx    13762 b- defN 24-May-24 00:50 torchao/sparsity/prototype/sparsifier/base_sparsifier.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-24 00:50 torchao/sparsity/prototype/sparsifier/nearly_diagonal_sparsifier.py
+-rw-r--r--  2.0 unx     4786 b- defN 24-May-24 00:50 torchao/sparsity/prototype/sparsifier/utils.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-24 00:50 torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py
+-rw-r--r--  2.0 unx     1453 b- defN 24-May-24 00:50 torchao_nightly-2024.5.24.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7128 b- defN 24-May-24 00:50 torchao_nightly-2024.5.24.dist-info/METADATA
+-rw-r--r--  2.0 unx      148 b- defN 24-May-24 00:50 torchao_nightly-2024.5.24.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-24 00:50 torchao_nightly-2024.5.24.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8239 b- defN 24-May-24 00:50 torchao_nightly-2024.5.24.dist-info/RECORD
+111 files, 1382667 bytes uncompressed, 401327 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: torchao/
 Comment: 
 
-Filename: torchao_nightly-2024.5.23.dist-info/
+Filename: torchao_nightly-2024.5.24.dist-info/
 Comment: 
 
 Filename: torchao_nightly.libs/
 Comment: 
 
 Filename: torchao/csrc/
 Comment: 
@@ -90,14 +90,17 @@
 
 Filename: torchao/prototype/common/
 Comment: 
 
 Filename: torchao/prototype/dora/
 Comment: 
 
+Filename: torchao/prototype/fp8/
+Comment: 
+
 Filename: torchao/prototype/galore/
 Comment: 
 
 Filename: torchao/prototype/hqq/
 Comment: 
 
 Filename: torchao/prototype/__init__.py
@@ -132,14 +135,20 @@
 
 Filename: torchao/prototype/dora/kernels/matmul.py
 Comment: 
 
 Filename: torchao/prototype/dora/kernels/smallk.py
 Comment: 
 
+Filename: torchao/prototype/fp8/__init__.py
+Comment: 
+
+Filename: torchao/prototype/fp8/splitk_gemm.py
+Comment: 
+
 Filename: torchao/prototype/galore/kernels/
 Comment: 
 
 Filename: torchao/prototype/galore/optim/
 Comment: 
 
 Filename: torchao/prototype/galore/__init__.py
@@ -303,23 +312,23 @@
 
 Filename: torchao/sparsity/prototype/sparsifier/utils.py
 Comment: 
 
 Filename: torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py
 Comment: 
 
-Filename: torchao_nightly-2024.5.23.dist-info/LICENSE
+Filename: torchao_nightly-2024.5.24.dist-info/LICENSE
 Comment: 
 
-Filename: torchao_nightly-2024.5.23.dist-info/METADATA
+Filename: torchao_nightly-2024.5.24.dist-info/METADATA
 Comment: 
 
-Filename: torchao_nightly-2024.5.23.dist-info/WHEEL
+Filename: torchao_nightly-2024.5.24.dist-info/WHEEL
 Comment: 
 
-Filename: torchao_nightly-2024.5.23.dist-info/top_level.txt
+Filename: torchao_nightly-2024.5.24.dist-info/top_level.txt
 Comment: 
 
-Filename: torchao_nightly-2024.5.23.dist-info/RECORD
+Filename: torchao_nightly-2024.5.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchao/_C.cpython-39-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --symbols {}

```diff
@@ -352,139 +352,139 @@
    348: 00000000000b56b0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
    349: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
    350: 000000000001f1a0   853 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
    351: 000000000001a700   951 FUNC    GLOBAL DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_
    352: 00000000000b6ec0     0 NOTYPE  GLOBAL DEFAULT   27 _end
    353: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
    354: 000000000001df70    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
-   355: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-   356: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
-   357: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-   358: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
-   359: 00000000000197f0  2955 FUNC    GLOBAL DEFAULT   12 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_
-   360: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
-   361: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
-   362: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED2Ev
-   363: 0000000000026da0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_
-   364: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
-   365: 00000000000b5488   472 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1011SymNodeImplE
-   366: 000000000001e0f0   269 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a
-   367: 000000000001df40    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
-   368: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD2Ev
-   369: 00000000000348c0    29 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1020intrusive_ptr_targetE
-   370: 00000000000155d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   371: 0000000000036190    19 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1010ValueErrorE
-   372: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
-   373: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED2Ev
-   374: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   375: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
-   376: 0000000000037720    47 OBJECT  WEAK   DEFAULT   14 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
-   377: 0000000000026730    56 FUNC    WEAK   DEFAULT   12 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv
-   378: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD2Ev
-   379: 0000000000018410    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   380: 000000000001e250   113 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv
-   381: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
-   382: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
-   383: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
-   384: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD2Ev
-   385: 0000000000015060    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9wrap_boolEb
-   386: 000000000001a380   895 FUNC    GLOBAL DEFAULT   12 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE
-   387: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   388: 0000000000016dc0   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_
-   389: 0000000000022570   482 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
-   390: 0000000000015740    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
-   391: 0000000000014ec0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12constant_intEv
-   392: 0000000000023ee0   183 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_4bitPh
-   393: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED2Ev
-   394: 00000000000150f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9sym_floatEv
-   395: 0000000000021ff0   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_
-   396: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
-   397: 000000000001e090    91 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE
-   398: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
-   399: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
-   400: 0000000000018d20   212 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
-   401: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
-   402: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD2Ev
-   403: 0000000000015210    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   404: 000000000001e2e0   106 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE
-   405: 0000000000016170   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   406: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
-   407: 00000000000153c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5floorEv
-   408: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
-   409: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD2Ev
-   410: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   26 _edata
-   411: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
-   412: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
-   413: 000000000001b1c0   816 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_
-   414: 00000000000b5460    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1020intrusive_ptr_targetE
-   415: 0000000000015b30   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   416: 0000000000015630    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   417: 0000000000017120    37 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD0Ev
-   418: 00000000000b5438    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
-   419: 000000000001deb0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c105Error22what_without_backtraceEv
-   420: 0000000000023d60    17 FUNC    GLOBAL DEFAULT   12 _Z31Extract_4_Bits_From_2_PaddedFP6hh
-   421: 0000000000014ee0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12maybe_as_intEv
-   422: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD2Ev
-   423: 000000000001dee0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9getDeviceEv
-   424: 00000000000b5718    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_S0_E
-   425: 0000000000036530    24 OBJECT  WEAK   DEFAULT   14 _ZTSSt19bad_optional_access
-   426: 00000000000b5910    40 OBJECT  WEAK   DEFAULT   21 _ZTVSt19bad_optional_access
-   427: 0000000000016870   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_
-   428: 0000000000015540    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   429: 0000000000026b30   109 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE9push_backEb
-   430: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
-   431: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
-   432: 0000000000025370   167 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
-   433: 000000000001aac0  1331 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10ScalarTypeES3_EE4callERKS3_S6_S9_
-   434: 00000000000152d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   435: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
-   436: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
-   437: 000000000001f500   917 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_
-   438: 000000000001dfd0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
-   439: 0000000000013990  3958 FUNC    GLOBAL DEFAULT   12 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi
-   440: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
-   441: 000000000001e450    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
-   442: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
-   443: 000000000001b7e0   606 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
-   444: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC2EPS1_
-   445: 0000000000014e90     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_trueEPKcl
-   446: 0000000000016b10   684 FUNC    WEAK   DEFAULT   12 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
-   447: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
-   448: 0000000000015180    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   449: 0000000000022760   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
-   450: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
-   451: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_
-   452: 0000000000015db0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   453: 0000000000015690    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8is_floatEv
-   454: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD1Ev
-   455: 000000000001dfe0    16 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11elapsedTimeEPvS2_a
-   456: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD1Ev
-   457: 0000000000017630   552 FUNC    WEAK   DEFAULT   12 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_
-   458: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
-   459: 0000000000023cc0   126 FUNC    GLOBAL DEFAULT   12 _Z24Padding_8_FP6_To_8_BytesPhS_
-   460: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   461: 0000000000020100   205 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev
-   462: 0000000000022f80  2042 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE
-   463: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   355: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
+   356: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
+   357: 00000000000197f0  2955 FUNC    GLOBAL DEFAULT   12 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_
+   358: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+   359: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
+   360: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED2Ev
+   361: 0000000000026da0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_
+   362: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
+   363: 00000000000b5488   472 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1011SymNodeImplE
+   364: 000000000001e0f0   269 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a
+   365: 000000000001df40    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
+   366: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD2Ev
+   367: 00000000000348c0    29 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1020intrusive_ptr_targetE
+   368: 00000000000155d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   369: 0000000000036190    19 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1010ValueErrorE
+   370: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
+   371: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED2Ev
+   372: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   373: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
+   374: 0000000000037720    47 OBJECT  WEAK   DEFAULT   14 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
+   375: 0000000000026730    56 FUNC    WEAK   DEFAULT   12 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv
+   376: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD2Ev
+   377: 0000000000018410    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   378: 000000000001e250   113 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv
+   379: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
+   380: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
+   381: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
+   382: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD2Ev
+   383: 0000000000015060    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9wrap_boolEb
+   384: 000000000001a380   895 FUNC    GLOBAL DEFAULT   12 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE
+   385: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   386: 0000000000016dc0   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_
+   387: 0000000000022570   482 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
+   388: 0000000000015740    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
+   389: 0000000000014ec0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12constant_intEv
+   390: 0000000000023ee0   183 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_4bitPh
+   391: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED2Ev
+   392: 00000000000150f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9sym_floatEv
+   393: 0000000000021ff0   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_
+   394: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
+   395: 000000000001e090    91 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE
+   396: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
+   397: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
+   398: 0000000000018d20   212 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
+   399: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
+   400: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD2Ev
+   401: 0000000000015210    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   402: 000000000001e2e0   106 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE
+   403: 0000000000016170   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   404: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
+   405: 00000000000153c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5floorEv
+   406: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
+   407: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD2Ev
+   408: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   26 _edata
+   409: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
+   410: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
+   411: 000000000001b1c0   816 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_
+   412: 00000000000b5460    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1020intrusive_ptr_targetE
+   413: 0000000000015b30   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   414: 0000000000015630    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   415: 0000000000017120    37 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD0Ev
+   416: 00000000000b5438    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
+   417: 000000000001deb0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c105Error22what_without_backtraceEv
+   418: 0000000000023d60    17 FUNC    GLOBAL DEFAULT   12 _Z31Extract_4_Bits_From_2_PaddedFP6hh
+   419: 0000000000014ee0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12maybe_as_intEv
+   420: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD2Ev
+   421: 000000000001dee0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9getDeviceEv
+   422: 00000000000b5718    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_S0_E
+   423: 0000000000036530    24 OBJECT  WEAK   DEFAULT   14 _ZTSSt19bad_optional_access
+   424: 00000000000b5910    40 OBJECT  WEAK   DEFAULT   21 _ZTVSt19bad_optional_access
+   425: 0000000000016870   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_
+   426: 0000000000015540    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   427: 0000000000026b30   109 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE9push_backEb
+   428: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
+   429: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
+   430: 0000000000025370   167 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
+   431: 000000000001aac0  1331 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10ScalarTypeES3_EE4callERKS3_S6_S9_
+   432: 00000000000152d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   433: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
+   434: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+   435: 000000000001f500   917 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_
+   436: 000000000001dfd0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
+   437: 0000000000013990  3958 FUNC    GLOBAL DEFAULT   12 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi
+   438: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
+   439: 000000000001e450    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
+   440: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
+   441: 000000000001b7e0   606 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
+   442: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC2EPS1_
+   443: 0000000000014e90     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_trueEPKcl
+   444: 0000000000016b10   684 FUNC    WEAK   DEFAULT   12 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
+   445: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
+   446: 0000000000015180    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   447: 0000000000022760   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
+   448: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d
+   449: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
+   450: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_
+   451: 0000000000015db0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   452: 0000000000015690    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8is_floatEv
+   453: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD1Ev
+   454: 000000000001dfe0    16 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11elapsedTimeEPvS2_a
+   455: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD1Ev
+   456: 0000000000017630   552 FUNC    WEAK   DEFAULT   12 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_
+   457: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
+   458: 0000000000023cc0   126 FUNC    GLOBAL DEFAULT   12 _Z24Padding_8_FP6_To_8_BytesPhS_
+   459: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   460: 0000000000020100   205 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev
+   461: 0000000000022f80  2042 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE
+   462: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   463: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
    464: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
    465: 0000000000018b50   458 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c106IValueESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
    466: 000000000001ed70   223 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl4sizeEl
    467: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
    468: 00000000000b53e0    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1020intrusive_ptr_targetE
    469: 000000000001ee50   561 FUNC    WEAK   DEFAULT   12 _ZNK2at10TensorBase7optionsEv
    470: 0000000000014f00     6 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_symbolicEv
    471: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
    472: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
    473: 0000000000032c5c     0 FUNC    GLOBAL DEFAULT   13 _fini
    474: 0000000000014ed0     5 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13constant_boolEv
    475: 00000000000349e0    25 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_S0_lE
    476: 00000000000361c0    38 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl24DeviceGuardImplInterfaceE
-   477: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-   478: 0000000000014ef0     3 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_constantEv
-   479: 0000000000036220   119 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   477: 0000000000014ef0     3 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_constantEv
+   478: 0000000000036220   119 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   479: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
    480: 00000000000377a0    52 OBJECT  WEAK   DEFAULT   14 _ZTSSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
    481: 000000000001e490    86 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
    482: 0000000000034900    40 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1015VariableVersion14VersionCounterE
    483: 0000000000010000     0 FUNC    GLOBAL DEFAULT    9 _init
    484: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    485: 00000000000169d0   318 FUNC    WEAK   DEFAULT   12 _ZN3c106IValue7destroyEv
    486: 0000000000015330    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
@@ -496,82 +496,82 @@
    492: 00000000000b5750    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
    493: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD2Ev
    494: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
    495: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev
    496: 00000000000b5938    16 OBJECT  WEAK   DEFAULT   21 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
    497: 0000000000034960   123 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
    498: 000000000001def0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9setDeviceENS_6DeviceE
-   499: 000000000001e050    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE
-   500: 0000000000015000    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10guard_boolEPKcl
-   501: 0000000000026520    66 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_
-   502: 00000000000b5790    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl24DeviceGuardImplInterfaceE
-   503: 0000000000017400   123 FUNC    WEAK   DEFAULT   12 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
-   504: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
-   505: 0000000000023d40    28 FUNC    GLOBAL DEFAULT   12 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh
-   506: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_
-   507: 0000000000015270    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_
-   508: 0000000000015030    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9guard_intEPKcl
-   509: 00000000000b57d0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorERKS0_S2_dE
-   510: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
-   511: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
-   512: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   513: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD1Ev
-   514: 000000000001b020    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev
-   515: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   27 __bss_start
-   516: 0000000000017360   155 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_sizeEPKcl
-   517: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
-   518: 00000000000b6ce4     4 OBJECT  UNIQUE DEFAULT   27 _ZZN3c104cuda13warning_stateEvE14warning_state_
-   519: 0000000000023d80   341 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_2bitPh
-   520: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
-   521: 0000000000015510    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   522: 00000000000152a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_notEv
-   523: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
-   524: 000000000001b4f0   751 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
-   525: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
-   526: 000000000001b0a0   101 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_
-   527: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   528: 000000000001dec0     9 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl4typeEv
-   529: 0000000000025230   311 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_
-   530: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   531: 000000000001df90    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl10queryEventEPv
-   532: 000000000001fa40   528 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE
-   533: 0000000000015600    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   534: 000000000001e020    24 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d
-   535: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
-   536: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED2Ev
-   537: 00000000000151b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   538: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED2Ev
-   539: 0000000000013980     5 FUNC    GLOBAL DEFAULT   12 _Z16SplitK_ReductionP6__halfPfmmi
-   540: 000000000002b6b0   478 FUNC    WEAK   DEFAULT   12 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs
-   541: 000000000001e200    68 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
-   542: 000000000001e000     6 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv
-   543: 00000000000b5700    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   544: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
-   545: 00000000000350a0   115 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   546: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
-   547: 00000000000b57e0    48 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1010ValueErrorE
-   548: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   549: 0000000000035070    18 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_E
-   550: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
-   551: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
-   552: 000000000001e3b0    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE
-   553: 00000000000154b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   554: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
-   555: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   556: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
-   557: 00000000000b5408    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1015VariableVersion14VersionCounterE
-   558: 0000000000015390    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3negEv
-   559: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
-   560: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD2Ev
-   561: 0000000000014910  1355 FUNC    GLOBAL DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l
-   562: 000000000001b000    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev
-   563: 000000000001e2d0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
-   564: 00000000000b5810   192 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104cuda4impl13CUDAGuardImplE
-   565: 0000000000014fa0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4int_Ev
-   566: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d
+   499: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+   500: 000000000001e050    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE
+   501: 0000000000015000    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10guard_boolEPKcl
+   502: 0000000000026520    66 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_
+   503: 00000000000b5790    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl24DeviceGuardImplInterfaceE
+   504: 0000000000017400   123 FUNC    WEAK   DEFAULT   12 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
+   505: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
+   506: 0000000000023d40    28 FUNC    GLOBAL DEFAULT   12 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh
+   507: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_
+   508: 0000000000015270    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_
+   509: 0000000000015030    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9guard_intEPKcl
+   510: 00000000000b57d0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorERKS0_S2_dE
+   511: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
+   512: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
+   513: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   514: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD1Ev
+   515: 000000000001b020    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev
+   516: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   27 __bss_start
+   517: 0000000000017360   155 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_sizeEPKcl
+   518: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
+   519: 00000000000b6ce4     4 OBJECT  UNIQUE DEFAULT   27 _ZZN3c104cuda13warning_stateEvE14warning_state_
+   520: 0000000000023d80   341 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_2bitPh
+   521: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
+   522: 0000000000015510    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   523: 00000000000152a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_notEv
+   524: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
+   525: 000000000001b4f0   751 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
+   526: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
+   527: 000000000001b0a0   101 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_
+   528: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   529: 000000000001dec0     9 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl4typeEv
+   530: 0000000000025230   311 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_
+   531: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   532: 000000000001df90    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl10queryEventEPv
+   533: 000000000001fa40   528 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE
+   534: 0000000000015600    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   535: 000000000001e020    24 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d
+   536: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
+   537: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED2Ev
+   538: 00000000000151b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   539: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED2Ev
+   540: 0000000000013980     5 FUNC    GLOBAL DEFAULT   12 _Z16SplitK_ReductionP6__halfPfmmi
+   541: 000000000002b6b0   478 FUNC    WEAK   DEFAULT   12 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs
+   542: 000000000001e200    68 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
+   543: 000000000001e000     6 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv
+   544: 00000000000b5700    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   545: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
+   546: 00000000000350a0   115 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   547: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
+   548: 00000000000b57e0    48 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1010ValueErrorE
+   549: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   550: 0000000000035070    18 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_E
+   551: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
+   552: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
+   553: 000000000001e3b0    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE
+   554: 00000000000154b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   555: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
+   556: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   557: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
+   558: 00000000000b5408    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1015VariableVersion14VersionCounterE
+   559: 0000000000015390    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3negEv
+   560: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
+   561: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD2Ev
+   562: 0000000000014910  1355 FUNC    GLOBAL DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l
+   563: 000000000001b000    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev
+   564: 000000000001e2d0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
+   565: 00000000000b5810   192 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104cuda4impl13CUDAGuardImplE
+   566: 0000000000014fa0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4int_Ev
    567: 0000000000015720    29 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
    568: 000000000001df00    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl18uncheckedSetDeviceENS_6DeviceE
    569: 0000000000017540   237 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l
    570: 0000000000013890   228 FUNC    GLOBAL DEFAULT   12 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi
    571: 000000000001f8a0   193 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv
    572: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
    573: 0000000000018e00  1012 FUNC    WEAK   DEFAULT   12 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE
@@ -605,15 +605,15 @@
    601: 00000000000157b0    70 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
    602: 00000000000b5778    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1010ValueErrorE
    603: 0000000000014e70     3 FUNC    WEAK   DEFAULT   12 _ZNK3c1011SymNodeImpl13is_nested_intEv
 
 Symbol table '.symtab' contains 840 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000875_00000000-6_fp6_linear.compute_86.cudafe1.cpp
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_000009f7_00000000-6_fp6_linear.compute_86.cudafe1.cpp
      2: 0000000000037988     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
      3: 00000000000133d0   568 FUNC    LOCAL  DEFAULT   12 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmi
      4: 00000000000b6aa0     8 OBJECT  LOCAL  DEFAULT   27 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
      5: 00000000000b6aa8     8 OBJECT  LOCAL  DEFAULT   27 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
      6: 0000000000013610    12 FUNC    LOCAL  DEFAULT   12 _ZL26__cudaUnregisterBinaryUtilv
      7: 00000000000b6b20     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
      8: 0000000000013620   549 FUNC    LOCAL  DEFAULT   12 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmi.constprop.0
@@ -633,49 +633,49 @@
     22: 00000000000b6b10     8 OBJECT  LOCAL  DEFAULT   27 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
     23: 00000000000b6b18     8 OBJECT  LOCAL  DEFAULT   27 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
     24: 0000000000011d80   502 FUNC    LOCAL  DEFAULT   12 _ZL24__sti____cudaRegisterAllv
     25: 00000000000b6a38    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     26: 0000000000034a00     1 OBJECT  LOCAL  DEFAULT   14 _ZN6thrust6system6detail10sequentialL3seqE
     27: 0000000000034a08     8 OBJECT  LOCAL  DEFAULT   14 _ZN3c10L45autograd_dispatch_keyset_with_ADInplaceOrViewE
     28: 00000000000113a0    24 FUNC    LOCAL  DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l.cold
-    29: 0000000000011f80   408 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp
+    29: 0000000000011f80   408 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp
     30: 00000000000b6ba0     1 OBJECT  LOCAL  DEFAULT   27 _ZStL8__ioinit
     31: 00000000000b6b40    96 OBJECT  LOCAL  DEFAULT   27 _ZN7torchaoL45TORCH_LIBRARY_IMPL_static_init_torchao_CUDA_2E
-    32: 00000000000113b8    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
-    33: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000876_00000000-6_weight_quant.compute_86.cudafe1.cpp
+    32: 00000000000113b8    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
+    33: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_000009f8_00000000-6_weight_quant.compute_86.cudafe1.cpp
     34: 000000000009d658     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
     35: 0000000000019550    12 FUNC    LOCAL  DEFAULT   12 _ZL26__cudaUnregisterBinaryUtilv
     36: 00000000000b6bc0     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
     37: 0000000000019560    50 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
     38: 0000000000011405    69 FUNC    LOCAL  DEFAULT   12 _Z13cast_fp16_fp6PtPh.cold
     39: 000000000001144a    69 FUNC    LOCAL  DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm.cold
     40: 0000000000012120    91 FUNC    LOCAL  DEFAULT   12 _ZL24__sti____cudaRegisterAllv
     41: 00000000000b6a50    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     42: 0000000000035135     1 OBJECT  LOCAL  DEFAULT   14 _ZN6thrust6system6detail10sequentialL3seqE
     43: 000000000001148f    16 FUNC    LOCAL  DEFAULT   12 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE.cold
     44: 000000000001149f    16 FUNC    LOCAL  DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_.cold
-    45: 0000000000012180   919 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp
+    45: 0000000000012180   919 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp
     46: 00000000000b6c40     1 OBJECT  LOCAL  DEFAULT   27 _ZStL8__ioinit
     47: 00000000000b6be0    96 OBJECT  LOCAL  DEFAULT   27 _ZN7torchaoL44TORCH_LIBRARY_IMPL_static_init_torchao_CPU_2E
-    48: 00000000000114af   119 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
-    49: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000877_00000000-6_nms.compute_86.cudafe1.cpp
+    48: 00000000000114af   119 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
+    49: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_000009f9_00000000-6_nms.compute_86.cudafe1.cpp
     50: 000000000009de68     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
     51: 000000000001ba40   624 FUNC    LOCAL  DEFAULT   12 _ZN3c10L8toStringENS_10ScalarTypeE
     52: 000000000001bcb0    12 FUNC    LOCAL  DEFAULT   12 _ZL26__cudaUnregisterBinaryUtilv
     53: 00000000000b6c60     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
     54: 000000000001bcc0    50 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
     55: 0000000000012520   226 FUNC    LOCAL  DEFAULT   12 _ZL24__sti____cudaRegisterAllv
     56: 00000000000b6a68    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     57: 00000000000352c4     1 OBJECT  LOCAL  DEFAULT   14 _ZN6thrust6system6detail10sequentialL3seqE
     58: 000000000001bd00   460 FUNC    LOCAL  DEFAULT   12 _ZN3c106SymInt8release_Ev.part.0
-    59: 0000000000011526   949 FUNC    LOCAL  DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d.cold
-    60: 0000000000012610   445 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp
+    59: 0000000000011526   949 FUNC    LOCAL  DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d.cold
+    60: 0000000000012610   445 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp
     61: 00000000000b6ce0     1 OBJECT  LOCAL  DEFAULT   27 _ZStL8__ioinit
     62: 00000000000b6c80    96 OBJECT  LOCAL  DEFAULT   27 _ZN7torchaoL45TORCH_LIBRARY_IMPL_static_init_torchao_CUDA_2E
-    63: 00000000000118db    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold
+    63: 00000000000118db    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold
     64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS fp6_llm.cpp
     65: 0000000000011928    39 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
     66: 00000000000127d0  1768 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_fp6_llm.cpp
     67: 00000000000b6d00    96 OBJECT  LOCAL  DEFAULT   27 _ZL44TORCH_LIBRARY_FRAGMENT_static_init_torchao_2
     68: 000000000001194f   238 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_fp6_llm.cpp.cold
     69: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS weight_prepacking.cpp
     70: 0000000000011a3e    39 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
@@ -874,33 +874,33 @@
    263: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9exceptionD2Ev@GLIBCXX_3.4
    264: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
    265: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyByteArray_Type
    266: 0000000000015540    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    267: 00000000000164f0   896 FUNC    WEAK   DEFAULT   12 _ZNK3c106IValue7tagKindEv
    268: 000000000001df10    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9getStreamENS_6DeviceE
    269: 0000000000032c5c     0 FUNC    GLOBAL DEFAULT   13 _fini
-   270: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
-   271: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
-   272: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   273: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttrString
-   274: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
-   275: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_IsSubtype
-   276: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memmove@GLIBC_2.2.5
-   277: 00000000000157b0    70 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
-   278: 0000000000022760   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
-   279: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZN3c1019UndefinedTensorImpl10_singletonE
-   280: 0000000000022f80  2042 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE
-   281: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Fetch
-   282: 000000000001b110   165 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_
-   283: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyException_SetTraceback
-   284: 0000000000014ec0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12constant_intEv
-   285: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __assert_fail@GLIBC_2.2.5
-   286: 0000000000015150    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl28is_non_overlapping_and_denseENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   287: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_RuntimeError
-   288: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
+   270: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+   271: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
+   272: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
+   273: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   274: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttrString
+   275: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
+   276: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_IsSubtype
+   277: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memmove@GLIBC_2.2.5
+   278: 00000000000157b0    70 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
+   279: 0000000000022760   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
+   280: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZN3c1019UndefinedTensorImpl10_singletonE
+   281: 0000000000022f80  2042 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE
+   282: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Fetch
+   283: 000000000001b110   165 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_
+   284: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyException_SetTraceback
+   285: 0000000000014ec0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12constant_intEv
+   286: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __assert_fail@GLIBC_2.2.5
+   287: 0000000000015150    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl28is_non_overlapping_and_denseENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   288: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_RuntimeError
    289: 0000000000015060    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9wrap_boolEb
    290: 00000000000154b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    291: 0000000000016b10   684 FUNC    WEAK   DEFAULT   12 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
    292: 000000000001e0f0   269 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a
    293: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_Copy
    294: 0000000000026b30   109 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE9push_backEb
    295: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyThreadState_UncheckedGet
@@ -957,205 +957,205 @@
    346: 00000000000195a0   405 FUNC    GLOBAL DEFAULT   12 _Z13cast_fp16_fp6PtPh
    347: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
    348: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3
    349: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_HasAttrString
    350: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt9bad_alloc@GLIBCXX_3.4
    351: 0000000000015b30   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
    352: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_guard_abort@CXXABI_1.3
-   353: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamQuery@libcudart.so.12
-   354: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.12
-   355: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c1010TensorType3getEv
-   356: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
-   357: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE
-   358: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda14ExchangeDeviceEa
-   359: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE
-   360: 00000000000b53e0    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1020intrusive_ptr_targetE
-   361: 000000000001deb0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c105Error22what_without_backtraceEv
-   362: 00000000000b57d0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorERKS0_S2_dE
-   363: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorD2Ev@GLIBCXX_3.4
-   364: 0000000000017630   552 FUNC    WEAK   DEFAULT   12 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_
-   365: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3
-   366: 00000000000152a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_notEv
-   367: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops9to_device4callERKNS_6TensorEN3c106DeviceENS5_10ScalarTypeEbbSt8optionalINS5_12MemoryFormatEE
-   368: 0000000000034900    40 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1015VariableVersion14VersionCounterE
-   369: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_AsString
-   370: 0000000000026730    56 FUNC    WEAK   DEFAULT   12 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv
-   371: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs12_M_leak_hardEv@GLIBCXX_3.4
-   372: 00000000000b5718    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_S0_E
-   373: 0000000000015270    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_
-   374: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_S2_
-   375: 0000000000015690    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8is_floatEv
-   376: 0000000000015db0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   377: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSo9_M_insertImEERSoT_@GLIBCXX_3.4.9
-   378: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt11_Hash_bytesPKvmm@CXXABI_1.3.5
-   379: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs5rfindEPKcmm@GLIBCXX_3.4
-   380: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs17find_first_not_ofEPKcmm@GLIBCXX_3.4
-   381: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyByteArray_Size
-   382: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD1Ev
-   383: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZdlPv@GLIBCXX_3.4
-   384: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
-   385: 000000000001df20    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12getNewStreamENS_6DeviceEi
-   386: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1EPKcmRKSaIcE@GLIBCXX_3.4
-   387: 0000000000014ee0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12maybe_as_intEv
-   388: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
-   389: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_GetContext
-   390: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE
-   391: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
-   392: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
-   393: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE
-   394: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
-   395: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
-   396: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendEPKcm@GLIBCXX_3.4
-   397: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
-   398: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4swapERSs@GLIBCXX_3.4
-   399: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
-   400: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyType_Lookup
-   401: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Clear
-   402: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Clear
-   403: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
-   404: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_throw@CXXABI_1.3
-   405: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamSynchronize@libcudart.so.12
-   406: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
-   407: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_New
-   408: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Calloc
-   409: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
-   410: 000000000001f1a0   853 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
-   411: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb
-   412: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc@GLIBCXX_3.4
-   413: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch7LibraryC1ENS0_4KindESsSt8optionalIN3c1011DispatchKeyEEPKcj
-   414: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Unwind_Resume@GCC_3.0
-   415: 00000000000223b0   441 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11queryStreamERKNS_6StreamE
-   416: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_Size
-   417: 00000000000350a0   115 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   418: 0000000000014eb0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl16nested_int_coeffEv
-   419: 000000000001e250   113 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv
-   420: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda12device_countEv
-   421: 000000000001f8a0   193 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv
-   422: 0000000000023d80   341 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_2bitPh
-   423: 000000000001a700   951 FUNC    GLOBAL DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_
-   424: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND vsnprintf@GLIBC_2.2.5
-   425: 000000000001b0a0   101 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_
-   426: 0000000000017030    37 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD0Ev
-   427: 0000000000015330    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   428: 00000000000b5450    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_S0_S0_lE
-   429: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_TypeError
-   430: 00000000000153c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5floorEv
-   431: 00000000000b57a0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104cuda4impl13CUDAGuardImplE
-   432: 000000000001df00    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl18uncheckedSetDeviceENS_6DeviceE
-   433: 000000000001e090    91 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE
-   434: 00000000000b5488   472 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1011SymNodeImplE
-   435: 00000000000b5778    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1010ValueErrorE
-   436: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   437: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_Ready
-   438: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
-   439: 0000000000035000   109 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   440: 0000000000015420    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   441: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c105ErrorC2ENS_14SourceLocationESs
-   442: 00000000000b53f0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1011SymNodeImplE
-   443: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt24__throw_out_of_range_fmtPKcz
-   444: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   445: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
-   446: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   447: 0000000000017120    37 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD0Ev
-   448: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignERKSs@GLIBCXX_3.4
-   449: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignEPKcm@GLIBCXX_3.4
-   450: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   451: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   452: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_RKSs
-   453: 00000000000255a0   291 FUNC    GLOBAL DEFAULT   12 PyInit__C
-   454: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendERKSs@GLIBCXX_3.4
-   455: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
-   456: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_GetItem
-   457: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptrneERKNS_13exception_ptrES2_@CXXABI_1.3.3
-   458: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
-   459: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
-   460: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at6Tensor5indexESt16initializer_listINS_8indexing11TensorIndexEE
-   461: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5
-   462: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
-   463: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIlEEPT_v
-   464: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_SetItem
-   465: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   466: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_get
-   467: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Restore
-   468: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
-   469: 0000000000018a30   275 FUNC    WEAK   DEFAULT   12 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
-   470: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD1Ev
-   471: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD1Ev
-   472: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_pure_virtual@CXXABI_1.3
-   473: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __pthread_key_create@GLIBC_2.2.5
-   474: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptr4swapERS0_@CXXABI_1.3.3
-   475: 0000000000015090    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10wrap_floatEd
-   476: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
-   477: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNR5torch7Library5_implEPKcONS_11CppFunctionENS_17_RegisterOrVerifyE
-   478: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
-   479: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSaIcE@GLIBCXX_3.4
-   480: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda9GetDeviceEPa
-   481: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
-   482: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4
-   483: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptrD1Ev@CXXABI_1.3.3
-   484: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops12index_select4callERKNS_6TensorElS4_
-   485: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_alloc
-   486: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt16nested_exception@CXXABI_1.3.5
-   487: 0000000000015450    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2leERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   488: 000000000001ded0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeDeviceENS_6DeviceE
-   489: 000000000001df30    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16getDefaultStreamENS_6DeviceE
-   490: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN6caffe28TypeMeta26error_unsupported_typemetaES0_
-   491: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
-   492: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt13runtime_error@GLIBCXX_3.4
-   493: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
-   494: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaGetErrorString@libcudart.so.12
-   495: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC1ERKSs@GLIBCXX_3.4
-   496: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_
-   497: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   498: 0000000000018570  1207 FUNC    WEAK   DEFAULT   12 _ZN5torch8autograd13make_variableEN2at6TensorEbb
-   499: 000000000001f110   139 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED0Ev
-   500: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
-   501: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
-   502: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
-   503: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
-   504: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
-   505: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9
-   506: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   507: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
-   508: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
-   509: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSsmm@GLIBCXX_3.4
-   510: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_GetThisThreadState
-   511: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_AsStringAndSize
-   512: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcmp@GLIBC_2.2.5
-   513: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
-   514: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsEncodedString
-   515: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs7compareEPKc@GLIBCXX_3.4
-   516: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIN3c104HalfEEEPT_v
-   517: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD2Ev
-   518: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
-   519: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
-   520: 0000000000015ef0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   521: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
-   522: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallFunctionObjArgs
-   523: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104impl23ExcludeDispatchKeyGuardC1ENS_14DispatchKeySetE
-   524: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIhEEPT_v
-   525: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
-   526: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
-   527: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventSynchronize@libcudart.so.12
-   528: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20getDefaultCUDAStreamEa
-   529: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
-   530: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
-   531: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
-   532: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c10lsERSoNS_10DeviceTypeE
-   533: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
-   534: 000000000001f970   195 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeDeviceENS_6DeviceE
-   535: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
-   536: 000000000002b580   294 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm
-   537: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
-   538: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   539: 0000000000014e70     3 FUNC    WEAK   DEFAULT   12 _ZNK3c1011SymNodeImpl13is_nested_intEv
-   540: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev
-   541: 00000000000b56d8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   542: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
-   543: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
+   353: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+   354: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamQuery@libcudart.so.12
+   355: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.12
+   356: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c1010TensorType3getEv
+   357: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
+   358: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE
+   359: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda14ExchangeDeviceEa
+   360: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE
+   361: 00000000000b53e0    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1020intrusive_ptr_targetE
+   362: 000000000001deb0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c105Error22what_without_backtraceEv
+   363: 00000000000b57d0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorERKS0_S2_dE
+   364: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorD2Ev@GLIBCXX_3.4
+   365: 0000000000017630   552 FUNC    WEAK   DEFAULT   12 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_
+   366: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3
+   367: 00000000000152a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_notEv
+   368: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops9to_device4callERKNS_6TensorEN3c106DeviceENS5_10ScalarTypeEbbSt8optionalINS5_12MemoryFormatEE
+   369: 0000000000034900    40 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1015VariableVersion14VersionCounterE
+   370: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_AsString
+   371: 0000000000026730    56 FUNC    WEAK   DEFAULT   12 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv
+   372: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs12_M_leak_hardEv@GLIBCXX_3.4
+   373: 00000000000b5718    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_S0_E
+   374: 0000000000015270    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_
+   375: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_S2_
+   376: 0000000000015690    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8is_floatEv
+   377: 0000000000015db0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   378: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSo9_M_insertImEERSoT_@GLIBCXX_3.4.9
+   379: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt11_Hash_bytesPKvmm@CXXABI_1.3.5
+   380: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs5rfindEPKcmm@GLIBCXX_3.4
+   381: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs17find_first_not_ofEPKcmm@GLIBCXX_3.4
+   382: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyByteArray_Size
+   383: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD1Ev
+   384: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZdlPv@GLIBCXX_3.4
+   385: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
+   386: 000000000001df20    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12getNewStreamENS_6DeviceEi
+   387: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1EPKcmRKSaIcE@GLIBCXX_3.4
+   388: 0000000000014ee0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12maybe_as_intEv
+   389: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
+   390: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_GetContext
+   391: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE
+   392: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
+   393: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
+   394: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE
+   395: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
+   396: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
+   397: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendEPKcm@GLIBCXX_3.4
+   398: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
+   399: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4swapERSs@GLIBCXX_3.4
+   400: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
+   401: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyType_Lookup
+   402: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Clear
+   403: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Clear
+   404: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
+   405: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_throw@CXXABI_1.3
+   406: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamSynchronize@libcudart.so.12
+   407: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
+   408: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_New
+   409: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Calloc
+   410: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
+   411: 000000000001f1a0   853 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
+   412: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb
+   413: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc@GLIBCXX_3.4
+   414: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch7LibraryC1ENS0_4KindESsSt8optionalIN3c1011DispatchKeyEEPKcj
+   415: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Unwind_Resume@GCC_3.0
+   416: 00000000000223b0   441 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11queryStreamERKNS_6StreamE
+   417: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_Size
+   418: 00000000000350a0   115 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   419: 0000000000014eb0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl16nested_int_coeffEv
+   420: 000000000001e250   113 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv
+   421: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda12device_countEv
+   422: 000000000001f8a0   193 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv
+   423: 0000000000023d80   341 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_2bitPh
+   424: 000000000001a700   951 FUNC    GLOBAL DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_
+   425: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND vsnprintf@GLIBC_2.2.5
+   426: 000000000001b0a0   101 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_
+   427: 0000000000017030    37 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD0Ev
+   428: 0000000000015330    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   429: 00000000000b5450    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_S0_S0_lE
+   430: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_TypeError
+   431: 00000000000153c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5floorEv
+   432: 00000000000b57a0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104cuda4impl13CUDAGuardImplE
+   433: 000000000001df00    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl18uncheckedSetDeviceENS_6DeviceE
+   434: 000000000001e090    91 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE
+   435: 00000000000b5488   472 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1011SymNodeImplE
+   436: 00000000000b5778    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1010ValueErrorE
+   437: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   438: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_Ready
+   439: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
+   440: 0000000000035000   109 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   441: 0000000000015420    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   442: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c105ErrorC2ENS_14SourceLocationESs
+   443: 00000000000b53f0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1011SymNodeImplE
+   444: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt24__throw_out_of_range_fmtPKcz
+   445: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   446: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
+   447: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   448: 0000000000017120    37 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD0Ev
+   449: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignERKSs@GLIBCXX_3.4
+   450: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignEPKcm@GLIBCXX_3.4
+   451: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   452: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   453: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_RKSs
+   454: 00000000000255a0   291 FUNC    GLOBAL DEFAULT   12 PyInit__C
+   455: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendERKSs@GLIBCXX_3.4
+   456: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
+   457: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_GetItem
+   458: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptrneERKNS_13exception_ptrES2_@CXXABI_1.3.3
+   459: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
+   460: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
+   461: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at6Tensor5indexESt16initializer_listINS_8indexing11TensorIndexEE
+   462: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5
+   463: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
+   464: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIlEEPT_v
+   465: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_SetItem
+   466: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   467: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_get
+   468: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Restore
+   469: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
+   470: 0000000000018a30   275 FUNC    WEAK   DEFAULT   12 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
+   471: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD1Ev
+   472: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD1Ev
+   473: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_pure_virtual@CXXABI_1.3
+   474: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __pthread_key_create@GLIBC_2.2.5
+   475: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptr4swapERS0_@CXXABI_1.3.3
+   476: 0000000000015090    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10wrap_floatEd
+   477: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
+   478: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNR5torch7Library5_implEPKcONS_11CppFunctionENS_17_RegisterOrVerifyE
+   479: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
+   480: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSaIcE@GLIBCXX_3.4
+   481: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda9GetDeviceEPa
+   482: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
+   483: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4
+   484: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptrD1Ev@CXXABI_1.3.3
+   485: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops12index_select4callERKNS_6TensorElS4_
+   486: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_alloc
+   487: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt16nested_exception@CXXABI_1.3.5
+   488: 0000000000015450    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2leERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   489: 000000000001ded0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeDeviceENS_6DeviceE
+   490: 000000000001df30    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16getDefaultStreamENS_6DeviceE
+   491: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN6caffe28TypeMeta26error_unsupported_typemetaES0_
+   492: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
+   493: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt13runtime_error@GLIBCXX_3.4
+   494: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
+   495: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaGetErrorString@libcudart.so.12
+   496: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC1ERKSs@GLIBCXX_3.4
+   497: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_
+   498: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   499: 0000000000018570  1207 FUNC    WEAK   DEFAULT   12 _ZN5torch8autograd13make_variableEN2at6TensorEbb
+   500: 000000000001f110   139 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED0Ev
+   501: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
+   502: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
+   503: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
+   504: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
+   505: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
+   506: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9
+   507: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+   508: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
+   509: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
+   510: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSsmm@GLIBCXX_3.4
+   511: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_GetThisThreadState
+   512: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_AsStringAndSize
+   513: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcmp@GLIBC_2.2.5
+   514: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
+   515: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsEncodedString
+   516: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs7compareEPKc@GLIBCXX_3.4
+   517: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIN3c104HalfEEEPT_v
+   518: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD2Ev
+   519: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
+   520: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
+   521: 0000000000015ef0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   522: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
+   523: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallFunctionObjArgs
+   524: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104impl23ExcludeDispatchKeyGuardC1ENS_14DispatchKeySetE
+   525: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIhEEPT_v
+   526: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
+   527: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
+   528: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventSynchronize@libcudart.so.12
+   529: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20getDefaultCUDAStreamEa
+   530: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
+   531: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
+   532: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
+   533: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c10lsERSoNS_10DeviceTypeE
+   534: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
+   535: 000000000001f970   195 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeDeviceENS_6DeviceE
+   536: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
+   537: 000000000002b580   294 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm
+   538: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
+   539: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   540: 0000000000014e70     3 FUNC    WEAK   DEFAULT   12 _ZNK3c1011SymNodeImpl13is_nested_intEv
+   541: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev
+   542: 00000000000b56d8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   543: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
    544: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_DeleteCurrent
    545: 00000000000172b0   162 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
    546: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIiEEPT_v
    547: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
    548: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
    549: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventRecord@libcudart.so.12
    550: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
@@ -1297,80 +1297,80 @@
    686: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@GLIBCXX_3.4
    687: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c107WarningC1ESt7variantIJNS0_11UserWarningENS0_18DeprecationWarningEEERKNS_14SourceLocationESsb
    688: 000000000001e3b0    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE
    689: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinaryEnd@libcudart.so.12
    690: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyInstanceMethod_New
    691: 0000000000014ef0     3 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_constantEv
    692: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __gxx_personality_v0@CXXABI_1.3
-   693: 000000000001dec0     9 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl4typeEv
-   694: 00000000000150c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8wrap_intEl
-   695: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD1Ev
-   696: 000000000001b4f0   751 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
-   697: 000000000001e350    33 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi
-   698: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_New
-   699: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD2Ev
-   700: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_SetPointer
-   701: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4
-   702: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD1Ev
-   703: 00000000000169d0   318 FUNC    WEAK   DEFAULT   12 _ZN3c106IValue7destroyEv
-   704: 0000000000015630    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   705: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_Release
-   706: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
-   707: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventElapsedTime@libcudart.so.12
-   708: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSspLEPKc@GLIBCXX_3.4
-   709: 00000000000153f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4ceilEv
-   710: 00000000000b5750    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   711: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NotImplementedStruct
-   712: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_baseD2Ev@GLIBCXX_3.4
-   713: 000000000001df70    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
-   714: 0000000000014e90     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_trueEPKcl
-   715: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6insertEmPKcm@GLIBCXX_3.4
-   716: 0000000000023d40    28 FUNC    GLOBAL DEFAULT   12 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh
-   717: 00000000000197f0  2955 FUNC    GLOBAL DEFAULT   12 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_
-   718: 0000000000017360   155 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_sizeEPKcl
-   719: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIfEEPT_v
-   720: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED2Ev
-   721: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops10empty_like4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbES5_INS6_12MemoryFormatEE
-   722: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4_Rep9_S_createEmmRKSaIcE@GLIBCXX_3.4
-   723: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetItem
-   724: 000000000001e200    68 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
-   725: 00000000000b57b8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
-   726: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_SystemError
-   727: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD2Ev
-   728: 0000000000018d20   212 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
-   729: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt6localeC1Ev@GLIBCXX_3.4
-   730: 0000000000025230   311 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_
-   731: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED1Ev
-   732: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c10neERKNS_6SymIntEi
-   733: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_
-   734: 0000000000015390    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3negEv
-   735: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_Type
-   736: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_end_catch@CXXABI_1.3
-   737: 000000000001e450    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
-   738: 0000000000010000     0 FUNC    GLOBAL DEFAULT    9 _init
-   739: 0000000000023d60    17 FUNC    GLOBAL DEFAULT   12 _Z31Extract_4_Bits_From_2_PaddedFP6hh
-   740: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD2Ev
-   741: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@GLIBC_2.2.5
-   742: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda9SetDeviceEa
-   743: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_rethrow@CXXABI_1.3
-   744: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD2Ev
-   745: 0000000000023fa0   765 FUNC    GLOBAL DEFAULT   12 _Z25Assign_32_FP6_To_4_ThreadPSt6vectorIhSaIhEES2_PhS3_S3_S3_
-   746: 0000000000026da0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_
-   747: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorD1Ev@GLIBCXX_3.4
-   748: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs4findEPKcmm@GLIBCXX_3.4
-   749: 0000000000018e00  1012 FUNC    WEAK   DEFAULT   12 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE
-   750: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@libcudart.so.12
-   751: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev
-   752: 0000000000036200    32 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104cuda4impl13CUDAGuardImplE
-   753: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD2Ev
-   754: 0000000000025370   167 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
-   755: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c107IntType3getEv
-   756: 0000000000015510    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   757: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_GetBack
-   758: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d
+   693: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d
+   694: 000000000001dec0     9 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl4typeEv
+   695: 00000000000150c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8wrap_intEl
+   696: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD1Ev
+   697: 000000000001b4f0   751 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
+   698: 000000000001e350    33 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi
+   699: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_New
+   700: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD2Ev
+   701: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_SetPointer
+   702: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4
+   703: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD1Ev
+   704: 00000000000169d0   318 FUNC    WEAK   DEFAULT   12 _ZN3c106IValue7destroyEv
+   705: 0000000000015630    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   706: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_Release
+   707: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
+   708: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventElapsedTime@libcudart.so.12
+   709: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSspLEPKc@GLIBCXX_3.4
+   710: 00000000000153f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4ceilEv
+   711: 00000000000b5750    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   712: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NotImplementedStruct
+   713: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt8ios_baseD2Ev@GLIBCXX_3.4
+   714: 000000000001df70    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
+   715: 0000000000014e90     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_trueEPKcl
+   716: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6insertEmPKcm@GLIBCXX_3.4
+   717: 0000000000023d40    28 FUNC    GLOBAL DEFAULT   12 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh
+   718: 00000000000197f0  2955 FUNC    GLOBAL DEFAULT   12 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_
+   719: 0000000000017360   155 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_sizeEPKcl
+   720: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIfEEPT_v
+   721: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED2Ev
+   722: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops10empty_like4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbES5_INS6_12MemoryFormatEE
+   723: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4_Rep9_S_createEmmRKSaIcE@GLIBCXX_3.4
+   724: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetItem
+   725: 000000000001e200    68 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
+   726: 00000000000b57b8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   727: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_SystemError
+   728: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD2Ev
+   729: 0000000000018d20   212 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
+   730: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt6localeC1Ev@GLIBCXX_3.4
+   731: 0000000000025230   311 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_
+   732: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED1Ev
+   733: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c10neERKNS_6SymIntEi
+   734: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_
+   735: 0000000000015390    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3negEv
+   736: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_Type
+   737: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_end_catch@CXXABI_1.3
+   738: 000000000001e450    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
+   739: 0000000000010000     0 FUNC    GLOBAL DEFAULT    9 _init
+   740: 0000000000023d60    17 FUNC    GLOBAL DEFAULT   12 _Z31Extract_4_Bits_From_2_PaddedFP6hh
+   741: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD2Ev
+   742: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@GLIBC_2.2.5
+   743: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda9SetDeviceEa
+   744: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_rethrow@CXXABI_1.3
+   745: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD2Ev
+   746: 0000000000023fa0   765 FUNC    GLOBAL DEFAULT   12 _Z25Assign_32_FP6_To_4_ThreadPSt6vectorIhSaIhEES2_PhS3_S3_S3_
+   747: 0000000000026da0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_
+   748: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorD1Ev@GLIBCXX_3.4
+   749: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs4findEPKcmm@GLIBCXX_3.4
+   750: 0000000000018e00  1012 FUNC    WEAK   DEFAULT   12 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE
+   751: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFunction@libcudart.so.12
+   752: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev
+   753: 0000000000036200    32 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104cuda4impl13CUDAGuardImplE
+   754: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD2Ev
+   755: 0000000000025370   167 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
+   756: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c107IntType3getEv
+   757: 0000000000015510    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   758: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_GetBack
    759: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPopCallConfiguration@libcudart.so.12
    760: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_IndexError
    761: 0000000000015660    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    762: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3
    763: 0000000000017540   237 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l
    764: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_free_exception@CXXABI_1.3
    765: 0000000000025200    37 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD0Ev
@@ -1420,31 +1420,31 @@
    809: 000000000001df60    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11deviceCountEv
    810: 000000000001b1c0   816 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_
    811: 0000000000014910  1355 FUNC    GLOBAL DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l
    812: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC2EPS1_
    813: 00000000000150f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9sym_floatEv
    814: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Str
    815: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c109FloatType3getEv
-   816: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-   817: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_GetItemWithError
-   818: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
-   819: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Format
-   820: 0000000000017150   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKSsEE4callERKS3_S5_
-   821: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
-   822: 00000000000348c0    29 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1020intrusive_ptr_targetE
-   823: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104impl23ExcludeDispatchKeyGuardD1Ev
-   824: 0000000000015030    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9guard_intEPKcl
-   825: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c106SymInt9guard_intEPKcl
-   826: 0000000000020930  1085 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE
-   827: 0000000000018410    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   828: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTIN3c105ErrorE
-   829: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt9terminatev@GLIBCXX_3.4
-   830: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsUTF8AndSize
-   831: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Size
-   832: 000000000001e3d0   123 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl11size_customEl
-   833: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD2Ev
+   816: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_GetItemWithError
+   817: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
+   818: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Format
+   819: 0000000000017150   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKSsEE4callERKS3_S5_
+   820: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
+   821: 00000000000348c0    29 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1020intrusive_ptr_targetE
+   822: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104impl23ExcludeDispatchKeyGuardD1Ev
+   823: 0000000000015030    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9guard_intEPKcl
+   824: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c106SymInt9guard_intEPKcl
+   825: 0000000000020930  1085 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE
+   826: 0000000000018410    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   827: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTIN3c105ErrorE
+   828: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt9terminatev@GLIBCXX_3.4
+   829: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsUTF8AndSize
+   830: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Size
+   831: 000000000001e3d0   123 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl11size_customEl
+   832: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD2Ev
+   833: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
    834: 00000000000151b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
    835: 000000000001e470    29 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
    836: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda21warn_or_error_on_syncEv
    837: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD2Ev
    838: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD2Ev
    839: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt11range_error@GLIBCXX_3.4
```

### readelf --wide --relocs {}

```diff
@@ -41,15 +41,15 @@
 00000000000b69e8  0000000000000008 R_X86_64_RELATIVE                         b5990
 00000000000b6a40  0000000000000008 R_X86_64_RELATIVE                         37988
 00000000000b6a58  0000000000000008 R_X86_64_RELATIVE                         9d658
 00000000000b6a70  0000000000000008 R_X86_64_RELATIVE                         9de68
 00000000000b53e0  0000003800000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 + 10
 00000000000b5790  0000003800000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 + 10
 00000000000b5938  0000003800000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 + 10
-00000000000b53e8  0000017100000001 R_X86_64_64            00000000000348c0 _ZTSN3c1020intrusive_ptr_targetE + 0
+00000000000b53e8  0000016f00000001 R_X86_64_64            00000000000348c0 _ZTSN3c1020intrusive_ptr_targetE + 0
 00000000000b53f0  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5408  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5420  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5438  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b56d8  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5700  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5778  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
@@ -64,275 +64,275 @@
 00000000000b59c0  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b53f8  000001d000000001 R_X86_64_64            00000000000348e0 _ZTSN3c1011SymNodeImplE + 0
 00000000000b5400  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
 00000000000b5418  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
 00000000000b5430  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
 00000000000b5468  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
 00000000000b5410  000001e200000001 R_X86_64_64            0000000000034900 _ZTSN3c1015VariableVersion14VersionCounterE + 0
-00000000000b5428  0000022600000001 R_X86_64_64            0000000000034930 _ZTSN3c1014OperatorKernelE + 0
+00000000000b5428  0000022700000001 R_X86_64_64            0000000000034930 _ZTSN3c1014OperatorKernelE + 0
 00000000000b5440  000001f100000001 R_X86_64_64            0000000000034960 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
-00000000000b5448  0000016600000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b5690  0000016600000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b56e8  0000016600000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b5710  0000016600000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b57c8  0000016600000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b5448  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b5690  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b56e8  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b5710  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b57c8  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
 00000000000b5450  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b56f0  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b5718  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b57d0  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b5458  000001db00000001 R_X86_64_64            00000000000349e0 _ZTSFN2at6TensorES0_S0_S0_lE + 0
-00000000000b5470  0000022f00000001 R_X86_64_64            0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
-00000000000b5478  000001ff00000001 R_X86_64_64            0000000000016ff0 _ZN3c1020intrusive_ptr_targetD0Ev + 0
-00000000000b5480  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b54a8  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5680  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b56a8  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b56d0  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5748  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5770  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b58f0  0000018e00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5e58  0000018e00000006 R_X86_64_GLOB_DAT      0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5470  0000023000000001 R_X86_64_64            0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
+00000000000b5478  0000020000000001 R_X86_64_64            0000000000016ff0 _ZN3c1020intrusive_ptr_targetD0Ev + 0
+00000000000b5480  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b54a8  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5680  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b56a8  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b56d0  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5748  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5770  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b58f0  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5e60  0000018c00000006 R_X86_64_GLOB_DAT      0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
 00000000000b5490  0000025000000001 R_X86_64_64            00000000000b53f0 _ZTIN3c1011SymNodeImplE + 0
-00000000000b5498  000001c800000001 R_X86_64_64            0000000000017100 _ZN3c1011SymNodeImplD1Ev + 0
-00000000000b54a0  000001a100000001 R_X86_64_64            0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
-00000000000b5de8  000001a100000006 R_X86_64_GLOB_DAT      0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
+00000000000b5498  000001c700000001 R_X86_64_64            0000000000017100 _ZN3c1011SymNodeImplD1Ev + 0
+00000000000b54a0  0000019f00000001 R_X86_64_64            0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
+00000000000b5df0  0000019f00000006 R_X86_64_GLOB_DAT      0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
 00000000000b54b0  0000013500000001 R_X86_64_64            00000000000156f0 _ZN3c1011SymNodeImpl6is_intEv + 0
-00000000000b54b8  0000017700000001 R_X86_64_64            00000000000156c0 _ZN3c1011SymNodeImpl7is_boolEv + 0
-00000000000b54c0  000001c500000001 R_X86_64_64            0000000000015690 _ZN3c1011SymNodeImpl8is_floatEv + 0
+00000000000b54b8  0000017500000001 R_X86_64_64            00000000000156c0 _ZN3c1011SymNodeImpl7is_boolEv + 0
+00000000000b54c0  000001c400000001 R_X86_64_64            0000000000015690 _ZN3c1011SymNodeImpl8is_floatEv + 0
 00000000000b54c8  0000025b00000001 R_X86_64_64            0000000000014e70 _ZNK3c1011SymNodeImpl13is_nested_intEv + 0
 00000000000b54d0  0000024500000001 R_X86_64_64            0000000000015660 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54d8  000001a000000001 R_X86_64_64            0000000000015630 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54e0  0000021500000001 R_X86_64_64            0000000000015600 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54e8  0000017200000001 R_X86_64_64            00000000000155d0 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54d8  0000019e00000001 R_X86_64_64            0000000000015630 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54e0  0000021600000001 R_X86_64_64            0000000000015600 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54e8  0000017000000001 R_X86_64_64            00000000000155d0 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b54f0  000001e400000001 R_X86_64_64            00000000000155a0 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b54f8  0000014c00000001 R_X86_64_64            0000000000015570 _ZN3c1011SymNodeImpl8floordivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5500  000001ac00000001 R_X86_64_64            0000000000015540 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5508  0000020900000001 R_X86_64_64            0000000000015510 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5510  000001cc00000001 R_X86_64_64            00000000000154e0 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5518  0000022900000001 R_X86_64_64            00000000000154b0 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5520  0000021200000001 R_X86_64_64            0000000000015480 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5500  000001aa00000001 R_X86_64_64            0000000000015540 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5508  0000020a00000001 R_X86_64_64            0000000000015510 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5510  000001cb00000001 R_X86_64_64            00000000000154e0 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5518  0000022a00000001 R_X86_64_64            00000000000154b0 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5520  0000021300000001 R_X86_64_64            0000000000015480 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5528  0000013800000001 R_X86_64_64            0000000000015450 _ZN3c1011SymNodeImpl2leERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5530  0000014500000001 R_X86_64_64            0000000000015420 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5538  0000015100000001 R_X86_64_64            00000000000153f0 _ZN3c1011SymNodeImpl4ceilEv + 0
-00000000000b5540  0000019700000001 R_X86_64_64            00000000000153c0 _ZN3c1011SymNodeImpl5floorEv + 0
-00000000000b5548  0000022e00000001 R_X86_64_64            0000000000015390 _ZN3c1011SymNodeImpl3negEv + 0
+00000000000b5540  0000019500000001 R_X86_64_64            00000000000153c0 _ZN3c1011SymNodeImpl5floorEv + 0
+00000000000b5548  0000022f00000001 R_X86_64_64            0000000000015390 _ZN3c1011SymNodeImpl3negEv + 0
 00000000000b5550  0000024f00000001 R_X86_64_64            0000000000015360 _ZN3c1011SymNodeImpl7sym_minERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5558  000001e600000001 R_X86_64_64            0000000000015330 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5560  0000020f00000001 R_X86_64_64            0000000000015300 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5568  000001b200000001 R_X86_64_64            00000000000152d0 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5570  0000020a00000001 R_X86_64_64            00000000000152a0 _ZN3c1011SymNodeImpl7sym_notEv + 0
-00000000000b5578  000001fb00000001 R_X86_64_64            0000000000015270 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_ + 0
-00000000000b5580  0000018300000001 R_X86_64_64            0000000000015240 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b5588  0000019300000001 R_X86_64_64            0000000000015210 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b5560  0000021000000001 R_X86_64_64            0000000000015300 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5568  000001b000000001 R_X86_64_64            00000000000152d0 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5570  0000020b00000001 R_X86_64_64            00000000000152a0 _ZN3c1011SymNodeImpl7sym_notEv + 0
+00000000000b5578  000001fc00000001 R_X86_64_64            0000000000015270 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_ + 0
+00000000000b5580  0000018100000001 R_X86_64_64            0000000000015240 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b5588  0000019100000001 R_X86_64_64            0000000000015210 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
 00000000000b5590  0000025800000001 R_X86_64_64            00000000000151e0 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b5598  0000021900000001 R_X86_64_64            00000000000151b0 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b55a0  000001c000000001 R_X86_64_64            0000000000015180 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b5598  0000021a00000001 R_X86_64_64            00000000000151b0 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b55a0  000001be00000001 R_X86_64_64            0000000000015180 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
 00000000000b55a8  0000013c00000001 R_X86_64_64            0000000000015150 _ZN3c1011SymNodeImpl28is_non_overlapping_and_denseENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b55b0  0000016c00000001 R_X86_64_64            0000000000015120 _ZN3c1011SymNodeImpl5cloneEv + 0
-00000000000b55b8  0000018a00000001 R_X86_64_64            00000000000150f0 _ZN3c1011SymNodeImpl9sym_floatEv + 0
+00000000000b55b0  0000016a00000001 R_X86_64_64            0000000000015120 _ZN3c1011SymNodeImpl5cloneEv + 0
+00000000000b55b8  0000018800000001 R_X86_64_64            00000000000150f0 _ZN3c1011SymNodeImpl9sym_floatEv + 0
 00000000000b55c0  0000025200000001 R_X86_64_64            00000000000150c0 _ZN3c1011SymNodeImpl8wrap_intEl + 0
 00000000000b55c8  000001e900000001 R_X86_64_64            0000000000015090 _ZN3c1011SymNodeImpl10wrap_floatEd + 0
-00000000000b55d0  0000018100000001 R_X86_64_64            0000000000015060 _ZN3c1011SymNodeImpl9wrap_boolEb + 0
-00000000000b55d8  000001fc00000001 R_X86_64_64            0000000000015030 _ZN3c1011SymNodeImpl9guard_intEPKcl + 0
-00000000000b55e0  000001f400000001 R_X86_64_64            0000000000015000 _ZN3c1011SymNodeImpl10guard_boolEPKcl + 0
-00000000000b55e8  0000019800000001 R_X86_64_64            0000000000014fd0 _ZN3c1011SymNodeImpl11guard_floatEPKcl + 0
+00000000000b55d0  0000017f00000001 R_X86_64_64            0000000000015060 _ZN3c1011SymNodeImpl9wrap_boolEb + 0
+00000000000b55d8  000001fd00000001 R_X86_64_64            0000000000015030 _ZN3c1011SymNodeImpl9guard_intEPKcl + 0
+00000000000b55e0  000001f500000001 R_X86_64_64            0000000000015000 _ZN3c1011SymNodeImpl10guard_boolEPKcl + 0
+00000000000b55e8  0000019600000001 R_X86_64_64            0000000000014fd0 _ZN3c1011SymNodeImpl11guard_floatEPKcl + 0
 00000000000b55f0  0000015700000001 R_X86_64_64            0000000000014e80 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl + 0
-00000000000b55f8  000001bd00000001 R_X86_64_64            0000000000014e90 _ZN3c1011SymNodeImpl11expect_trueEPKcl + 0
-00000000000b5600  0000020400000001 R_X86_64_64            0000000000017360 _ZN3c1011SymNodeImpl11expect_sizeEPKcl + 0
-00000000000b5608  0000023500000001 R_X86_64_64            0000000000014fa0 _ZN3c1011SymNodeImpl4int_Ev + 0
-00000000000b5610  0000022000000001 R_X86_64_64            0000000000014f70 _ZN3c1011SymNodeImpl5bool_Ev + 0
-00000000000b5618  000001bf00000001 R_X86_64_64            0000000000014f40 _ZN3c1011SymNodeImpl8has_hintEv + 0
+00000000000b55f8  000001bb00000001 R_X86_64_64            0000000000014e90 _ZN3c1011SymNodeImpl11expect_trueEPKcl + 0
+00000000000b5600  0000020500000001 R_X86_64_64            0000000000017360 _ZN3c1011SymNodeImpl11expect_sizeEPKcl + 0
+00000000000b5608  0000023600000001 R_X86_64_64            0000000000014fa0 _ZN3c1011SymNodeImpl4int_Ev + 0
+00000000000b5610  0000022100000001 R_X86_64_64            0000000000014f70 _ZN3c1011SymNodeImpl5bool_Ev + 0
+00000000000b5618  000001bd00000001 R_X86_64_64            0000000000014f40 _ZN3c1011SymNodeImpl8has_hintEv + 0
 00000000000b5620  0000013d00000001 R_X86_64_64            0000000000014f10 _ZN3c1011SymNodeImpl3strEv + 0
 00000000000b5628  0000015000000001 R_X86_64_64            0000000000014ea0 _ZN3c1011SymNodeImpl10nested_intEv + 0
 00000000000b5630  0000013200000001 R_X86_64_64            0000000000014eb0 _ZN3c1011SymNodeImpl16nested_int_coeffEv + 0
-00000000000b5638  0000018700000001 R_X86_64_64            0000000000014ec0 _ZN3c1011SymNodeImpl12constant_intEv + 0
+00000000000b5638  0000018500000001 R_X86_64_64            0000000000014ec0 _ZN3c1011SymNodeImpl12constant_intEv + 0
 00000000000b5640  000001da00000001 R_X86_64_64            0000000000014ed0 _ZN3c1011SymNodeImpl13constant_boolEv + 0
-00000000000b5648  000001a500000001 R_X86_64_64            0000000000014ee0 _ZN3c1011SymNodeImpl12maybe_as_intEv + 0
-00000000000b5650  000001de00000001 R_X86_64_64            0000000000014ef0 _ZN3c1011SymNodeImpl11is_constantEv + 0
+00000000000b5648  000001a300000001 R_X86_64_64            0000000000014ee0 _ZN3c1011SymNodeImpl12maybe_as_intEv + 0
+00000000000b5650  000001dd00000001 R_X86_64_64            0000000000014ef0 _ZN3c1011SymNodeImpl11is_constantEv + 0
 00000000000b5658  000001d600000001 R_X86_64_64            0000000000014f00 _ZN3c1011SymNodeImpl11is_symbolicEv + 0
-00000000000b5668  0000022d00000001 R_X86_64_64            00000000000b5408 _ZTIN3c1015VariableVersion14VersionCounterE + 0
-00000000000b5670  0000017400000001 R_X86_64_64            0000000000017010 _ZN3c1015VariableVersion14VersionCounterD1Ev + 0
+00000000000b5668  0000022e00000001 R_X86_64_64            00000000000b5408 _ZTIN3c1015VariableVersion14VersionCounterE + 0
+00000000000b5670  0000017200000001 R_X86_64_64            0000000000017010 _ZN3c1015VariableVersion14VersionCounterD1Ev + 0
 00000000000b5678  0000014600000001 R_X86_64_64            0000000000017030 _ZN3c1015VariableVersion14VersionCounterD0Ev + 0
 00000000000b5698  0000023c00000001 R_X86_64_64            0000000000017060 _ZN3c1014OperatorKernelD1Ev + 0
-00000000000b56a0  0000020b00000001 R_X86_64_64            0000000000017080 _ZN3c1014OperatorKernelD0Ev + 0
-00000000000b56b8  000001a200000001 R_X86_64_64            00000000000b5438 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
-00000000000b56c0  000001fe00000001 R_X86_64_64            00000000000170b0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev + 0
+00000000000b56a0  0000020c00000001 R_X86_64_64            0000000000017080 _ZN3c1014OperatorKernelD0Ev + 0
+00000000000b56b8  000001a000000001 R_X86_64_64            00000000000b5438 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
+00000000000b56c0  000001ff00000001 R_X86_64_64            00000000000170b0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev + 0
 00000000000b56c8  000001d700000001 R_X86_64_64            00000000000170d0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev + 0
 00000000000b56e0  0000014a00000001 R_X86_64_64            0000000000035000 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
-00000000000b56f8  0000022500000001 R_X86_64_64            0000000000035070 _ZTSFN2at6TensorES0_E + 0
-00000000000b5708  0000022100000001 R_X86_64_64            00000000000350a0 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
-00000000000b5720  0000019c00000001 R_X86_64_64            0000000000035120 _ZTSFN2at6TensorES0_S0_E + 0
+00000000000b56f8  0000022600000001 R_X86_64_64            0000000000035070 _ZTSFN2at6TensorES0_E + 0
+00000000000b5708  0000022200000001 R_X86_64_64            00000000000350a0 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
+00000000000b5720  0000019a00000001 R_X86_64_64            0000000000035120 _ZTSFN2at6TensorES0_S0_E + 0
 00000000000b5730  0000023e00000001 R_X86_64_64            00000000000b56d8 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
-00000000000b5738  0000023200000001 R_X86_64_64            000000000001b000 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev + 0
-00000000000b5740  0000020200000001 R_X86_64_64            000000000001b020 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev + 0
-00000000000b5758  0000021f00000001 R_X86_64_64            00000000000b5700 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
+00000000000b5738  0000023300000001 R_X86_64_64            000000000001b000 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev + 0
+00000000000b5740  0000020300000001 R_X86_64_64            000000000001b020 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev + 0
+00000000000b5758  0000022000000001 R_X86_64_64            00000000000b5700 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
 00000000000b5760  000001ee00000001 R_X86_64_64            000000000001b050 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev + 0
-00000000000b5768  000001ca00000001 R_X86_64_64            000000000001b070 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev + 0
-00000000000b5780  0000017300000001 R_X86_64_64            0000000000036190 _ZTSN3c1010ValueErrorE + 0
+00000000000b5768  000001c900000001 R_X86_64_64            000000000001b070 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev + 0
+00000000000b5780  0000017100000001 R_X86_64_64            0000000000036190 _ZTSN3c1010ValueErrorE + 0
 00000000000b5788  0000012b00000001 R_X86_64_64            0000000000000000 _ZTIN3c105ErrorE + 0
 00000000000b5798  000001dc00000001 R_X86_64_64            00000000000361c0 _ZTSN3c104impl24DeviceGuardImplInterfaceE + 0
 00000000000b57a8  0000024300000001 R_X86_64_64            0000000000036200 _ZTSN3c104cuda4impl13CUDAGuardImplE + 0
-00000000000b57b0  000001f600000001 R_X86_64_64            00000000000b5790 _ZTIN3c104impl24DeviceGuardImplInterfaceE + 0
-00000000000b57c0  000001df00000001 R_X86_64_64            0000000000036220 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
-00000000000b57d8  0000018c00000001 R_X86_64_64            00000000000362a0 _ZTSFN2at6TensorERKS0_S2_dE + 0
+00000000000b57b0  000001f700000001 R_X86_64_64            00000000000b5790 _ZTIN3c104impl24DeviceGuardImplInterfaceE + 0
+00000000000b57c0  000001de00000001 R_X86_64_64            0000000000036220 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
+00000000000b57d8  0000018a00000001 R_X86_64_64            00000000000362a0 _ZTSFN2at6TensorERKS0_S2_dE + 0
 00000000000b57e8  0000025a00000001 R_X86_64_64            00000000000b5778 _ZTIN3c1010ValueErrorE + 0
-00000000000b5dd0  0000025a00000006 R_X86_64_GLOB_DAT      00000000000b5778 _ZTIN3c1010ValueErrorE + 0
-00000000000b57f0  0000016900000001 R_X86_64_64            000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
-00000000000b5e28  0000016900000006 R_X86_64_GLOB_DAT      000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
+00000000000b5dd8  0000025a00000006 R_X86_64_GLOB_DAT      00000000000b5778 _ZTIN3c1010ValueErrorE + 0
+00000000000b57f0  0000016700000001 R_X86_64_64            000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
+00000000000b5e30  0000016700000006 R_X86_64_GLOB_DAT      000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
 00000000000b57f8  0000013e00000001 R_X86_64_64            000000000001e9f0 _ZN3c1010ValueErrorD0Ev + 0
 00000000000b5800  0000009c00000001 R_X86_64_64            0000000000000000 _ZNK3c105Error4whatEv + 0
-00000000000b5808  000001a300000001 R_X86_64_64            000000000001deb0 _ZNK3c105Error22what_without_backtraceEv + 0
+00000000000b5808  000001a100000001 R_X86_64_64            000000000001deb0 _ZNK3c105Error22what_without_backtraceEv + 0
 00000000000b5818  0000024800000001 R_X86_64_64            00000000000b57a0 _ZTIN3c104cuda4impl13CUDAGuardImplE + 0
-00000000000b5820  0000021e00000001 R_X86_64_64            000000000001e000 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv + 0
+00000000000b5820  0000021f00000001 R_X86_64_64            000000000001e000 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv + 0
 00000000000b5828  0000025600000001 R_X86_64_64            000000000001f970 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeDeviceENS_6DeviceE + 0
 00000000000b5830  0000023b00000001 R_X86_64_64            000000000001f8a0 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv + 0
-00000000000b5838  0000018d00000001 R_X86_64_64            000000000001e090 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE + 0
+00000000000b5838  0000018b00000001 R_X86_64_64            000000000001e090 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE + 0
 00000000000b5840  0000015500000001 R_X86_64_64            0000000000020930 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE + 0
-00000000000b5848  000001f300000001 R_X86_64_64            000000000001e050 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE + 0
-00000000000b5850  0000022800000001 R_X86_64_64            000000000001e3b0 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE + 0
-00000000000b5858  000001ba00000001 R_X86_64_64            000000000001e380 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb + 0
+00000000000b5848  000001f400000001 R_X86_64_64            000000000001e050 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE + 0
+00000000000b5850  0000022900000001 R_X86_64_64            000000000001e3b0 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE + 0
+00000000000b5858  000001b800000001 R_X86_64_64            000000000001e380 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb + 0
 00000000000b5860  0000014b00000001 R_X86_64_64            000000000001e350 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi + 0
-00000000000b5868  0000019400000001 R_X86_64_64            000000000001e2e0 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE + 0
+00000000000b5868  0000019200000001 R_X86_64_64            000000000001e2e0 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE + 0
 00000000000b5870  0000024900000001 R_X86_64_64            0000000000020d70 _ZNK3c104cuda4impl13CUDAGuardImpl12destroyEventEPva + 0
 00000000000b5878  000001d800000001 R_X86_64_64            000000000001fc50 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE + 0
-00000000000b5880  0000021400000001 R_X86_64_64            000000000001fa40 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE + 0
+00000000000b5880  0000021500000001 R_X86_64_64            000000000001fa40 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE + 0
 00000000000b5888  000001e100000001 R_X86_64_64            000000000001e490 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv + 0
-00000000000b5890  0000023300000001 R_X86_64_64            000000000001e2d0 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv + 0
+00000000000b5890  0000023400000001 R_X86_64_64            000000000001e2d0 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv + 0
 00000000000b5898  0000025500000001 R_X86_64_64            00000000000223b0 _ZNK3c104cuda4impl13CUDAGuardImpl11queryStreamERKNS_6StreamE + 0
-00000000000b58a0  0000018500000001 R_X86_64_64            0000000000022570 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE + 0
-00000000000b58a8  0000017c00000001 R_X86_64_64            000000000001e250 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv + 0
-00000000000b58b0  0000021d00000001 R_X86_64_64            000000000001e200 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE + 0
-00000000000b58b8  0000016e00000001 R_X86_64_64            000000000001e0f0 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a + 0
+00000000000b58a0  0000018300000001 R_X86_64_64            0000000000022570 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE + 0
+00000000000b58a8  0000017a00000001 R_X86_64_64            000000000001e250 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv + 0
+00000000000b58b0  0000021e00000001 R_X86_64_64            000000000001e200 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE + 0
+00000000000b58b8  0000016c00000001 R_X86_64_64            000000000001e0f0 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a + 0
 00000000000b58c0  0000015200000001 R_X86_64_64            000000000001e010 _ZN3c104cuda4impl13CUDAGuardImplD1Ev + 0
 00000000000b58c8  0000025100000001 R_X86_64_64            000000000001e070 _ZN3c104cuda4impl13CUDAGuardImplD0Ev + 0
 00000000000b58d8  0000014700000001 R_X86_64_64            00000000000b57b8 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
 00000000000b58e0  000001ef00000001 R_X86_64_64            0000000000020030 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev + 0
-00000000000b58e8  000001cd00000001 R_X86_64_64            0000000000020100 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev + 0
-00000000000b5900  000001a900000001 R_X86_64_64            0000000000036530 _ZTSSt19bad_optional_access + 0
+00000000000b58e8  000001cc00000001 R_X86_64_64            0000000000020100 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev + 0
+00000000000b5900  000001a700000001 R_X86_64_64            0000000000036530 _ZTSSt19bad_optional_access + 0
 00000000000b5908  0000002300000001 R_X86_64_64            0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
 00000000000b59b8  0000002300000001 R_X86_64_64            0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
 00000000000b5d30  0000002300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
 00000000000b6a30  0000002300000001 R_X86_64_64            0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
-00000000000b5918  0000021700000001 R_X86_64_64            00000000000b58f8 _ZTISt19bad_optional_access + 0
+00000000000b5918  0000021800000001 R_X86_64_64            00000000000b58f8 _ZTISt19bad_optional_access + 0
 00000000000b5920  0000014e00000001 R_X86_64_64            00000000000251e0 _ZNSt19bad_optional_accessD1Ev + 0
 00000000000b5928  0000024e00000001 R_X86_64_64            0000000000025200 _ZNSt19bad_optional_accessD0Ev + 0
-00000000000b5930  0000016400000001 R_X86_64_64            00000000000251d0 _ZNKSt19bad_optional_access4whatEv + 0
-00000000000b5940  0000017800000001 R_X86_64_64            0000000000037720 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
+00000000000b5930  0000016300000001 R_X86_64_64            00000000000251d0 _ZNKSt19bad_optional_access4whatEv + 0
+00000000000b5940  0000017600000001 R_X86_64_64            0000000000037720 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
 00000000000b5950  000001e000000001 R_X86_64_64            00000000000377a0 _ZTSSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
 00000000000b5958  000001f000000001 R_X86_64_64            00000000000b5938 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
 00000000000b5970  0000007f00000001 R_X86_64_64            0000000000000000 _ZTISt13runtime_error@GLIBCXX_3.4 + 0
-00000000000b5e20  0000007f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt13runtime_error@GLIBCXX_3.4 + 0
-00000000000b59d0  0000018f00000001 R_X86_64_64            00000000000b5948 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
+00000000000b5e28  0000007f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt13runtime_error@GLIBCXX_3.4 + 0
+00000000000b59d0  0000018d00000001 R_X86_64_64            00000000000b5948 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
 00000000000b59f8  000000be00000001 R_X86_64_64            0000000000000000 _ZNKSt13runtime_error4whatEv@GLIBCXX_3.4 + 0
 00000000000b5a28  000000be00000001 R_X86_64_64            0000000000000000 _ZNKSt13runtime_error4whatEv@GLIBCXX_3.4 + 0
 00000000000b5a00  0000007300000001 R_X86_64_64            0000000000000000 __cxa_pure_virtual@CXXABI_1.3 + 0
 00000000000b5cb8  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 PyInstanceMethod_Type + 0
-00000000000b5cc0  0000021600000006 R_X86_64_GLOB_DAT      000000000001e020 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d + 0
+00000000000b5cc0  0000021700000006 R_X86_64_GLOB_DAT      000000000001e020 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d + 0
 00000000000b5cc8  0000013100000006 R_X86_64_GLOB_DAT      0000000000019200 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
-00000000000b5cd0  000001aa00000006 R_X86_64_GLOB_DAT      00000000000b5910 _ZTVSt19bad_optional_access + 0
+00000000000b5cd0  000001a800000006 R_X86_64_GLOB_DAT      00000000000b5910 _ZTVSt19bad_optional_access + 0
 00000000000b5cd8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000000000 PyByteArray_Type + 0
-00000000000b5ce0  0000025900000006 R_X86_64_GLOB_DAT      00000000000157b0 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
-00000000000b5ce8  0000001000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c1019UndefinedTensorImpl10_singletonE + 0
-00000000000b5cf0  000001ce00000006 R_X86_64_GLOB_DAT      0000000000022f80 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE + 0
-00000000000b5cf8  0000014100000006 R_X86_64_GLOB_DAT      000000000001b110 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_ + 0
-00000000000b5d00  0000001400000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_RuntimeError + 0
-00000000000b5d08  0000016300000006 R_X86_64_GLOB_DAT      000000000001e690 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py + 0
-00000000000b5d10  0000018200000006 R_X86_64_GLOB_DAT      000000000001a380 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE + 0
+00000000000b5ce0  000001cf00000006 R_X86_64_GLOB_DAT      000000000001e690 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py + 0
+00000000000b5ce8  0000025900000006 R_X86_64_GLOB_DAT      00000000000157b0 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
+00000000000b5cf0  0000001000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c1019UndefinedTensorImpl10_singletonE + 0
+00000000000b5cf8  000001cd00000006 R_X86_64_GLOB_DAT      0000000000022f80 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE + 0
+00000000000b5d00  0000014100000006 R_X86_64_GLOB_DAT      000000000001b110 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_ + 0
+00000000000b5d08  0000001400000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_RuntimeError + 0
+00000000000b5d10  0000018000000006 R_X86_64_GLOB_DAT      000000000001a380 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE + 0
 00000000000b5d18  0000001e00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_MemoryError + 0
 00000000000b5d20  0000001f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVN3c105ErrorE + 0
 00000000000b5d28  0000002000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSs4_Rep20_S_empty_rep_storageE@GLIBCXX_3.4 + 0
-00000000000b5d38  0000020600000006 R_X86_64_GLOB_DAT      00000000000b6ce4 _ZZN3c104cuda13warning_stateEvE14warning_state_ + 0
+00000000000b5d38  0000020700000006 R_X86_64_GLOB_DAT      00000000000b6ce4 _ZZN3c104cuda13warning_stateEvE14warning_state_ + 0
 00000000000b5d40  0000002400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl26device_guard_impl_registryE + 0
 00000000000b5d48  0000002900000006 R_X86_64_GLOB_DAT      0000000000000000 PyBaseObject_Type + 0
 00000000000b5d50  0000002c00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12out_of_range@GLIBCXX_3.4 + 0
 00000000000b6a08  0000002c00000001 R_X86_64_64            0000000000000000 _ZTISt12out_of_range@GLIBCXX_3.4 + 0
 00000000000b5d58  0000002e00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl8GPUTrace13gpuTraceStateE + 0
 00000000000b5d60  0000002f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12length_error@GLIBCXX_3.4 + 0
 00000000000b6a00  0000002f00000001 R_X86_64_64            0000000000000000 _ZTISt12length_error@GLIBCXX_3.4 + 0
 00000000000b5d68  0000003300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
 00000000000b5d70  0000003a00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt9bad_alloc@GLIBCXX_3.4 + 0
-00000000000b5d78  0000019f00000006 R_X86_64_GLOB_DAT      0000000000015b30 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5d80  000001fd00000006 R_X86_64_GLOB_DAT      00000000000b57d0 _ZTIFN2at6TensorERKS0_S2_dE + 0
-00000000000b5d88  000001a800000006 R_X86_64_GLOB_DAT      00000000000b5718 _ZTIFN2at6TensorES0_S0_E + 0
-00000000000b5d90  000001c400000006 R_X86_64_GLOB_DAT      0000000000015db0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5d98  000001d300000006 R_X86_64_GLOB_DAT      00000000000b5660 _ZTVN3c1015VariableVersion14VersionCounterE + 0
-00000000000b5da0  0000015f00000006 R_X86_64_GLOB_DAT      000000000001a700 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_ + 0
-00000000000b5da8  0000006100000006 R_X86_64_GLOB_DAT      0000000000000000 vsnprintf@GLIBC_2.2.5 + 0
-00000000000b5db0  0000020e00000006 R_X86_64_GLOB_DAT      000000000001b0a0 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_ + 0
-00000000000b5db8  0000013300000006 R_X86_64_GLOB_DAT      00000000000b5450 _ZTIFN2at6TensorES0_S0_S0_lE + 0
-00000000000b5dc0  0000006200000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_TypeError + 0
-00000000000b5dc8  0000016d00000006 R_X86_64_GLOB_DAT      00000000000b5488 _ZTVN3c1011SymNodeImplE + 0
-00000000000b5dd8  0000022b00000006 R_X86_64_GLOB_DAT      00000000000b5728 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
-00000000000b5de0  0000022400000006 R_X86_64_GLOB_DAT      00000000000158b0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5df0  000001f800000006 R_X86_64_GLOB_DAT      0000000000024910 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE + 0
-00000000000b5df8  0000017d00000006 R_X86_64_GLOB_DAT      00000000000b5688 _ZTVN3c1014OperatorKernelE + 0
-00000000000b5e00  0000017600000006 R_X86_64_GLOB_DAT      0000000000015c70 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5e08  0000007400000006 R_X86_64_GLOB_DAT      0000000000000000 __pthread_key_create@GLIBC_2.2.5 + 0
-00000000000b5e10  000001c200000006 R_X86_64_GLOB_DAT      0000000000015760 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
-00000000000b5e18  0000007d00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16nested_exception@CXXABI_1.3.5 + 0
+00000000000b5d78  0000019d00000006 R_X86_64_GLOB_DAT      0000000000015b30 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5d80  000001df00000006 R_X86_64_GLOB_DAT      000000000001e5c0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py + 0
+00000000000b5d88  000001fe00000006 R_X86_64_GLOB_DAT      00000000000b57d0 _ZTIFN2at6TensorERKS0_S2_dE + 0
+00000000000b5d90  000001a600000006 R_X86_64_GLOB_DAT      00000000000b5718 _ZTIFN2at6TensorES0_S0_E + 0
+00000000000b5d98  000001c300000006 R_X86_64_GLOB_DAT      0000000000015db0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5da0  000001d300000006 R_X86_64_GLOB_DAT      00000000000b5660 _ZTVN3c1015VariableVersion14VersionCounterE + 0
+00000000000b5da8  0000015f00000006 R_X86_64_GLOB_DAT      000000000001a700 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_ + 0
+00000000000b5db0  0000006100000006 R_X86_64_GLOB_DAT      0000000000000000 vsnprintf@GLIBC_2.2.5 + 0
+00000000000b5db8  0000020f00000006 R_X86_64_GLOB_DAT      000000000001b0a0 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_ + 0
+00000000000b5dc0  0000013300000006 R_X86_64_GLOB_DAT      00000000000b5450 _ZTIFN2at6TensorES0_S0_S0_lE + 0
+00000000000b5dc8  0000006200000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_TypeError + 0
+00000000000b5dd0  0000016b00000006 R_X86_64_GLOB_DAT      00000000000b5488 _ZTVN3c1011SymNodeImplE + 0
+00000000000b5de0  0000022c00000006 R_X86_64_GLOB_DAT      00000000000b5728 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
+00000000000b5de8  0000022500000006 R_X86_64_GLOB_DAT      00000000000158b0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5df8  000001f900000006 R_X86_64_GLOB_DAT      0000000000024910 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE + 0
+00000000000b5e00  0000017b00000006 R_X86_64_GLOB_DAT      00000000000b5688 _ZTVN3c1014OperatorKernelE + 0
+00000000000b5e08  0000017400000006 R_X86_64_GLOB_DAT      0000000000015c70 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5e10  0000007400000006 R_X86_64_GLOB_DAT      0000000000000000 __pthread_key_create@GLIBC_2.2.5 + 0
+00000000000b5e18  000001c100000006 R_X86_64_GLOB_DAT      0000000000015760 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
+00000000000b5e20  0000007d00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16nested_exception@CXXABI_1.3.5 + 0
 00000000000b6a20  0000007d00000001 R_X86_64_64            0000000000000000 _ZTISt16nested_exception@CXXABI_1.3.5 + 0
-00000000000b5e30  0000008400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-00000000000b5e38  0000008500000006 R_X86_64_GLOB_DAT      0000000000000000 PyCFunction_Type + 0
-00000000000b5e40  0000024000000006 R_X86_64_GLOB_DAT      0000000000015ef0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5e48  0000016100000006 R_X86_64_GLOB_DAT      0000000000015800 _ZN5torch6detail16TorchLibraryInitD1Ev + 0
-00000000000b5e50  0000009400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
-00000000000b5e60  0000009500000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ImportError + 0
-00000000000b5e68  000001dd00000006 R_X86_64_GLOB_DAT      000000000001e5c0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py + 0
-00000000000b5e70  0000020000000006 R_X86_64_GLOB_DAT      0000000000016030 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5e78  0000020800000006 R_X86_64_GLOB_DAT      00000000000b56f0 _ZTIFN2at6TensorES0_E + 0
+00000000000b5e38  0000008400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+00000000000b5e40  0000008500000006 R_X86_64_GLOB_DAT      0000000000000000 PyCFunction_Type + 0
+00000000000b5e48  0000024000000006 R_X86_64_GLOB_DAT      0000000000015ef0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5e50  0000016100000006 R_X86_64_GLOB_DAT      0000000000015800 _ZN5torch6detail16TorchLibraryInitD1Ev + 0
+00000000000b5e58  0000009400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
+00000000000b5e68  0000009500000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ImportError + 0
+00000000000b5e70  0000020100000006 R_X86_64_GLOB_DAT      0000000000016030 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5e78  0000020900000006 R_X86_64_GLOB_DAT      00000000000b56f0 _ZTIFN2at6TensorES0_E + 0
 00000000000b5e80  000000a200000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt14overflow_error@GLIBCXX_3.4 + 0
 00000000000b6a10  000000a200000001 R_X86_64_64            0000000000000000 _ZTISt14overflow_error@GLIBCXX_3.4 + 0
 00000000000b5e88  000000a300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ValueError + 0
 00000000000b5e90  000000ad00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt9bad_allocD1Ev@GLIBCXX_3.4 + 0
 00000000000b5e98  0000013900000006 R_X86_64_GLOB_DAT      00000000000159f0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
 00000000000b5ea0  000000b300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_OverflowError + 0
 00000000000b5ea8  000000b400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
 00000000000b5eb0  000000b700000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
 00000000000b5eb8  000000b800000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 00000000000b5ec0  000000b900000006 R_X86_64_GLOB_DAT      0000000000000000 PyDict_Type + 0
 00000000000b5ec8  000000ba00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12domain_error@GLIBCXX_3.4 + 0
 00000000000b69f8  000000ba00000001 R_X86_64_64            0000000000000000 _ZTISt12domain_error@GLIBCXX_3.4 + 0
 00000000000b5ed0  0000015c00000006 R_X86_64_GLOB_DAT      00000000000b56b0 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
-00000000000b5ed8  0000021b00000006 R_X86_64_GLOB_DAT      0000000000013980 _Z16SplitK_ReductionP6__halfPfmmi + 0
+00000000000b5ed8  0000021c00000006 R_X86_64_GLOB_DAT      0000000000013980 _Z16SplitK_ReductionP6__halfPfmmi + 0
 00000000000b5ee0  000000cb00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104cuda20CUDACachingAllocator9allocatorE + 0
 00000000000b5ee8  0000014f00000006 R_X86_64_GLOB_DAT      00000000000b58d0 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
 00000000000b5ef0  000000d000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt16invalid_argumentD1Ev@GLIBCXX_3.4 + 0
 00000000000b5ef8  000000d100000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16invalid_argument@GLIBCXX_3.4 + 0
 00000000000b6a18  000000d100000001 R_X86_64_64            0000000000000000 _ZTISt16invalid_argument@GLIBCXX_3.4 + 0
 00000000000b5f00  000000d200000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
 00000000000b5f08  000000d900000006 R_X86_64_GLOB_DAT      0000000000000000 PyType_Type + 0
 00000000000b5f10  000000db00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVN5torch8autograd12AutogradMetaE + 0
-00000000000b5f18  0000019e00000006 R_X86_64_GLOB_DAT      00000000000b5460 _ZTVN3c1020intrusive_ptr_targetE + 0
+00000000000b5f18  0000019c00000006 R_X86_64_GLOB_DAT      00000000000b5460 _ZTVN3c1020intrusive_ptr_targetE + 0
 00000000000b5f20  000000dd00000006 R_X86_64_GLOB_DAT      0000000000000000 PyProperty_Type + 0
 00000000000b5f28  000000e500000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt9bad_alloc@GLIBCXX_3.4 + 0
 00000000000b6a28  000000e500000001 R_X86_64_64            0000000000000000 _ZTISt9bad_alloc@GLIBCXX_3.4 + 0
 00000000000b5f30  000000ea00000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NoneStruct + 0
-00000000000b5f38  0000020c00000006 R_X86_64_GLOB_DAT      000000000001b4f0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
-00000000000b5f40  000000f400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 + 0
-00000000000b5f48  000001ec00000006 R_X86_64_GLOB_DAT      00000000000b5750 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
-00000000000b5f50  000000f800000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NotImplementedStruct + 0
-00000000000b5f58  000000ff00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_SystemError + 0
-00000000000b5f60  0000010200000006 R_X86_64_GLOB_DAT      0000000000000000 PyCapsule_Type + 0
-00000000000b5f68  000001b900000006 R_X86_64_GLOB_DAT      000000000001e450 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
-00000000000b5f70  0000010700000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt13runtime_errorD1Ev@GLIBCXX_3.4 + 0
-00000000000b5f78  0000023600000006 R_X86_64_GLOB_DAT      000000000001bed0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d + 0
+00000000000b5f38  000001c000000006 R_X86_64_GLOB_DAT      000000000001bed0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d + 0
+00000000000b5f40  0000020d00000006 R_X86_64_GLOB_DAT      000000000001b4f0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
+00000000000b5f48  000000f400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 + 0
+00000000000b5f50  000001ec00000006 R_X86_64_GLOB_DAT      00000000000b5750 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
+00000000000b5f58  000000f800000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NotImplementedStruct + 0
+00000000000b5f60  000000ff00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_SystemError + 0
+00000000000b5f68  0000010200000006 R_X86_64_GLOB_DAT      0000000000000000 PyCapsule_Type + 0
+00000000000b5f70  000001b700000006 R_X86_64_GLOB_DAT      000000000001e450 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
+00000000000b5f78  0000010700000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt13runtime_errorD1Ev@GLIBCXX_3.4 + 0
 00000000000b5f80  0000010d00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_IndexError + 0
 00000000000b5f88  0000023900000006 R_X86_64_GLOB_DAT      0000000000017540 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l + 0
-00000000000b5f90  0000019500000006 R_X86_64_GLOB_DAT      0000000000016170 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5f90  0000019300000006 R_X86_64_GLOB_DAT      0000000000016170 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
 00000000000b5f98  0000023700000006 R_X86_64_GLOB_DAT      0000000000015720 _ZN3c1014getTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
 00000000000b5fa0  0000011400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt15basic_streambufIcSt11char_traitsIcEE@GLIBCXX_3.4 + 0
-00000000000b5fa8  0000018600000006 R_X86_64_GLOB_DAT      0000000000015740 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
-00000000000b5fb0  000001bb00000006 R_X86_64_GLOB_DAT      000000000001b7e0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
-00000000000b5fb8  0000022300000006 R_X86_64_GLOB_DAT      00000000000b57e0 _ZTVN3c1010ValueErrorE + 0
-00000000000b5fc0  0000023400000006 R_X86_64_GLOB_DAT      00000000000b5810 _ZTVN3c104cuda4impl13CUDAGuardImplE + 0
+00000000000b5fa8  0000018400000006 R_X86_64_GLOB_DAT      0000000000015740 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
+00000000000b5fb0  000001b900000006 R_X86_64_GLOB_DAT      000000000001b7e0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
+00000000000b5fb8  0000022400000006 R_X86_64_GLOB_DAT      00000000000b57e0 _ZTVN3c1010ValueErrorE + 0
+00000000000b5fc0  0000023500000006 R_X86_64_GLOB_DAT      00000000000b5810 _ZTVN3c104cuda4impl13CUDAGuardImplE + 0
 00000000000b5fc8  0000012000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt9basic_iosIcSt11char_traitsIcEE@GLIBCXX_3.4 + 0
 00000000000b5fd0  0000012300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl8GPUTrace9haveStateE + 0
-00000000000b5fd8  0000023100000006 R_X86_64_GLOB_DAT      0000000000014910 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l + 0
-00000000000b5fe0  0000016500000006 R_X86_64_GLOB_DAT      000000000001e4f0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py + 0
-00000000000b5fe8  0000024600000006 R_X86_64_GLOB_DAT      000000000001e3d0 _ZNK3c1010TensorImpl11size_customEl + 0
+00000000000b5fd8  0000023200000006 R_X86_64_GLOB_DAT      0000000000014910 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l + 0
+00000000000b5fe0  0000024600000006 R_X86_64_GLOB_DAT      000000000001e3d0 _ZNK3c1010TensorImpl11size_customEl + 0
+00000000000b5fe8  000001f300000006 R_X86_64_GLOB_DAT      000000000001e4f0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py + 0
 00000000000b5ff0  0000013f00000006 R_X86_64_GLOB_DAT      000000000001e470 _ZN3c1014getTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
 00000000000b5ff8  0000013000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt11range_error@GLIBCXX_3.4 + 0
 00000000000b69f0  0000013000000001 R_X86_64_64            0000000000000000 _ZTISt11range_error@GLIBCXX_3.4 + 0
 00000000000b69c0  000000f100000001 R_X86_64_64            0000000000000000 __gxx_personality_v0@CXXABI_1.3 + 0
 00000000000b69d0  000000ac00000001 R_X86_64_64            0000000000000000 _ZTIN10__cxxabiv115__forced_unwindE@CXXABI_1.3.2 + 0
 
 Relocation section '.rela.plt' at offset 0xdd48 contains 309 entries:
@@ -345,104 +345,104 @@
 00000000000b6040  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@GLIBCXX_3.4 + 0
 00000000000b6048  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyByteArray_AsString + 0
 00000000000b6050  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 strdup@GLIBC_2.2.5 + 0
 00000000000b6058  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_Create2 + 0
 00000000000b6060  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_begin_catch@CXXABI_1.3 + 0
 00000000000b6068  000001e700000007 R_X86_64_JUMP_SLOT     00000000000174e0 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev + 0
 00000000000b6070  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt9exceptionD2Ev@GLIBCXX_3.4 + 0
-00000000000b6078  000001b400000007 R_X86_64_JUMP_SLOT     00000000000272f0 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
-00000000000b6080  0000020500000007 R_X86_64_JUMP_SLOT     0000000000025c90 _ZNKSt9type_info9hash_codeEv + 0
-00000000000b6088  0000022f00000007 R_X86_64_JUMP_SLOT     0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
-00000000000b6090  000001cf00000007 R_X86_64_JUMP_SLOT     0000000000017860 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
+00000000000b6078  000001b200000007 R_X86_64_JUMP_SLOT     00000000000272f0 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
+00000000000b6080  0000020600000007 R_X86_64_JUMP_SLOT     0000000000025c90 _ZNKSt9type_info9hash_codeEv + 0
+00000000000b6088  0000023000000007 R_X86_64_JUMP_SLOT     0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
+00000000000b6090  000001ce00000007 R_X86_64_JUMP_SLOT     0000000000017860 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
 00000000000b6098  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetAttrString + 0
 00000000000b60a0  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyType_IsSubtype + 0
 00000000000b60a8  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 memmove@GLIBC_2.2.5 + 0
-00000000000b60b0  000001c100000007 R_X86_64_JUMP_SLOT     0000000000022760 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_ + 0
+00000000000b60b0  000001bf00000007 R_X86_64_JUMP_SLOT     0000000000022760 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_ + 0
 00000000000b60b8  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Fetch + 0
 00000000000b60c0  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyException_SetTraceback + 0
 00000000000b60c8  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 __assert_fail@GLIBC_2.2.5 + 0
-00000000000b60d0  000001be00000007 R_X86_64_JUMP_SLOT     0000000000016b10 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE + 0
+00000000000b60d0  000001bc00000007 R_X86_64_JUMP_SLOT     0000000000016b10 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE + 0
 00000000000b60d8  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_Copy + 0
-00000000000b60e0  000001ad00000007 R_X86_64_JUMP_SLOT     0000000000026b30 _ZNSt6vectorIbSaIbEE9push_backEb + 0
+00000000000b60e0  000001ab00000007 R_X86_64_JUMP_SLOT     0000000000026b30 _ZNSt6vectorIbSaIbEE9push_backEb + 0
 00000000000b60e8  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyThreadState_UncheckedGet + 0
-00000000000b60f0  000001b700000007 R_X86_64_JUMP_SLOT     0000000000013990 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi + 0
+00000000000b60f0  000001b500000007 R_X86_64_JUMP_SLOT     0000000000013990 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi + 0
 00000000000b60f8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c107SymBool10guard_boolEPKcl + 0
 00000000000b6100  0000001800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_Size + 0
 00000000000b6108  0000001900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaUnregisterFatBinary@libcudart.so.12 + 0
 00000000000b6110  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventDestroy@libcudart.so.12 + 0
 00000000000b6118  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda20getCurrentCUDAStreamEa + 0
 00000000000b6120  0000001c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c108SymFloat11guard_floatEPKcl + 0
 00000000000b6128  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail12infer_schema20make_function_schemaENS_8ArrayRefINS1_11ArgumentDefEEES4_ + 0
-00000000000b6130  000001fa00000007 R_X86_64_JUMP_SLOT     0000000000018470 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_ + 0
+00000000000b6130  000001fb00000007 R_X86_64_JUMP_SLOT     0000000000018470 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_ + 0
 00000000000b6138  0000002100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromString + 0
 00000000000b6140  0000002200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda29c10_cuda_check_implementationEiPKcS2_ib + 0
 00000000000b6148  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda17getStreamFromPoolEba + 0
 00000000000b6150  0000002600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c10ltERKNS_6SymIntEi + 0
 00000000000b6158  0000002700000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.12 + 0
 00000000000b6160  0000002800000007 R_X86_64_JUMP_SLOT     0000000000000000 memset@GLIBC_2.2.5 + 0
 00000000000b6168  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail14torchCheckFailEPKcS2_jS2_ + 0
 00000000000b6170  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt13runtime_errorC1EPKc + 0
-00000000000b6178  000001cb00000007 R_X86_64_JUMP_SLOT     0000000000023cc0 _Z24Padding_8_FP6_To_8_BytesPhS_ + 0
+00000000000b6178  000001ca00000007 R_X86_64_JUMP_SLOT     0000000000023cc0 _Z24Padding_8_FP6_To_8_BytesPhS_ + 0
 00000000000b6180  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt17rethrow_exceptionNSt15__exception_ptr13exception_ptrE@CXXABI_1.3.3 + 0
-00000000000b6188  000001f700000007 R_X86_64_JUMP_SLOT     0000000000017400 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv + 0
-00000000000b6190  0000016800000007 R_X86_64_JUMP_SLOT     0000000000026600 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev + 0
+00000000000b6188  000001f800000007 R_X86_64_JUMP_SLOT     0000000000017400 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv + 0
+00000000000b6190  0000016600000007 R_X86_64_JUMP_SLOT     0000000000026600 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev + 0
 00000000000b6198  0000003000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs4findEcm@GLIBCXX_3.4 + 0
 00000000000b61a0  0000003100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c106IValue23reportToTensorTypeErrorEv + 0
 00000000000b61a8  0000023a00000007 R_X86_64_JUMP_SLOT     0000000000013890 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi + 0
 00000000000b61b0  0000003200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs9push_backEc@GLIBCXX_3.4 + 0
-00000000000b61b8  000001b500000007 R_X86_64_JUMP_SLOT     000000000001f500 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_ + 0
+00000000000b61b8  000001b300000007 R_X86_64_JUMP_SLOT     000000000001f500 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_ + 0
 00000000000b61c0  0000003400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_WriteUnraisable + 0
 00000000000b61c8  0000003500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThread_tss_create + 0
 00000000000b61d0  0000003600000007 R_X86_64_JUMP_SLOT     0000000000000000 strlen@GLIBC_2.2.5 + 0
 00000000000b61d8  0000003700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt15__exception_ptr13exception_ptrC1ERKS0_@CXXABI_1.3.3 + 0
 00000000000b61e0  0000015800000007 R_X86_64_JUMP_SLOT     00000000000195a0 _Z13cast_fp16_fp6PtPh + 0
 00000000000b61e8  0000003900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_HasAttrString + 0
 00000000000b61f0  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_guard_abort@CXXABI_1.3 + 0
 00000000000b61f8  0000003c00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaStreamQuery@libcudart.so.12 + 0
 00000000000b6200  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinary@libcudart.so.12 + 0
 00000000000b6208  0000003e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c1010TensorType3getEv + 0
 00000000000b6210  0000003f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE + 0
 00000000000b6218  0000004000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda14ExchangeDeviceEa + 0
 00000000000b6220  0000004100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE + 0
 00000000000b6228  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt13runtime_errorD2Ev@GLIBCXX_3.4 + 0
-00000000000b6230  000001c900000007 R_X86_64_JUMP_SLOT     0000000000017630 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_ + 0
+00000000000b6230  000001c800000007 R_X86_64_JUMP_SLOT     0000000000017630 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_ + 0
 00000000000b6238  0000004400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops9to_device4callERKNS_6TensorEN3c106DeviceENS5_10ScalarTypeEbbSt8optionalINS5_12MemoryFormatEE + 0
 00000000000b6240  0000004500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_AsString + 0
-00000000000b6248  0000017900000007 R_X86_64_JUMP_SLOT     0000000000026730 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv + 0
+00000000000b6248  0000017700000007 R_X86_64_JUMP_SLOT     0000000000026730 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv + 0
 00000000000b6250  0000004600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs12_M_leak_hardEv@GLIBCXX_3.4 + 0
 00000000000b6258  0000004700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_S2_ + 0
 00000000000b6260  0000004800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSo9_M_insertImEERSoT_@GLIBCXX_3.4.9 + 0
 00000000000b6268  0000004900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt11_Hash_bytesPKvmm@CXXABI_1.3.5 + 0
 00000000000b6270  0000004a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs5rfindEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6278  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs17find_first_not_ofEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6280  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyByteArray_Size + 0
-00000000000b6288  000001c600000007 R_X86_64_JUMP_SLOT     00000000000201d0 _ZN2at8indexing11TensorIndexD1Ev + 0
+00000000000b6288  000001c500000007 R_X86_64_JUMP_SLOT     00000000000201d0 _ZN2at8indexing11TensorIndexD1Ev + 0
 00000000000b6290  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZdlPv@GLIBCXX_3.4 + 0
 00000000000b6298  0000004e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1EPKcmRKSaIcE@GLIBCXX_3.4 + 0
 00000000000b62a0  0000004f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_GetContext + 0
 00000000000b62a8  0000005000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE + 0
 00000000000b62b0  0000005100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE + 0
 00000000000b62b8  0000005200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendEPKcm@GLIBCXX_3.4 + 0
 00000000000b62c0  0000005300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs4swapERSs@GLIBCXX_3.4 + 0
 00000000000b62c8  0000005400000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyType_Lookup + 0
 00000000000b62d0  0000005500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_Clear + 0
 00000000000b62d8  0000005600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Clear + 0
-00000000000b62e0  0000020d00000007 R_X86_64_JUMP_SLOT     0000000000027630 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb + 0
+00000000000b62e0  0000020e00000007 R_X86_64_JUMP_SLOT     0000000000027630 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb + 0
 00000000000b62e8  0000005700000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_throw@CXXABI_1.3 + 0
 00000000000b62f0  0000005800000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaStreamSynchronize@libcudart.so.12 + 0
 00000000000b62f8  0000005900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_New + 0
 00000000000b6300  0000005a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Calloc + 0
 00000000000b6308  0000015e00000007 R_X86_64_JUMP_SLOT     000000000001f1a0 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_ + 0
 00000000000b6310  0000005b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb + 0
 00000000000b6318  0000005c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt20__throw_length_errorPKc@GLIBCXX_3.4 + 0
 00000000000b6320  0000005d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN5torch7LibraryC1ENS0_4KindESsSt8optionalIN3c1011DispatchKeyEEPKcj + 0
 00000000000b6328  0000005e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _Unwind_Resume@GCC_3.0 + 0
 00000000000b6330  0000005f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_Size + 0
 00000000000b6338  0000006000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda12device_countEv + 0
-00000000000b6340  0000020700000007 R_X86_64_JUMP_SLOT     0000000000023d80 _Z20BitInterleaving_2bitPh + 0
+00000000000b6340  0000020800000007 R_X86_64_JUMP_SLOT     0000000000023d80 _Z20BitInterleaving_2bitPh + 0
 00000000000b6348  0000006300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyType_Ready + 0
 00000000000b6350  0000006400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c105ErrorC2ENS_14SourceLocationESs + 0
 00000000000b6358  0000006500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt24__throw_out_of_range_fmtPKcz + 0
 00000000000b6360  0000006600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6assignERKSs@GLIBCXX_3.4 + 0
 00000000000b6368  0000006700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6assignEPKcm@GLIBCXX_3.4 + 0
 00000000000b6370  0000006800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_RKSs + 0
 00000000000b6378  0000006900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendERKSs@GLIBCXX_3.4 + 0
@@ -451,60 +451,60 @@
 00000000000b6390  0000006c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyObject_GetDictPtr + 0
 00000000000b6398  0000006d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at6Tensor5indexESt16initializer_listINS_8indexing11TensorIndexEE + 0
 00000000000b63a0  0000006e00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
 00000000000b63a8  0000006f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIlEEPT_v + 0
 00000000000b63b0  0000007000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_SetItem + 0
 00000000000b63b8  0000007100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThread_tss_get + 0
 00000000000b63c0  0000007200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Restore + 0
-00000000000b63c8  0000019100000007 R_X86_64_JUMP_SLOT     0000000000019740 _Z29weight_prepacking_fp16_to_fp6PtPhmm + 0
+00000000000b63c8  0000018f00000007 R_X86_64_JUMP_SLOT     0000000000019740 _Z29weight_prepacking_fp16_to_fp6PtPhmm + 0
 00000000000b63d0  0000024c00000007 R_X86_64_JUMP_SLOT     0000000000018a30 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE + 0
 00000000000b63d8  0000024b00000007 R_X86_64_JUMP_SLOT     0000000000016300 _ZN5torch7LibraryD1Ev + 0
 00000000000b63e0  0000007500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt15__exception_ptr13exception_ptr4swapERS0_@CXXABI_1.3.3 + 0
 00000000000b63e8  0000007600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNR5torch7Library5_implEPKcONS_11CppFunctionENS_17_RegisterOrVerifyE + 0
-00000000000b63f0  000001ae00000007 R_X86_64_JUMP_SLOT     0000000000026570 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_ + 0
+00000000000b63f0  000001ac00000007 R_X86_64_JUMP_SLOT     0000000000026570 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_ + 0
 00000000000b63f8  0000007700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1ERKSaIcE@GLIBCXX_3.4 + 0
 00000000000b6400  0000007800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda9GetDeviceEPa + 0
 00000000000b6408  0000007900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4 + 0
 00000000000b6410  0000007a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt15__exception_ptr13exception_ptrD1Ev@CXXABI_1.3.3 + 0
 00000000000b6418  0000007b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops12index_select4callERKNS_6TensorElS4_ + 0
 00000000000b6420  0000007c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThread_tss_alloc + 0
 00000000000b6428  0000007e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN6caffe28TypeMeta26error_unsupported_typemetaES0_ + 0
 00000000000b6430  0000008000000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaGetErrorString@libcudart.so.12 + 0
 00000000000b6438  0000008100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt13runtime_errorC1ERKSs@GLIBCXX_3.4 + 0
 00000000000b6440  0000008200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_ + 0
 00000000000b6448  0000014300000007 R_X86_64_JUMP_SLOT     0000000000018570 _ZN5torch8autograd13make_variableEN2at6TensorEbb + 0
-00000000000b6450  0000022700000007 R_X86_64_JUMP_SLOT     0000000000026470 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_ + 0
+00000000000b6450  0000022800000007 R_X86_64_JUMP_SLOT     0000000000026470 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_ + 0
 00000000000b6458  0000008300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9 + 0
 00000000000b6460  0000008600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1ERKSsmm@GLIBCXX_3.4 + 0
 00000000000b6468  0000008700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyGILState_GetThisThreadState + 0
 00000000000b6470  0000008800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_AsStringAndSize + 0
 00000000000b6478  0000008900000007 R_X86_64_JUMP_SLOT     0000000000000000 memcmp@GLIBC_2.2.5 + 0
-00000000000b6480  0000019600000007 R_X86_64_JUMP_SLOT     0000000000017480 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev + 0
+00000000000b6480  0000019400000007 R_X86_64_JUMP_SLOT     0000000000017480 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev + 0
 00000000000b6488  0000008a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_AsEncodedString + 0
 00000000000b6490  0000008b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs7compareEPKc@GLIBCXX_3.4 + 0
 00000000000b6498  0000008c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIN3c104HalfEEEPT_v + 0
 00000000000b64a0  0000008d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_New + 0
 00000000000b64a8  0000008e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_CallFunctionObjArgs + 0
 00000000000b64b0  0000008f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104impl23ExcludeDispatchKeyGuardC1ENS_14DispatchKeySetE + 0
 00000000000b64b8  0000009000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIhEEPT_v + 0
 00000000000b64c0  0000009100000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventSynchronize@libcudart.so.12 + 0
 00000000000b64c8  0000009200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda20getDefaultCUDAStreamEa + 0
-00000000000b64d0  000001af00000007 R_X86_64_JUMP_SLOT     00000000000242a0 _Z24weight_matrix_prepackingPiS_mm + 0
-00000000000b64d8  000001b300000007 R_X86_64_JUMP_SLOT     00000000000162b0 _ZNK3c1010TensorImpl6deviceEv + 0
-00000000000b64e0  0000022200000007 R_X86_64_JUMP_SLOT     0000000000026770 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb + 0
+00000000000b64d0  000001ad00000007 R_X86_64_JUMP_SLOT     00000000000242a0 _Z24weight_matrix_prepackingPiS_mm + 0
+00000000000b64d8  000001b100000007 R_X86_64_JUMP_SLOT     00000000000162b0 _ZNK3c1010TensorImpl6deviceEv + 0
+00000000000b64e0  0000022300000007 R_X86_64_JUMP_SLOT     0000000000026770 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb + 0
 00000000000b64e8  0000009300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c10lsERSoNS_10DeviceTypeE + 0
 00000000000b64f0  0000013a00000007 R_X86_64_JUMP_SLOT     000000000002b580 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm + 0
 00000000000b64f8  0000009600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev + 0
 00000000000b6500  0000009700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Occurred + 0
 00000000000b6508  0000009800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_DeleteCurrent + 0
 00000000000b6510  0000015300000007 R_X86_64_JUMP_SLOT     00000000000172b0 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
 00000000000b6518  0000009900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIiEEPT_v + 0
 00000000000b6520  0000009a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventRecord@libcudart.so.12 + 0
 00000000000b6528  0000009b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyWeakref_NewRef + 0
-00000000000b6530  0000021c00000007 R_X86_64_JUMP_SLOT     000000000002b6b0 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs + 0
+00000000000b6530  0000021d00000007 R_X86_64_JUMP_SLOT     000000000002b6b0 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs + 0
 00000000000b6538  0000009d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1EPKcRKSaIcE@GLIBCXX_3.4 + 0
 00000000000b6540  0000009e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs7reserveEm@GLIBCXX_3.4 + 0
 00000000000b6548  0000009f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaFuncSetAttribute@libcudart.so.12 + 0
 00000000000b6550  000000a000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_AsUTF8String + 0
 00000000000b6558  000000a100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_GetBuiltins + 0
 00000000000b6560  000000a400000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
 00000000000b6568  000000a500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs7replaceEmmPKcm@GLIBCXX_3.4 + 0
@@ -515,19 +515,19 @@
 00000000000b6590  000000aa00000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
 00000000000b6598  000000ab00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventCreateWithFlags@libcudart.so.12 + 0
 00000000000b65a0  000000ae00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendEmc@GLIBCXX_3.4 + 0
 00000000000b65a8  000000af00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_GetName + 0
 00000000000b65b0  000000b000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendERKSsmm@GLIBCXX_3.4 + 0
 00000000000b65b8  000000b100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt17__throw_bad_allocv@GLIBCXX_3.4 + 0
 00000000000b65c0  000000b200000007 R_X86_64_JUMP_SLOT     0000000000000000 _Znwm@GLIBCXX_3.4 + 0
-00000000000b65c8  000001f500000007 R_X86_64_JUMP_SLOT     0000000000026520 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_ + 0
+00000000000b65c8  000001f600000007 R_X86_64_JUMP_SLOT     0000000000026520 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_ + 0
 00000000000b65d0  000000b500000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 00000000000b65d8  000000b600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEED1Ev@GLIBCXX_3.4 + 0
-00000000000b65e0  000001ab00000007 R_X86_64_JUMP_SLOT     0000000000016870 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_ + 0
-00000000000b65e8  0000018400000007 R_X86_64_JUMP_SLOT     0000000000016dc0 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_ + 0
+00000000000b65e0  000001a900000007 R_X86_64_JUMP_SLOT     0000000000016870 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_ + 0
+00000000000b65e8  0000018200000007 R_X86_64_JUMP_SLOT     0000000000016dc0 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_ + 0
 00000000000b65f0  000000bb00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCMethod_New + 0
 00000000000b65f8  000000bc00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaGetLastError@libcudart.so.12 + 0
 00000000000b6600  000000bd00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c1017SymbolicShapeMeta18init_is_contiguousEv + 0
 00000000000b6608  000000bf00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyException_SetContext + 0
 00000000000b6610  000000c000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyGILState_Ensure + 0
 00000000000b6618  000000c100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_AcquireThread + 0
 00000000000b6620  000000c200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_SetString + 0
@@ -564,85 +564,85 @@
 00000000000b6718  000000e600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSt15basic_stringbufIcSt11char_traitsIcESaIcEE3strEv@GLIBCXX_3.4 + 0
 00000000000b6720  000000e700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs9_M_mutateEmmm@GLIBCXX_3.4 + 0
 00000000000b6728  000000e800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_GetPointer + 0
 00000000000b6730  000000e900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c1010TensorImpl17set_autograd_metaESt10unique_ptrINS_21AutogradMetaInterfaceESt14default_deleteIS2_EE + 0
 00000000000b6738  0000014000000007 R_X86_64_JUMP_SLOT     000000000001f090 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED1Ev + 0
 00000000000b6740  000000eb00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_guard_release@CXXABI_1.3 + 0
 00000000000b6748  000000ec00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventQuery@libcudart.so.12 + 0
-00000000000b6750  0000018800000007 R_X86_64_JUMP_SLOT     0000000000023ee0 _Z20BitInterleaving_4bitPh + 0
+00000000000b6750  0000018600000007 R_X86_64_JUMP_SLOT     0000000000023ee0 _Z20BitInterleaving_4bitPh + 0
 00000000000b6758  000000ed00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@GLIBCXX_3.4 + 0
 00000000000b6760  000000ee00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c107WarningC1ESt7variantIJNS0_11UserWarningENS0_18DeprecationWarningEEERKNS_14SourceLocationESsb + 0
 00000000000b6768  000000ef00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.12 + 0
 00000000000b6770  000000f000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyInstanceMethod_New + 0
 00000000000b6778  000000f200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_New + 0
 00000000000b6780  000000f300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_SetPointer + 0
 00000000000b6788  000001e500000007 R_X86_64_JUMP_SLOT     00000000000169d0 _ZN3c106IValue7destroyEv + 0
 00000000000b6790  000000f500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyGILState_Release + 0
 00000000000b6798  000000f600000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventElapsedTime@libcudart.so.12 + 0
 00000000000b67a0  000000f700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSspLEPKc@GLIBCXX_3.4 + 0
 00000000000b67a8  000000f900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_baseD2Ev@GLIBCXX_3.4 + 0
 00000000000b67b0  000000fa00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6insertEmPKcm@GLIBCXX_3.4 + 0
-00000000000b67b8  000001f900000007 R_X86_64_JUMP_SLOT     0000000000023d40 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh + 0
-00000000000b67c0  0000016700000007 R_X86_64_JUMP_SLOT     00000000000197f0 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_ + 0
+00000000000b67b8  000001fa00000007 R_X86_64_JUMP_SLOT     0000000000023d40 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh + 0
+00000000000b67c0  0000016500000007 R_X86_64_JUMP_SLOT     00000000000197f0 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_ + 0
 00000000000b67c8  000000fb00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIfEEPT_v + 0
 00000000000b67d0  000000fc00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops10empty_like4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbES5_INS6_12MemoryFormatEE + 0
 00000000000b67d8  000000fd00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs4_Rep9_S_createEmmRKSaIcE@GLIBCXX_3.4 + 0
 00000000000b67e0  000000fe00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetItem + 0
-00000000000b67e8  0000019000000007 R_X86_64_JUMP_SLOT     0000000000018d20 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
+00000000000b67e8  0000018e00000007 R_X86_64_JUMP_SLOT     0000000000018d20 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
 00000000000b67f0  0000010000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt6localeC1Ev@GLIBCXX_3.4 + 0
-00000000000b67f8  0000021100000007 R_X86_64_JUMP_SLOT     0000000000025230 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_ + 0
+00000000000b67f8  0000021200000007 R_X86_64_JUMP_SLOT     0000000000025230 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_ + 0
 00000000000b6800  0000014800000007 R_X86_64_JUMP_SLOT     0000000000023850 _ZNSt6vectorIN3c108ArgumentESaIS1_EED1Ev + 0
 00000000000b6808  0000010100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c10neERKNS_6SymIntEi + 0
-00000000000b6810  000001c300000007 R_X86_64_JUMP_SLOT     00000000000184f0 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_ + 0
+00000000000b6810  000001c200000007 R_X86_64_JUMP_SLOT     00000000000184f0 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_ + 0
 00000000000b6818  0000010300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_end_catch@CXXABI_1.3 + 0
-00000000000b6820  000001a400000007 R_X86_64_JUMP_SLOT     0000000000023d60 _Z31Extract_4_Bits_From_2_PaddedFP6hh + 0
+00000000000b6820  000001a200000007 R_X86_64_JUMP_SLOT     0000000000023d60 _Z31Extract_4_Bits_From_2_PaddedFP6hh + 0
 00000000000b6828  0000010400000007 R_X86_64_JUMP_SLOT     0000000000000000 strcmp@GLIBC_2.2.5 + 0
 00000000000b6830  0000010500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda9SetDeviceEa + 0
 00000000000b6838  0000010600000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_rethrow@CXXABI_1.3 + 0
 00000000000b6840  0000025300000007 R_X86_64_JUMP_SLOT     0000000000016f20 _ZN3c1020intrusive_ptr_targetD2Ev + 0
 00000000000b6848  0000024a00000007 R_X86_64_JUMP_SLOT     0000000000023fa0 _Z25Assign_32_FP6_To_4_ThreadPSt6vectorIhSaIhEES2_PhS3_S3_S3_ + 0
-00000000000b6850  0000016b00000007 R_X86_64_JUMP_SLOT     0000000000026da0 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_ + 0
+00000000000b6850  0000016900000007 R_X86_64_JUMP_SLOT     0000000000026da0 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_ + 0
 00000000000b6858  0000010800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs4findEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6860  0000023d00000007 R_X86_64_JUMP_SLOT     0000000000018e00 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE + 0
 00000000000b6868  0000010900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFunction@libcudart.so.12 + 0
 00000000000b6870  0000015600000007 R_X86_64_JUMP_SLOT     00000000000178b0 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev + 0
-00000000000b6878  000001b000000007 R_X86_64_JUMP_SLOT     0000000000025370 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
+00000000000b6878  000001ae00000007 R_X86_64_JUMP_SLOT     0000000000025370 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
 00000000000b6880  0000010a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c107IntType3getEv + 0
 00000000000b6888  0000010b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_GetBack + 0
 00000000000b6890  0000010c00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.12 + 0
 00000000000b6898  0000010f00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_free_exception@CXXABI_1.3 + 0
 00000000000b68a0  0000015900000007 R_X86_64_JUMP_SLOT     00000000000264d0 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_OS6_ + 0
 00000000000b68a8  0000011000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail14torchCheckFailEPKcS2_jRKSs + 0
 00000000000b68b0  0000011100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda14MaybeSetDeviceEa + 0
 00000000000b68b8  0000011200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_SaveThread + 0
-00000000000b68c0  0000020100000007 R_X86_64_JUMP_SLOT     00000000000179e0 _ZN3c1014FunctionSchemaD1Ev + 0
+00000000000b68c0  0000020200000007 R_X86_64_JUMP_SLOT     00000000000179e0 _ZN3c1014FunctionSchemaD1Ev + 0
 00000000000b68c8  000001d100000007 R_X86_64_JUMP_SLOT     0000000000018b50 _ZNSt6vectorIN3c106IValueESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
 00000000000b68d0  0000011300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_GetCode + 0
 00000000000b68d8  0000011500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail19maybe_wrap_dim_slowIlEET_S2_S2_b + 0
 00000000000b68e0  0000011600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_SetContext + 0
 00000000000b68e8  0000011700000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaLaunchKernel@libcudart.so.12 + 0
 00000000000b68f0  000001d500000007 R_X86_64_JUMP_SLOT     000000000001ee50 _ZNK2at10TensorBase7optionsEv + 0
 00000000000b68f8  0000011800000007 R_X86_64_JUMP_SLOT     0000000000000000 Py_GetVersion + 0
 00000000000b6900  0000011900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs16find_last_not_ofEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6908  0000011a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GC_UnTrack + 0
 00000000000b6910  0000011b00000007 R_X86_64_JUMP_SLOT     0000000000000000 __dynamic_cast@CXXABI_1.3 + 0
 00000000000b6918  0000011c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt6localeD1Ev@GLIBCXX_3.4 + 0
-00000000000b6920  0000018b00000007 R_X86_64_JUMP_SLOT     0000000000021ff0 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_ + 0
+00000000000b6920  0000018900000007 R_X86_64_JUMP_SLOT     0000000000021ff0 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_ + 0
 00000000000b6928  0000011d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_baseC2Ev@GLIBCXX_3.4 + 0
 00000000000b6930  0000011e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 + 0
 00000000000b6938  0000011f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c104cuda10CUDAStream6streamEv + 0
 00000000000b6940  0000012100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GetAttrString + 0
 00000000000b6948  0000012200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyException_SetCause + 0
 00000000000b6950  0000012400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm@GLIBCXX_3.4.18 + 0
-00000000000b6958  0000019d00000007 R_X86_64_JUMP_SLOT     000000000001b1c0 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_ + 0
+00000000000b6958  0000019b00000007 R_X86_64_JUMP_SLOT     000000000001b1c0 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_ + 0
 00000000000b6960  0000012500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Str + 0
 00000000000b6968  0000012600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c109FloatType3getEv + 0
 00000000000b6970  0000012700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_GetItemWithError + 0
 00000000000b6978  0000012800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Format + 0
 00000000000b6980  0000012900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104impl23ExcludeDispatchKeyGuardD1Ev + 0
 00000000000b6988  0000012a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c106SymInt9guard_intEPKcl + 0
 00000000000b6990  0000015500000007 R_X86_64_JUMP_SLOT     0000000000020930 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE + 0
-00000000000b6998  0000017b00000007 R_X86_64_JUMP_SLOT     0000000000018410 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
+00000000000b6998  0000017900000007 R_X86_64_JUMP_SLOT     0000000000018410 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
 00000000000b69a0  0000012c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt9terminatev@GLIBCXX_3.4 + 0
 00000000000b69a8  0000012d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_AsUTF8AndSize + 0
 00000000000b69b0  0000012e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_Size + 0
 00000000000b69b8  0000012f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda21warn_or_error_on_syncEv + 0
```

### readelf --wide --dynamic {}

```diff
@@ -9,15 +9,15 @@
  0x0000000000000001 (NEEDED)             Shared library: [libc10_cuda.so]
  0x0000000000000001 (NEEDED)             Shared library: [libtorch_cuda.so]
  0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libm.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libgcc_s.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libpthread.so.0]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
- 0x000000000000000f (RPATH)              Library rpath: [/__w/_temp/conda_environment_9200202766/lib]
+ 0x000000000000000f (RPATH)              Library rpath: [/__w/_temp/conda_environment_9216653705/lib]
  0x000000000000000c (INIT)               0x10000
  0x000000000000000d (FINI)               0x32c5c
  0x0000000000000019 (INIT_ARRAY)         0xb5318
  0x000000000000001b (INIT_ARRAYSZ)       88 (bytes)
  0x000000000000001a (FINI_ARRAY)         0xb5370
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x260
```

### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 93c816f2b36726e3bdc7cf3e247c1d32d3857af2
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 6403fde4781da3e9a42afdbd43debd85d3a4b897
```

### strings --all --bytes=8 {}

```diff
@@ -306,17 +306,17 @@
 _ZN3c104cuda20getDefaultCUDAStreamEa
 _ZNK3c1010TensorImpl11size_customEl
 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
 _ZN3c109FloatType3getEv
 _ZN3c1014getTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
 cudaEventQuery
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
 _ZN3c1010ValueErrorD2Ev
 _ZTVN3c105ErrorE
 _ZNSt9exceptionD2Ev
 _ZN3c1010ValueErrorD1Ev
 _ZN3c1010ValueErrorD0Ev
 _ZN3c1014DispatchKeySetC2ENS_11DispatchKeyE
 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
@@ -361,15 +361,15 @@
 cudaStreamQuery
 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
 _ZZN3c104cuda13warning_stateEvE14warning_state_
 cudaStreamSynchronize
 _ZN3c104cuda21warn_or_error_on_syncEv
 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d
 _ZTVN3c104cuda4impl13CUDAGuardImplE
 _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb
 _ZN2at4_ops12index_select4callERKNS_6TensorElS4_
 _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE
 _ZN2at4_ops15to_dtype_layout4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbEbbS5_INS6_12MemoryFormatEE
 _ZNK2at10TensorBase8data_ptrIlEEPT_v
 _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_
@@ -602,15 +602,15 @@
 GLIBCXX_3.4.18
 CXXABI_1.3.2
 CXXABI_1.3.5
 GLIBCXX_3.4.9
 CXXABI_1.3.3
 CXXABI_1.3
 GLIBCXX_3.4
-/__w/_temp/conda_environment_9200202766/lib
+/__w/_temp/conda_environment_9216653705/lib
 AVAUATUSH
 []A\A]A^A_
 AVAUATUSH
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATUSH
@@ -727,15 +727,15 @@
 ([]A\A]A^A_
 ([]A\A]A^A_
 AWAVAUATI
 []A\A]A^A_
 D$ H9D$Xu
 AWAVAUATUSH
 []A\A]A^A_
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/SymNodeImpl.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/SymNodeImpl.h
 has_hint
 guard_float
 guard_bool
 guard_int
 wrap_bool
 wrap_float
 wrap_int
@@ -746,15 +746,15 @@
 is_channels_last_contiguous_3d
 is_channels_last_contiguous_2d
 is_contiguous
 floordiv
 is_float
 tensor does not have a device
 device_default
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
 cudaError_t fp6_linear_kernel(cudaStream_t, const uint4*, const half*, const half*, half*, size_t, size_t, size_t, float*, int)
 /__w/ao/ao/pytorch/ao/torchao/csrc/cuda/fp6_llm/fp6_linear.cu
 FP6LLM_API Error: Unsupported N dimension %d!
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
@@ -778,60 +778,60 @@
 PyObject
 Uninitialized
 Quantizer
 Generator
 InvalidTag(
 unexpected tag 
 isIntrusivePtr
-static_cast<uint32_t>(tag) < kNumTags INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":1315, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
+static_cast<uint32_t>(tag) < kNumTags INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":1315, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
 TTarget violates the invariant that refcount > 0  =>  weakcount > 0
-owning_ptr == NullType::singleton() || owning_ptr->refcount_.load() == 0 || owning_ptr->weakcount_.load() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":483, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h
+owning_ptr == NullType::singleton() || owning_ptr->refcount_.load() == 0 || owning_ptr->weakcount_.load() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":483, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h
 Operators taking TensorOptions cannot take a TensorOptions with options.requires_grad set as true. This isn't implemented yet.
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
 check_tensor_options_and_extract_memory_format
 Cannot set memory_format both in TensorOptions and explicit argument; please delete the redundant setter.
 IntArrayRef contains an int that cannot be represented as a SymInt: 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
 created ArrayRef with nullptr and non-zero length! std::optional relies on this being illegal
-Data != nullptr || Length == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h":62, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
+Data != nullptr || Length == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h":62, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
 fromIntArrayRefSlow
 debugCheckNullptrInvariant
 Tried to destruct an intrusive_ptr_target that still has intrusive_ptr to it; refcount was 
-refcount_.load() == 0 || refcount_.load() >= detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":118, please report a bug to PyTorch. 
+refcount_.load() == 0 || refcount_.load() >= detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":118, please report a bug to PyTorch. 
 Tried to destruct an intrusive_ptr_target that still has weak_intrusive_ptr to it
-weakcount_.load() == 1 || weakcount_.load() == 0 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount - 1 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":133, please report a bug to PyTorch. 
+weakcount_.load() == 1 || weakcount_.load() == 0 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount - 1 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":133, please report a bug to PyTorch. 
 ~intrusive_ptr_target
-self_impl INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
+self_impl INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
 Only Tensors of floating point and complex dtype can require gradients
 AutogradMeta
 set_requires_grad
 intrusive_ptr: Newly-created target had non-zero refcounts. Does its constructor do something strange like incref or create an intrusive_ptr from `this`?
-target_->refcount_ == 0 && target_->weakcount_ == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":319, please report a bug to PyTorch. 
+target_->refcount_ == 0 && target_->weakcount_ == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":319, please report a bug to PyTorch. 
 intrusive_ptr
 TensorImpl with nullptr is not supported
 intrusive_ptr: Cannot increase refcount after it reached zero.
-new_refcount != 1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":274, please report a bug to PyTorch. 
+new_refcount != 1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":274, please report a bug to PyTorch. 
 vector::_M_realloc_insert
 expected int
-0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
+0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
 N3c1020intrusive_ptr_targetE
 N3c1011SymNodeImplE
 N3c1015VariableVersion14VersionCounterE
 N3c1014OperatorKernelE
 N3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
 FN2at6TensorES0_S0_S0_lE
 Input value out of range for FP6.
 void DeQuantMatrix_FP6_To_FP16(half*, unsigned char*, size_t, size_t, half*)
 /__w/ao/ao/pytorch/ao/torchao/csrc/cuda/fp6_llm/weight_quant.cu
 _ZN46_INTERNAL_4c03c64a_15_weight_quant_cu_f5655ced6thrust6system6detail10sequential3seqE
-extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
+extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
 Expected fp6_tensor.size(1) % 3 == 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected fp16_scale.size(0) == OC to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 (K * 6 % 8) should be 0
 weight must be 2-dimensional
 fp16_to_fp6_cpu
 weight must be FP16
 symbolic_shape_meta
@@ -861,63 +861,63 @@
 scores must be a CUDA tensor
 dimension 0, got 
 CUDAGuardImpl
 " not implemented for '
 operator()
 slice step cannot be zero
 torchao::nms
-d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":53, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h
+d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":53, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h
 setDevice
 Both events must be recorded before calculating elapsed time.
 elapsedTime
 Expected stream_.device_type() == DeviceType::CUDA to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAStream.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAStream.h
 CUDAStream
 synchronizeEvent
 queryEvent
 There is an error in the layout calculation logic.
-is_mkldnn() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-_ZN41_INTERNAL_5b2e9259_6_nms_cu_1b1d7d0e_22006thrust6system6detail10sequential3seqE
-is_heap_allocated() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h":89, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
+is_mkldnn() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+_ZN41_INTERNAL_5b2e9259_6_nms_cu_15b95e91_25866thrust6system6detail10sequential3seqE
+is_heap_allocated() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h":89, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
 /__w/ao/ao/pytorch/ao/torchao/csrc/cuda/nms.cu
 boxes should be a 2d tensor, got 
 boxes should have 4 elements in dimension 1, got 
 scores should be a 1d tensor, got 
 boxes and scores should have same number of elements in 
-t == DeviceType::CUDA INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":28, please report a bug to PyTorch. 
+t == DeviceType::CUDA INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":28, please report a bug to PyTorch. 
 cannot create std::vector larger than max_size()
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/ATen/TensorIndexing.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/ATen/TensorIndexing.h
 getDevice
 validate
 Device index must be -1 or non-negative, got 
-index_ >= -1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/Device.h":177, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/Device.h
-d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":34, please report a bug to PyTorch. 
+index_ >= -1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/Device.h":177, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/Device.h
+d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":34, please report a bug to PyTorch. 
 exchangeDevice
 Event device index 
 createEvent
  does not match recording stream's device index 
 CUDA event received unknown flag
 CUDA warning: 
 uncheckedSetDevice
 destroyEvent
  devices
 getDeviceGuardImpl
 PyTorch is not linked with support for 
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
 stream_synchronize
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAFunctions.h
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAFunctions.h
 Expected ptr_->is_float() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
-0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9200202766/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
+0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9216653705/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
 expected double
 toDouble
 N3c1010ValueErrorE
 N3c104impl24DeviceGuardImplInterfaceE
 N3c104cuda4impl13CUDAGuardImplE
 N3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
 FN2at6TensorERKS0_S2_dE
@@ -1402,113 +1402,113 @@
 .nv.global
 _ZN46_INTERNAL_4c03c64a_15_weight_quant_cu_f5655ced6thrust6system6detail10sequential3seqE
 .debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-_ZN41_INTERNAL_5b2e9259_6_nms_cu_1b1d7d0e_22006thrust6system6detail10sequential3seqE
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
+_ZN41_INTERNAL_5b2e9259_6_nms_cu_15b95e91_25866thrust6system6detail10sequential3seqE
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-_ZN41_INTERNAL_5b2e9259_6_nms_cu_1b1d7d0e_22006thrust6system6detail10sequential3seqE
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
+_ZN41_INTERNAL_5b2e9259_6_nms_cu_15b95e91_25866thrust6system6detail10sequential3seqE
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 GCC: (GNU) 9.3.1 20200408 (Red Hat 9.3.1-2)
 GCC: (GNU) 4.8.5 20150623 (Red Hat 4.8.5-44)
-tmpxft_00000875_00000000-6_fp6_linear.compute_86.cudafe1.cpp
+tmpxft_000009f7_00000000-6_fp6_linear.compute_86.cudafe1.cpp
 fatbinData
 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmi
 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
 _ZL26__cudaUnregisterBinaryUtilv
 _ZL20__cudaFatCubinHandle
 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmi.constprop.0
@@ -1528,32 +1528,32 @@
 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
 _ZL24__sti____cudaRegisterAllv
 _ZL15__fatDeviceText
 _ZN6thrust6system6detail10sequentialL3seqE
 _ZN3c10L45autograd_dispatch_keyset_with_ADInplaceOrViewE
 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l.cold
-_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp
 _ZStL8__ioinit
 _ZN7torchaoL45TORCH_LIBRARY_IMPL_static_init_torchao_CUDA_2E
-_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
-tmpxft_00000876_00000000-6_weight_quant.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
+tmpxft_000009f8_00000000-6_weight_quant.compute_86.cudafe1.cpp
 _Z13cast_fp16_fp6PtPh.cold
 _Z29weight_prepacking_fp16_to_fp6PtPhmm.cold
 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE.cold
 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_.cold
-_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp
 _ZN7torchaoL44TORCH_LIBRARY_IMPL_static_init_torchao_CPU_2E
-_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
-tmpxft_00000877_00000000-6_nms.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
+tmpxft_000009f9_00000000-6_nms.compute_86.cudafe1.cpp
 _ZN3c10L8toStringENS_10ScalarTypeE
 _ZN3c106SymInt8release_Ev.part.0
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d.cold
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d.cold
+_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold
 _GLOBAL__sub_I_fp6_llm.cpp
 _ZL44TORCH_LIBRARY_FRAGMENT_static_init_torchao_2
 _GLOBAL__sub_I_fp6_llm.cpp.cold
 _Z24weight_matrix_prepackingPiS_mm.cold
 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE.cold
 _GLOBAL__sub_I_weight_prepacking.cpp
 _GLOBAL__sub_I_weight_prepacking.cpp.cold
@@ -1733,14 +1733,15 @@
 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZNSt9exceptionD2Ev@GLIBCXX_3.4
 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
 PyByteArray_Type
 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZNK3c106IValue7tagKindEv
 _ZNK3c104impl16VirtualGuardImpl9getStreamENS_6DeviceE
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIdEEvidPKT_Py
 _ZNKSt9type_info9hash_codeEv
 _ZN3c1020intrusive_ptr_targetD1Ev
 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
 PyObject_SetAttrString
 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
 PyType_IsSubtype
 memmove@GLIBC_2.2.5
@@ -1751,15 +1752,14 @@
 PyErr_Fetch
 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_
 PyException_SetTraceback
 _ZN3c1011SymNodeImpl12constant_intEv
 __assert_fail@GLIBC_2.2.5
 _ZN3c1011SymNodeImpl28is_non_overlapping_and_denseENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
 PyExc_RuntimeError
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIdEEvidPKT_Py
 _ZN3c1011SymNodeImpl9wrap_boolEb
 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a
 PyDict_Copy
 _ZNSt6vectorIbSaIbEE9push_backEb
 _PyThreadState_UncheckedGet
@@ -1815,14 +1815,15 @@
 _Z13cast_fp16_fp6PtPh
 _ZTSN3c1014OperatorKernelE
 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3
 PyObject_HasAttrString
 _ZTVSt9bad_alloc@GLIBCXX_3.4
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 __cxa_guard_abort@CXXABI_1.3
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIN3c104HalfEEEvidPKT_Py
 cudaStreamQuery@libcudart.so.12
 __cudaRegisterFatBinary@libcudart.so.12
 _ZN3c1010TensorType3getEv
 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
 _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE
 _ZN3c104cuda14ExchangeDeviceEa
 _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE
@@ -2005,15 +2006,14 @@
 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm
 PyExc_ImportError
 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZNK3c1011SymNodeImpl13is_nested_intEv
 _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev
 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
 PyErr_Occurred
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIN3c104HalfEEEvidPKT_Py
 PyThreadState_DeleteCurrent
 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
 _ZNK2at10TensorBase8data_ptrIiEEPT_v
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
 _ZTIFN2at6TensorES0_E
 cudaEventRecord@libcudart.so.12
 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
@@ -2152,14 +2152,15 @@
 _ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@GLIBCXX_3.4
 _ZN3c107WarningC1ESt7variantIJNS0_11UserWarningENS0_18DeprecationWarningEEERKNS_14SourceLocationESsb
 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE
 __cudaRegisterFatBinaryEnd@libcudart.so.12
 PyInstanceMethod_New
 _ZN3c1011SymNodeImpl11is_constantEv
 __gxx_personality_v0@CXXABI_1.3
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258610nms_kernelERKN2at6TensorES4_d
 _ZNK3c104impl16VirtualGuardImpl4typeEv
 _ZN3c1011SymNodeImpl8wrap_intEl
 _ZN3c1011SymNodeImplD1Ev
 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi
 PyDict_New
 _ZN3c1015VariableVersion14VersionCounterD2Ev
@@ -2216,15 +2217,14 @@
 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev
 _ZTSN3c104cuda4impl13CUDAGuardImplE
 _ZN3c104impl16VirtualGuardImplD2Ev
 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
 _ZN3c107IntType3getEv
 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 PyFrame_GetBack
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220010nms_kernelERKN2at6TensorES4_d
 __cudaPopCallConfiguration@libcudart.so.12
 PyExc_IndexError
 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3
 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l
 __cxa_free_exception@CXXABI_1.3
 _ZNSt19bad_optional_accessD0Ev
@@ -2274,15 +2274,14 @@
 _ZNK3c104impl16VirtualGuardImpl11deviceCountEv
 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_
 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l
 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC2EPS1_
 _ZN3c1011SymNodeImpl9sym_floatEv
 PyObject_Str
 _ZN3c109FloatType3getEv
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_1b1d7d0e_220015nms_kernel_implIfEEvidPKT_Py
 PyDict_GetItemWithError
 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
 PyErr_Format
 _ZN3c106detail12_str_wrapperIJPKcRKSsEE4callERKS3_S5_
 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
 _ZTSN3c1020intrusive_ptr_targetE
 _ZN3c104impl23ExcludeDispatchKeyGuardD1Ev
@@ -2292,14 +2291,15 @@
 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
 _ZTIN3c105ErrorE
 _ZSt9terminatev@GLIBCXX_3.4
 PyUnicode_AsUTF8AndSize
 PyTuple_Size
 _ZNK3c1010TensorImpl11size_customEl
 _ZN3c1014OperatorKernelD2Ev
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_15b95e91_258615nms_kernel_implIfEEvidPKT_Py
 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
 _ZN3c1014getTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
 _ZN3c104cuda21warn_or_error_on_syncEv
 _ZN3c104cuda4impl13CUDAGuardImplD2Ev
 _ZN2at8indexing11TensorIndexD2Ev
 _ZTISt11range_error@GLIBCXX_3.4
 .shstrtab
```

### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,82 +1,82 @@
 
 Hex dump of section '.gnu.hash':
   0x00000260 07010000 31010000 20000000 0b000000 ....1... .......
   0x00000270 0002a400 81000010 08900400 89b68001 ................
   0x00000280 2c080000 e8840003 00800001 e4050404 ,...............
   0x00000290 848c81b7 40120050 404b8971 90310808 ....@..P@K.q.1..
-  0x000002a0 0340000c 5888844c 6243a419 1c274311 .@..X..LbC...'C.
+  0x000002a0 0340000c 58c8a44c 6243a419 1c274311 .@..X..LbC...'C.
   0x000002b0 b1810100 00088004 8aa80411 70040110 ............p...
   0x000002c0 03a9390c 2c8cd424 1602d0c1 c0326ba0 ..9.,..$.....2k.
   0x000002d0 0884d69b 84200a23 02400a42 01608005 ..... .#.@.B.`..
-  0x000002e0 721d0a96 83885808 10801010 400e141c r.....X.....@...
-  0x000002f0 00042000 80012210 1321d848 36880042 .. ..."..!.H6..B
-  0x00000300 30800000 e00881c3 1382e1c3 4100032b 0...........A..+
+  0x000002e0 721d0a96 83885808 10801010 400e041c r.....X.....@...
+  0x000002f0 00042000 80012210 1321d848 368880c2 .. ..."..!.H6...
+  0x00000300 30800000 e00881c3 0302e181 4100032b 0...........A..+
   0x00000310 000c8125 05583404 18980888 12815810 ...%.X4.......X.
   0x00000320 00200002 30240211 20c81000 1c80c608 . ..0$.. .......
   0x00000330 4c800058 01963001 01030260 50188080 L..X..0....`P...
-  0x00000340 10102005 20a18250 0c482100 81158000 .. . ..P.H!.....
+  0x00000340 10102005 20a18250 0c486100 85158000 .. . ..P.Ha.....
   0x00000350 b402cb82 801642e4 12808302 44282062 ......B.....D( b
-  0x00000360 da80400c 6b0e328d 04104209 00002080 ..@.k.2...B... .
+  0x00000360 9a80400c 6b0e328d 04104209 00002080 ..@.k.2...B... .
   0x00000370 31010000 36010000 00000000 38010000 1...6.......8...
   0x00000380 3a010000 00000000 00000000 00000000 :...............
   0x00000390 3c010000 3d010000 40010000 41010000 <...=...@...A...
   0x000003a0 00000000 00000000 00000000 42010000 ............B...
   0x000003b0 43010000 44010000 00000000 45010000 C...D.......E...
   0x000003c0 46010000 49010000 00000000 00000000 F...I...........
   0x000003d0 4a010000 4c010000 4d010000 4f010000 J...L...M...O...
   0x000003e0 52010000 53010000 55010000 00000000 R...S...U.......
   0x000003f0 56010000 57010000 58010000 5a010000 V...W...X...Z...
   0x00000400 5c010000 5e010000 00000000 00000000 \...^...........
-  0x00000410 60010000 62010000 00000000 63010000 `...b.......c...
-  0x00000420 64010000 66010000 68010000 6a010000 d...f...h...j...
-  0x00000430 6c010000 00000000 6d010000 6e010000 l.......m...n...
-  0x00000440 70010000 71010000 72010000 00000000 p...q...r.......
-  0x00000450 00000000 74010000 00000000 00000000 ....t...........
-  0x00000460 76010000 00000000 79010000 7a010000 v.......y...z...
-  0x00000470 7c010000 7e010000 81010000 82010000 |...~...........
-  0x00000480 87010000 89010000 8a010000 00000000 ................
-  0x00000490 8b010000 8c010000 00000000 8f010000 ................
-  0x000004a0 91010000 92010000 93010000 00000000 ................
-  0x000004b0 00000000 96010000 00000000 97010000 ................
-  0x000004c0 9c010000 00000000 9e010000 9f010000 ................
-  0x000004d0 00000000 a1010000 a3010000 00000000 ................
-  0x000004e0 00000000 a5010000 a6010000 00000000 ................
-  0x000004f0 00000000 a7010000 a8010000 aa010000 ................
-  0x00000500 ac010000 00000000 ad010000 ae010000 ................
-  0x00000510 b0010000 b1010000 b2010000 00000000 ................
-  0x00000520 b3010000 00000000 b4010000 b6010000 ................
-  0x00000530 00000000 00000000 b7010000 b8010000 ................
-  0x00000540 ba010000 bd010000 be010000 c0010000 ................
-  0x00000550 c1010000 00000000 00000000 00000000 ................
-  0x00000560 c2010000 c4010000 c5010000 00000000 ................
-  0x00000570 c9010000 cb010000 ce010000 cf010000 ................
-  0x00000580 00000000 d0010000 00000000 d1010000 ................
+  0x00000410 60010000 62010000 00000000 00000000 `...b...........
+  0x00000420 63010000 64010000 66010000 68010000 c...d...f...h...
+  0x00000430 6a010000 00000000 6b010000 6c010000 j.......k...l...
+  0x00000440 6e010000 6f010000 70010000 00000000 n...o...p.......
+  0x00000450 00000000 72010000 00000000 00000000 ....r...........
+  0x00000460 74010000 00000000 77010000 78010000 t.......w...x...
+  0x00000470 7a010000 7c010000 7f010000 80010000 z...|...........
+  0x00000480 85010000 87010000 88010000 00000000 ................
+  0x00000490 89010000 8a010000 00000000 8d010000 ................
+  0x000004a0 8f010000 90010000 91010000 00000000 ................
+  0x000004b0 00000000 94010000 00000000 95010000 ................
+  0x000004c0 9a010000 00000000 9c010000 9d010000 ................
+  0x000004d0 00000000 9f010000 a1010000 00000000 ................
+  0x000004e0 00000000 a3010000 a4010000 00000000 ................
+  0x000004f0 00000000 a5010000 a6010000 a8010000 ................
+  0x00000500 aa010000 00000000 ab010000 ac010000 ................
+  0x00000510 ae010000 af010000 b0010000 00000000 ................
+  0x00000520 b1010000 00000000 b2010000 b4010000 ................
+  0x00000530 00000000 00000000 b5010000 b6010000 ................
+  0x00000540 b8010000 bb010000 bc010000 be010000 ................
+  0x00000550 bf010000 00000000 00000000 c0010000 ................
+  0x00000560 c1010000 c3010000 c4010000 00000000 ................
+  0x00000570 c8010000 ca010000 cd010000 ce010000 ................
+  0x00000580 00000000 cf010000 00000000 d1010000 ................
   0x00000590 00000000 d2010000 d4010000 d6010000 ................
   0x000005a0 00000000 d7010000 00000000 d9010000 ................
   0x000005b0 00000000 00000000 da010000 00000000 ................
   0x000005c0 db010000 00000000 dd010000 00000000 ................
-  0x000005d0 df010000 00000000 00000000 e0010000 ................
+  0x000005d0 de010000 00000000 df010000 e0010000 ................
   0x000005e0 e4010000 e5010000 e6010000 00000000 ................
   0x000005f0 00000000 e7010000 e9010000 ea010000 ................
   0x00000600 00000000 ee010000 ef010000 f0010000 ................
-  0x00000610 f2010000 f3010000 00000000 00000000 ................
-  0x00000620 f4010000 00000000 f7010000 fa010000 ................
-  0x00000630 00000000 fd010000 fe010000 00000000 ................
-  0x00000640 ff010000 02020000 03020000 04020000 ................
-  0x00000650 05020000 00000000 06020000 08020000 ................
-  0x00000660 00000000 09020000 0a020000 0d020000 ................
-  0x00000670 00000000 0e020000 0f020000 11020000 ................
-  0x00000680 00000000 00000000 00000000 12020000 ................
-  0x00000690 15020000 00000000 16020000 1a020000 ................
-  0x000006a0 1c020000 1e020000 20020000 24020000 ........ ...$...
-  0x000006b0 00000000 00000000 00000000 26020000 ............&...
-  0x000006c0 27020000 00000000 28020000 29020000 '.......(...)...
-  0x000006d0 2e020000 2f020000 32020000 00000000 ..../...2.......
-  0x000006e0 33020000 00000000 35020000 36020000 3.......5...6...
+  0x00000610 f2010000 f4010000 00000000 00000000 ................
+  0x00000620 f5010000 00000000 f8010000 fb010000 ................
+  0x00000630 00000000 fe010000 ff010000 00000000 ................
+  0x00000640 00020000 03020000 04020000 05020000 ................
+  0x00000650 06020000 00000000 07020000 09020000 ................
+  0x00000660 00000000 0a020000 0b020000 0e020000 ................
+  0x00000670 00000000 0f020000 10020000 12020000 ................
+  0x00000680 00000000 00000000 00000000 13020000 ................
+  0x00000690 16020000 00000000 17020000 1b020000 ................
+  0x000006a0 1d020000 1f020000 21020000 25020000 ........!...%...
+  0x000006b0 00000000 00000000 00000000 27020000 ............'...
+  0x000006c0 28020000 00000000 29020000 2a020000 (.......)...*...
+  0x000006d0 2f020000 30020000 33020000 00000000 /...0...3.......
+  0x000006e0 34020000 00000000 36020000 00000000 4.......6.......
   0x000006f0 37020000 38020000 39020000 3a020000 7...8...9...:...
   0x00000700 00000000 00000000 3e020000 3f020000 ........>...?...
   0x00000710 00000000 00000000 00000000 00000000 ................
   0x00000720 41020000 00000000 00000000 00000000 A...............
   0x00000730 00000000 42020000 00000000 44020000 ....B.......D...
   0x00000740 00000000 46020000 47020000 4b020000 ....F...G...K...
   0x00000750 4c020000 00000000 00000000 00000000 L...............
@@ -91,68 +91,68 @@
   0x000007e0 ceb5ef4d d890ab41 65246ad6 3f4fc4e8 ...M...Ae$j.?O..
   0x000007f0 4a812065 fd0a4894 5fe5cd9f b834db7d J. e..H._....4.}
   0x00000800 0be195aa a47c409b be2c5ecf 837853ce .....|@..,^..xS.
   0x00000810 f1faad2c 12cb1f67 d1c43ad0 6b908c99 ...,...g..:.k...
   0x00000820 592125c6 4fef45a0 701a5425 f9bc202a Y!%.O.E.p.T%.. *
   0x00000830 560f641f 3d571b4b 5e494e62 47e9e4a9 V.d.=W.K^INbG...
   0x00000840 289fb23b a10757a6 bae3927c ab8f8b8c (..;..W....|....
-  0x00000850 d784d5f6 c5f494ce 48b4049e 87af7b30 ........H.....{0
-  0x00000860 d6a9b069 492607ee d8223690 fb33dfb8 ...iI&..."6..3..
-  0x00000870 42528d3f 999bbb4c 17a8c695 c5a5e423 BR.?...L.......#
-  0x00000880 aa2fa53b c9491703 2db3dc77 355d7595 ./.;.I..-..w5]u.
-  0x00000890 7cddfae6 f75e326b 10baef4d a5286ad6 |....^2k...M.(j.
-  0x000008a0 10c3a2f6 6ecc0770 2bd5f6bf 4f92fe78 ....n..p+...O..x
-  0x000008b0 4ae595aa 91db71b0 9a828e22 a5b96994 J.....q...."..i.
-  0x000008c0 f695ffaf 5832c56e 31ffad2c 9b910321 ....X2.n1..,...!
-  0x000008d0 baba2758 8426ec49 26dbfe15 c4a3521f ..'X.&.I&.....R.
-  0x000008e0 41f6acd4 c8e1185c f1ec498a 992525c6 A......\..I..%%.
-  0x000008f0 f991741f e7505f11 e2493c34 f06acdd9 ..t..P_..I<4.j..
-  0x00000900 e7787ebb e64655ff f7890bcc 53a553bf .x~..FU.....S.S.
-  0x00000910 eb938b8c 16cbae90 6a5f0533 2f067b51 ........j_.3/.{Q
-  0x00000920 1dbd544d 0822b67c 0eaeb36e 3c38dfb8 ..TM.".|...n<8..
-  0x00000930 4245d5ec 19273690 9e6352ae 7b7304f6 BE...'6..cR.{s..
-  0x00000940 b91fc917 8cb2e115 ff17ac59 a4aebeb5 ...........Y....
-  0x00000950 113fbeb3 b252bb2e 63ef1bef bf27cc22 .?...R..c....'."
-  0x00000960 51beef4d 8b18ff4f 949ad083 f3ba40f5 Q..M...O......@.
-  0x00000970 961ffd61 27f92483 f5fa92bf 2148e42f ...a'.$.....!H./
-  0x00000980 06b96a6e 69413d51 e116b884 2d66413f ..jniA=Q....-fA?
-  0x00000990 a52d0132 5d661733 b624fcd0 27547eb8 .-.2]f.3.$..'T~.
-  0x000009a0 55f4092b 3b7a3c7c 226ba1b1 39eb67aa U..+;z<|"k..9.g.
-  0x000009b0 8c2db72e 5a14dfdc ab23603f cf7da59d .-..Z....#`?.}..
-  0x000009c0 600444eb 17a30a3f ab31a18d 790b4835 `.D....?.1..y.H5
-  0x000009d0 c611c5c7 b709706c 89533e2c 9a424223 ......pl.S>,.BB#
-  0x000009e0 66cfdc15 a6105e81 e7b2beb5 dce3f77e f.....^........~
-  0x000009f0 3b65ab31 66be899f 86d7b7ee c5d978b1 ;e.1f.........x.
-  0x00000a00 d7ac2aff 2db36874 a31a6fbf 53f43a63 ..*.-.ht..o.S.:c
+  0x00000850 d784d5f6 49b4049e d6a9b069 492607ee ....I......iI&..
+  0x00000860 d8223690 fb33dfb8 42528d3f 999bbb4c ."6..3..BR.?...L
+  0x00000870 17a8c695 c5a5e423 aa2fa53b c9491703 .......#./.;.I..
+  0x00000880 2db3dc77 355d7595 7cddfae6 f75e326b -..w5]u.|....^2k
+  0x00000890 10baef4d a5286ad6 10c3a2f6 6ecc0770 ...M.(j.....n..p
+  0x000008a0 2bd5f6bf 4f92fe78 4ae595aa 91db71b0 +...O..xJ.....q.
+  0x000008b0 9a828e22 a5b96994 f695ffaf 5832c56e ..."..i.....X2.n
+  0x000008c0 31ffad2c 9b910321 baba2758 8426ec49 1..,...!..'X.&.I
+  0x000008d0 26dbfe15 c4a3521f 41f6acd4 c8e1185c &.....R.A......\
+  0x000008e0 f1ec498a 992525c6 f991741f e7505f11 ..I..%%...t..P_.
+  0x000008f0 e2493c34 f06acdd9 e7787ebb e64655ff .I<4.j...x~..FU.
+  0x00000900 f7890bcc 53a553bf eb938b8c 16cbae90 ....S.S.........
+  0x00000910 6a5f0533 2f067b51 1dbd544d 0822b67c j_.3/.{Q..TM.".|
+  0x00000920 0eaeb36e 3c38dfb8 4245d5ec 19273690 ...n<8..BE...'6.
+  0x00000930 9e6352ae 7b7304f6 b91fc917 8cb2e115 .cR.{s..........
+  0x00000940 ff17ac59 a4aebeb5 113fbeb3 b252bb2e ...Y.....?...R..
+  0x00000950 63ef1bef bf27cc22 51beef4d 8b18ff4f c....'."Q..M...O
+  0x00000960 949ad083 f3ba40f5 961ffd61 27f92483 ......@....a'.$.
+  0x00000970 f5fa92bf 2148e42f 06b96a6e 69413d51 ....!H./..jniA=Q
+  0x00000980 e116b884 2d66413f a52d0132 5d661733 ....-fA?.-.2]f.3
+  0x00000990 b624fcd0 27547eb8 55f4092b 3b7a3c7c .$..'T~.U..+;z<|
+  0x000009a0 226ba1b1 39eb67aa 8c2db72e 5a14dfdc "k..9.g..-..Z...
+  0x000009b0 ab23603f cf7da59d 600444eb 17a30a3f .#`?.}..`.D....?
+  0x000009c0 ab31a18d 790b4835 b3a90b86 c611c5c7 .1..y.H5........
+  0x000009d0 b709706c 89533e2c 9a424223 66cfdc15 ..pl.S>,.BB#f...
+  0x000009e0 a6105e81 e7b2beb5 dce3f77e 3b65ab31 ..^........~;e.1
+  0x000009f0 66be899f 86d7b7ee c5d978b1 d7ac2aff f.........x...*.
+  0x00000a00 2db36874 e2b6e445 a31a6fbf 53f43a63 -.ht...E..o.S.:c
   0x00000a10 1c9b8bcd 2fa68be0 2a2a5e38 538bdc2b ..../...**^8S..+
   0x00000a20 716a5c04 deb23359 1be17196 ebd3ef0e qj\...3Y..q.....
-  0x00000a30 eb1e26db ac662293 415c57ca d87c6867 ..&..f".A\W..|hg
-  0x00000a40 d98f9c4a 63bcf6ad b0be5902 ae46d3f5 ...Jc.....Y..F..
+  0x00000a30 eb1e26db ac662293 415c57ca d98f9c4a ..&..f".A\W....J
+  0x00000a40 63bcf6ad 77fcaf6f b0be5902 ae46d3f5 c...w..o..Y..F..
   0x00000a50 8c5bccde b98df10e 0be16ca3 5b657489 .[........l.[et.
   0x00000a60 b75ac029 06028a59 afa20bd5 8faf1362 .Z.)...Y.......b
   0x00000a70 26b7beb5 864fbf5a 3a2f9c7b a7d3dc15 &....O.Z:/.{....
   0x00000a80 7b69ab31 07de78b1 a0e33888 9b1f6861 {i.1..x...8...ha
-  0x00000a90 2d8f5471 2175c7e1 44cf4de1 586bebc4 -.Tq!u..D.M.Xk..
-  0x00000aa0 f71d0d80 20854e9c 72418a9d b30a7245 .... .N.rA....rE
-  0x00000ab0 0afb0a3d 3cac53b3 bbd7a8ad 19a51d1f ...=<.S.........
-  0x00000ac0 1fb73359 78383bb9 aac4333c 6f78e0a2 ..3Yx8;...3<ox..
-  0x00000ad0 cf865ca0 d971581c abc0bb5b 777d8f87 ..\..qX....[w}..
-  0x00000ae0 2255f253 af9b9f85 73259f9f 0b446fa5 "U.S....s%...Do.
-  0x00000af0 f0150db5 64e29b05 49fe7d14 815b2598 ....d...I.}..[%.
-  0x00000b00 d7675445 30acd6f9 f9fce865 1f81e828 .gTE0......e...(
-  0x00000b10 b4332c58 6af69c28 bb717818 03e6a81f .3,Xj..(.qx.....
-  0x00000b20 6060f79e 281622e0 bc6dab31 abe5c9af ``..(."..m.1....
-  0x00000b30 46e278b1 2190d23a bad19060 99d64e51 F.x.!..:...`..NQ
-  0x00000b40 3c498574 ed2137bd f0b2ca4f 761836ed <I.t.!7....Ov.6.
-  0x00000b50 1af13f51 bb91c17d 2ae6506d bd7a7cec ..?Q...}*.Pm.z|.
-  0x00000b60 61ddc83b e3282996 93b3cf6b ae211d71 a..;.()....k.!.q
-  0x00000b70 802aa546 ce81b900 60bb3359 c362f9d8 .*.F....`.3Y.b..
-  0x00000b80 1f7ef0fc b83c3bb9 b07ce0a2 51b924fe .~...<;..|..Q.$.
-  0x00000b90 0f8b5ca0 80a75118 0fc93a72 af19fbdc ..\...Q...:r....
-  0x00000ba0 d5a3c324 6544aaee a72f0bd1 457d6eff ...$eD.../..E}n.
+  0x00000a90 2c8f5471 a571cba7 2175c7e1 44cf4de1 ,.Tq.q..!u..D.M.
+  0x00000aa0 586bebc4 f71d0d80 20854e9c 72418a9d Xk...... .N.rA..
+  0x00000ab0 b30a7245 0afb0a3d 3cac53b3 bbd7a8ad ..rE...=<.S.....
+  0x00000ac0 19a51d1f 1fb73359 78383bb9 aac4333c ......3Yx8;...3<
+  0x00000ad0 6f78e0a2 cf865ca0 d971581c abc0bb5b ox....\..qX....[
+  0x00000ae0 777d8f87 2255f253 af9b9f85 73259f9f w}.."U.S....s%..
+  0x00000af0 0b446fa5 f0150db5 64e29b05 49fe7d14 .Do.....d...I.}.
+  0x00000b00 815b2598 d7675445 30acd6f9 f9fce865 .[%..gTE0......e
+  0x00000b10 1f81e828 b4332c58 6af69c28 bb717818 ...(.3,Xj..(.qx.
+  0x00000b20 03e6a81f 6060f79e 281622e0 bc6dab31 ....``..(."..m.1
+  0x00000b30 abe5c9af 46e278b1 2190d23a bad19060 ....F.x.!..:...`
+  0x00000b40 99d64e51 3c498574 ed2137bd f0b2ca4f ..NQ<I.t.!7....O
+  0x00000b50 761836ed 1af13f51 bb91c17d 2ae6506d v.6...?Q...}*.Pm
+  0x00000b60 bd7a7cec 61ddc83b e3282996 93b3cf6b .z|.a..;.()....k
+  0x00000b70 ae211d71 802aa546 ce81b900 60bb3359 .!.q.*.F....`.3Y
+  0x00000b80 c362f9d8 1f7ef0fc b83c3bb9 b07ce0a2 .b...~...<;..|..
+  0x00000b90 51b924fe 0f8b5ca0 80a75118 0fc93a72 Q.$...\...Q...:r
+  0x00000ba0 af19fbdc 6544aaee a72f0bd1 457d6eff ....eD.../..E}n.
   0x00000bb0 66522973 4eafc9c6 a4e69b05 c9e113b3 fR)sN...........
   0x00000bc0 412acdb3 7eaf37a5 e9239031 c1498d3f A*..~.7..#.1.I.?
   0x00000bd0 aaaadc77 6d711e42 02c6816c 5f73fbe0 ...wmq.B...l_s..
   0x00000be0 656cdc0f a6c0fd4e a2a26a4c e6041b27 el.....N..jL...'
   0x00000bf0 1127dad8 fd4ac4e8 efdd0fd2 028bbdff .'...J..........
   0x00000c00 c9dc95aa f4df8617 d84ae7c5 aef6ad2c .........J.....,
   0x00000c10 6248eba2 fb403bb9 518f5ca0 18110eb9 bH...@;.Q.\.....
```

### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1172,27 +1172,27 @@
   0x00008de8 70655074 72495331 5f454576 005f5a4e pePtrIS1_EEv._ZN
   0x00008df8 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
   0x00008e08 33435544 41477561 7264496d 706c3130 3CUDAGuardImpl10
   0x00008e18 71756572 79457665 6e744550 76006375 queryEventEPv.cu
   0x00008e28 64614576 656e7451 75657279 005f5a4e daEventQuery._ZN
   0x00008e38 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x00008e48 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x00008e58 5f6e6d73 5f63755f 31623164 37643065 _nms_cu_1b1d7d0e
-  0x00008e68 5f323230 3031356e 6d735f6b 65726e65 _220015nms_kerne
+  0x00008e58 5f6e6d73 5f63755f 31356239 35653931 _nms_cu_15b95e91
+  0x00008e68 5f323538 3631356e 6d735f6b 65726e65 _258615nms_kerne
   0x00008e78 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x00008e88 5f507900 5f5a4e37 746f7263 68616f34 _Py._ZN7torchao4
   0x00008e98 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
   0x00008ea8 65393235 395f365f 6e6d735f 63755f31 e9259_6_nms_cu_1
-  0x00008eb8 62316437 6430655f 32323030 31356e6d b1d7d0e_220015nm
+  0x00008eb8 35623935 6539315f 32353836 31356e6d 5b95e91_258615nm
   0x00008ec8 735f6b65 726e656c 5f696d70 6c494e33 s_kernel_implIN3
   0x00008ed8 63313034 48616c66 45454576 6964504b c104HalfEEEvidPK
   0x00008ee8 545f5079 005f5a4e 37746f72 6368616f T_Py._ZN7torchao
   0x00008ef8 34335f47 4c4f4241 4c5f5f4e 5f5f3562 43_GLOBAL__N__5b
   0x00008f08 32653932 35395f36 5f6e6d73 5f63755f 2e9259_6_nms_cu_
-  0x00008f18 31623164 37643065 5f323230 3031356e 1b1d7d0e_220015n
+  0x00008f18 31356239 35653931 5f323538 3631356e 15b95e91_258615n
   0x00008f28 6d735f6b 65726e65 6c5f696d 706c4964 ms_kernel_implId
   0x00008f38 45457669 64504b54 5f507900 5f5a4e33 EEvidPKT_Py._ZN3
   0x00008f48 63313031 3056616c 75654572 726f7244 c1010ValueErrorD
   0x00008f58 32457600 5f5a5456 4e336331 30354572 2Ev._ZTVN3c105Er
   0x00008f68 726f7245 005f5a4e 53743965 78636570 rorE._ZNSt9excep
   0x00008f78 74696f6e 44324576 005f5a4e 33633130 tionD2Ev._ZN3c10
   0x00008f88 31305661 6c756545 72726f72 44314576 10ValueErrorD1Ev
@@ -1334,16 +1334,16 @@
   0x00009808 335f5335 5f53385f 005f5a4e 33633130 3_S5_S8_._ZN3c10
   0x00009818 36646574 61696c31 325f7374 725f7772 6detail12_str_wr
   0x00009828 61707065 72494a52 4b63524b 5053325f apperIJRKcRKPS2_
   0x00009838 53345f53 365f5334 5f454534 63616c6c S4_S6_S4_EE4call
   0x00009848 4553335f 53365f53 365f5336 5f53365f ES3_S6_S6_S6_S6_
   0x00009858 005f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x00009868 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x00009878 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x00009888 37643065 5f323230 3031306e 6d735f6b 7d0e_220010nms_k
+  0x00009878 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x00009888 35653931 5f323538 3631306e 6d735f6b 5e91_258610nms_k
   0x00009898 65726e65 6c45524b 4e326174 3654656e ernelERKN2at6Ten
   0x000098a8 736f7245 53345f64 005f5a54 564e3363 sorES4_d._ZTVN3c
   0x000098b8 31303463 75646134 696d706c 31334355 104cuda4impl13CU
   0x000098c8 44414775 61726449 6d706c45 005f5a4e DAGuardImplE._ZN
   0x000098d8 32617434 5f6f7073 3131736f 72745f73 2at4_ops11sort_s
   0x000098e8 7461626c 65346361 6c6c4552 4b4e535f table4callERKNS_
   0x000098f8 3654656e 736f7245 5374386f 7074696f 6TensorESt8optio
@@ -1842,9 +1842,9 @@
   0x0000b7c8 5f332e34 2e313800 43585841 42495f31 _3.4.18.CXXABI_1
   0x0000b7d8 2e332e32 00435858 4142495f 312e332e .3.2.CXXABI_1.3.
   0x0000b7e8 3500474c 49424358 585f332e 342e3900 5.GLIBCXX_3.4.9.
   0x0000b7f8 43585841 42495f31 2e332e33 00435858 CXXABI_1.3.3.CXX
   0x0000b808 4142495f 312e3300 474c4942 4358585f ABI_1.3.GLIBCXX_
   0x0000b818 332e3400 2f5f5f77 2f5f7465 6d702f63 3.4./__w/_temp/c
   0x0000b828 6f6e6461 5f656e76 69726f6e 6d656e74 onda_environment
-  0x0000b838 5f393230 30323032 3736362f 6c696200 _9200202766/lib.
+  0x0000b838 5f393231 36363533 3730352f 6c696200 _9216653705/lib.
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 Disassembly of section .plt.got:
 
 0000000000011380 <vsnprintf@plt>:
-	jmp    *0xa4a22(%rip)        
+	jmp    *0xa4a2a(%rip)        
 	xchg   %ax,%ax
 
 0000000000011388 <__cxa_finalize@plt>:
 	jmp    *0xa4b2a(%rip)        
 	xchg   %ax,%ax
 
 0000000000011390 <SplitK_Reduction(__half*, float*, unsigned long, unsigned long, int)@plt>:
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -8,34 +8,34 @@
 	mov    %r12,%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    %r13,%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    %rbx,%rdi
 	call   10650 <_Unwind_Resume@plt>
 
-00000000000113b8 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>:
-_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold():
+00000000000113b8 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>:
+_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold():
 	mov    %r12,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
 	lea    0xa5779(%rip),%rdi        
 	call   107b0 <torch::Library::~Library()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    0x10(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa4944(%rip),%rdi        
-	je     113f0 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x38>
+	je     113f0 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x38>
 	lea    0x6(%rsp),%rsi
 	call   13850 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    113c0 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
+	jmp    113c0 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
 
 0000000000011405 <cast_fp16_fp6(unsigned short*, unsigned char*) [clone .cold]>:
 cast_fp16_fp6(unsigned short*, unsigned char*) [clone .cold]:
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x235fa(%rip),%rsi        
 	mov    %rax,%rdi
@@ -79,45 +79,45 @@
 000000000001149f <torchao::weight_matrix_dequant_cpu(at::Tensor, at::Tensor) [clone .cold]>:
 torchao::weight_matrix_dequant_cpu(at::Tensor, at::Tensor) [clone .cold]:
 	mov    %r13,%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 
-00000000000114af <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>:
-_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold():
+00000000000114af <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>:
+_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold():
 	mov    %r12,%rdi
 	call   11180 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    %r13,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
 	lea    0xa571a(%rip),%rdi        
 	call   107b0 <torch::Library::~Library()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    0xa0(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa4842(%rip),%rdi        
-	je     114f2 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x43>
+	je     114f2 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x43>
 	lea    0x30(%rsp),%rsi
 	call   19560 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 	mov    %r12,%rdi
 	call   11180 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    %r13,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 
 0000000000011526 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]>:
 torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]:
 	mov    -0x1b0(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa47f0(%rip),%rdi        
 	je     11542 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x1c>
@@ -205,16 +205,16 @@
 	mov    %rax,(%rbx)
 	mov    -0x210(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa463a(%rip),%rdi        
 	je     116fc <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x1d6>
 	mov    -0x2d8(%rbp),%rsi
 	call   1bcc0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
-	mov    0xa4725(%rip),%rdx        
-	mov    0xa46c6(%rip),%rsi        
+	mov    0xa472d(%rip),%rdx        
+	mov    0xa46ce(%rip),%rsi        
 	mov    %rbx,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbx
 	mov    $0x3,%eax
 	shl    $0x3e,%rax
 	cmp    %rax,-0x170(%rbp)
 	jge    1172f <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x209>
@@ -301,38 +301,38 @@
 	jmp    115f6 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0xd0>
 	mov    -0x190(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa4458(%rip),%rdi        
 	jne    1153a <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x14>
 	jmp    11542 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x1c>
 
-00000000000118db <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold>:
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold():
+00000000000118db <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold>:
+_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold():
 	mov    0x10(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa443d(%rip),%rdi        
-	je     118f7 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x1c>
+	je     118f7 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x1c>
 	lea    0x6(%rsp),%rsi
 	call   1bcc0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    11914 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
+	jmp    11914 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
 	mov    %r12,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
 	lea    0xa5365(%rip),%rdi        
 	call   107b0 <torch::Library::~Library()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 
 0000000000011928 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa44d8(%rip)        
+	cmpq   $0x0,0xa44e0(%rip)        
 	je     1193c <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x14>
 	or     $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	jmp    11945 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x1d>
 	mov    0x10(%rdi),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x10(%rdi)
@@ -402,15 +402,15 @@
 	lea    0x12(%rsp),%rsi
 	call   11928 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    11967 <_GLOBAL__sub_I_fp6_llm.cpp.cold+0x18>
 	nop
 
 0000000000011a3e <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa43c2(%rip)        
+	cmpq   $0x0,0xa43ca(%rip)        
 	je     11a52 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x14>
 	or     $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	jmp    11a5b <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x1d>
 	mov    0x10(%rdi),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x10(%rdi)
@@ -538,16 +538,16 @@
 	push   %rbp
 	push   %rax
 	call   10d60 <__cxa_allocate_exception@plt>
 	mov    %r12,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	call   102e0 <std::runtime_error::runtime_error(char const*)@plt>
-	mov    0xa433f(%rip),%rdx        
-	mov    0xa41e8(%rip),%rsi        
+	mov    0xa4347(%rip),%rdx        
+	mov    0xa41f0(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%r12
 	mov    %rbp,%rdi
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
@@ -560,16 +560,16 @@
 	push   %rbp
 	push   %rax
 	call   10d60 <__cxa_allocate_exception@plt>
 	mov    %r12,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	call   10870 <std::runtime_error::runtime_error(std::string const&)@plt>
-	mov    0xa42f7(%rip),%rdx        
-	mov    0xa41a0(%rip),%rsi        
+	mov    0xa42ff(%rip),%rdx        
+	mov    0xa41a8(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%r12
 	mov    %rbp,%rdi
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
@@ -592,15 +592,15 @@
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	nop
 
 0000000000011ce6 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa411a(%rip)        
+	cmpq   $0x0,0xa4122(%rip)        
 	je     11cfa <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x14>
 	or     $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	jmp    11d03 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x1d>
 	mov    0x10(%rdi),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x10(%rdi)
@@ -648,15 +648,15 @@
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	lea    0x215e7(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
-	mov    0xa4050(%rip),%rsi        # b5e00 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0190>
+	mov    0xa4058(%rip),%rsi        # b5e08 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0198>
 	mov    %rcx,%rdx
 	push   $0x0
 	mov    %rax,0xa4d64(%rip)        
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
@@ -682,15 +682,15 @@
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x21660(%rip),%rcx        
-	mov    0xa3fa9(%rip),%rsi        # b5de0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0530>
+	mov    0xa3fb1(%rip),%rsi        # b5de8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0538>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -718,27 +718,27 @@
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x216de(%rip),%rcx        
-	mov    0xa3f7f(%rip),%rsi        # b5e40 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff50>
+	mov    0xa3f87(%rip),%rsi        # b5e48 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff58>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x21708(%rip),%rcx        
-	mov    0xa3ea1(%rip),%rsi        # b5d90 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe0>
+	mov    0xa3ea9(%rip),%rsi        # b5d98 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe8>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -768,23 +768,23 @@
 	pop    %rdx
 	call   10ed0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0x16a0(%rip),%rdi        
 	pop    %rbp
 	jmp    32c40 <atexit>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000011f80 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp>:
-_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp():
+0000000000011f80 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp>:
+_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp():
 	push   %r12
 	lea    0xa4c17(%rip),%rdi        
 	push   %rbp
 	push   %rbx
 	sub    $0x60,%rsp
 	call   11260 <std::ios_base::Init::Init()@plt>
-	mov    0xa3fa5(%rip),%rdi        
+	mov    0xa3fad(%rip),%rdi        
 	lea    0x10(%rsp),%rbp
 	lea    0xa33d1(%rip),%rdx        
 	lea    0xa4bf2(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	mov    $0x31,%eax
 	movb   $0x0,0xb(%rsp)
 	mov    %rbp,%rdi
@@ -802,15 +802,15 @@
 	lea    0x2131c(%rip),%r8        
 	lea    0xa4b3d(%rip),%rdi        
 	call   10640 <torch::Library::Library(torch::Library::Kind, std::string, std::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x10(%rsp),%rax
 	mov    0xa3d14(%rip),%rbx        
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
-	jne    120e9 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0x169>
+	jne    120e9 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0x169>
 	mov    $0x18,%edi
 	movb   $0x0,0x12(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	movq   $0x0,0x8(%rax)
 	mov    %rax,%rsi
 	lea    0x18(%rsp),%r12
 	mov    0xa3e89(%rip),%rax        # b5ed0 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >@@Base+0x820>
@@ -823,46 +823,46 @@
 	lea    0x48(%rsp),%rdi
 	movb   $0x1,0x40(%rsp)
 	mov    0xa3c56(%rip),%rax        # b5cc8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9cac8>
 	movq   $0x0,0x30(%rsp)
 	mov    %rax,0x20(%rsp)
 	mov    0xa3f01(%rip),%rax        # b5f88 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, at::Tensor (at::Tensor, at::Tensor, at::Tensor, long)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor, at::Tensor, at::Tensor, long)@@Base+0x9ea48>
 	mov    %rax,0x28(%rsp)
-	mov    0xa3d25(%rip),%rax        
+	mov    0xa3d2d(%rip),%rax        
 	mov    %rax,0x38(%rsp)
 	call   10fd0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long)>()@plt>
 	lea    0x18(%rbx),%rax
 	xor    %ecx,%ecx
 	lea    0x216ae(%rip),%rsi        
 	mov    %rbp,%rdx
 	lea    0xa4a8c(%rip),%rdi        
 	mov    %rax,0x50(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa3d7b(%rip),%rdi        
+	mov    0xa3d83(%rip),%rdi        
 	lea    0xa32a4(%rip),%rdx        
 	lea    0xa4a65(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x60,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 	lea    0x6(%rsp),%rsi
 	call   13850 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
-	jmp    12021 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0xa1>
+	jmp    12021 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0xa1>
 	mov    %rax,%rbp
-	jmp    113c0 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
+	jmp    113c0 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
 	mov    %rax,%rbp
-	jmp    113d4 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x1c>
+	jmp    113d4 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x1c>
 	mov    %rax,%rbx
-	jmp    113f8 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x40>
+	jmp    113f8 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x40>
 	mov    %rax,%rbp
-	jmp    113b8 <_GLOBAL__sub_I_tmpxft_00000875_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>
+	jmp    113b8 <_GLOBAL__sub_I_tmpxft_000009f7_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>
 	nopl   0x0(%rax,%rax,1)
 
 0000000000012120 <__sti____cudaRegisterAll()>:
 __sti____cudaRegisterAll():
 	sub    $0x8,%rsp
 	lea    0xa4925(%rip),%rdi        
 	call   10400 <__cudaRegisterFatBinary@plt>
@@ -881,26 +881,26 @@
 	pop    %rdx
 	call   10ed0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0x73de(%rip),%rdi        
 	add    $0x8,%rsp
 	jmp    32c40 <atexit>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000012180 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp>:
-_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp():
+0000000000012180 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp>:
+_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp():
 	push   %r15
 	lea    0xa4ab7(%rip),%rdi        
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0xf8,%rsp
 	call   11260 <std::ios_base::Init::Init()@plt>
-	mov    0xa3d9c(%rip),%rdi        
+	mov    0xa3da4(%rip),%rdi        
 	lea    0xa31cd(%rip),%rdx        
 	lea    0xa4a8e(%rip),%rsi        
 	lea    0xa0(%rsp),%r12
 	lea    0x50(%rsp),%rbp
 	call   10740 <__cxa_atexit@plt>
 	mov    $0x30,%eax
 	mov    %rbp,%rdx
@@ -919,43 +919,43 @@
 	lea    0x2287d(%rip),%r8        
 	lea    0xa49ce(%rip),%rdi        
 	call   10640 <torch::Library::Library(torch::Library::Kind, std::string, std::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0xa0(%rsp),%rax
 	mov    0xa3b02(%rip),%rbx        
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
-	jne    124c8 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp+0x348>
+	jne    124c8 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp+0x348>
 	mov    $0x18,%edi
 	movb   $0x0,0x52(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	mov    %rax,%rsi
 	lea    0x58(%rsp),%r13
 	lea    0x30(%rsp),%r14
 	movq   $0x0,0x8(%rax)
-	mov    0xa3b7a(%rip),%rax        # b5dd8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >@@Base+0x6b0>
+	mov    0xa3b82(%rip),%rax        # b5de0 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >@@Base+0x6b8>
 	mov    %r13,%rdi
 	lea    0x20(%rsp),%r15
-	movq   0xa3ba2(%rip),%xmm0        # b5e10 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b0>
+	movq   0xa3baa(%rip),%xmm0        # b5e18 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b8>
 	add    $0x10,%rax
-	movhps 0xa3a67(%rip),%xmm0        # b5ce0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0530>
+	movhps 0xa3a6f(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	mov    %rax,(%rsi)
 	mov    0xa3a8d(%rip),%rax        
 	movaps %xmm0,(%rsp)
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	movdqa (%rsp),%xmm0
 	mov    %r14,%rcx
 	mov    %r15,%rsi
 	mov    0xa3d0e(%rip),%rax        # b5fb0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9a7d0>
 	mov    $0x1,%r8d
 	mov    $0x1,%edx
 	mov    %r12,%rdi
 	movq   $0x0,0x70(%rsp)
 	mov    %rax,0x60(%rsp)
-	mov    0xa3aeb(%rip),%rax        # b5db0 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor)@@Base+0x9ad10>
+	mov    0xa3af3(%rip),%rax        # b5db8 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor)@@Base+0x9ad18>
 	movb   $0x1,0x80(%rsp)
 	mov    %rax,0x68(%rsp)
 	mov    0xa3b9f(%rip),%rax        
 	movaps %xmm0,0x20(%rsp)
 	mov    %rax,0x78(%rsp)
 	movaps %xmm0,0x30(%rsp)
 	call   10250 <c10::detail::infer_schema::make_function_schema(c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>, c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>)@plt>
@@ -985,33 +985,33 @@
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
 	mov    $0x18,%edi
 	movb   $0x0,0x52(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	mov    %rax,%rsi
 	movq   $0x0,0x8(%rax)
 	mov    %r13,%rdi
-	mov    0xa3bae(%rip),%rax        # b5f48 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >@@Base+0x7f8>
+	mov    0xa3bb6(%rip),%rax        # b5f50 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >@@Base+0x800>
 	add    $0x10,%rax
 	mov    %rax,(%rsi)
-	mov    0xa39f8(%rip),%rax        
+	mov    0xa3a00(%rip),%rax        
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	movdqa (%rsp),%xmm1
 	mov    %r15,%rcx
 	mov    %r14,%rsi
-	mov    0xa3b75(%rip),%rax        # b5f38 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9aa48>
+	mov    0xa3b7d(%rip),%rax        # b5f40 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9aa50>
 	mov    $0x1,%r8d
 	mov    $0x2,%edx
 	mov    %r12,%rdi
 	movq   $0x0,0x70(%rsp)
 	mov    %rax,0x60(%rsp)
-	mov    0xa3912(%rip),%rax        # b5cf8 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, at::Tensor (at::Tensor, at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor, at::Tensor)@@Base+0x9abe8>
+	mov    0xa391a(%rip),%rax        # b5d00 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, at::Tensor (at::Tensor, at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor, at::Tensor)@@Base+0x9abf0>
 	movb   $0x1,0x80(%rsp)
 	mov    %rax,0x68(%rsp)
-	mov    0xa398e(%rip),%rax        
+	mov    0xa3996(%rip),%rax        
 	movaps %xmm1,0x30(%rsp)
 	mov    %rax,0x78(%rsp)
 	movaps %xmm1,0x40(%rsp)
 	movaps %xmm1,0x20(%rsp)
 	call   10250 <c10::detail::infer_schema::make_function_schema(c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>, c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>)@plt>
 	mov    $0x48,%edi
 	call   10b80 <operator new(unsigned long)@plt>
@@ -1033,45 +1033,45 @@
 	movups %xmm6,0x20(%rax)
 	movups %xmm7,0x30(%rax)
 	lea    0x18(%rbx),%rax
 	mov    %rax,0x90(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa39a5(%rip),%rdi        
+	mov    0xa39ad(%rip),%rdi        
 	lea    0xa2ece(%rip),%rdx        
 	lea    0xa472f(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0xf8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	lea    0x30(%rsp),%rsi
 	call   19560 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
-	jmp    12233 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp+0xb3>
+	jmp    12233 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp+0xb3>
 	mov    %rax,%rbp
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 	mov    %rax,%rbp
-	jmp    114d3 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x24>
+	jmp    114d3 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x24>
 	mov    %rax,%rbx
-	jmp    114fa <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x4b>
+	jmp    114fa <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x4b>
 	mov    %rax,%rbp
-	jmp    11507 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x58>
+	jmp    11507 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x58>
 	mov    %rax,%rbp
-	jmp    1150f <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x60>
+	jmp    1150f <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x60>
 	mov    %rax,%rbx
-	jmp    11519 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x6a>
+	jmp    11519 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x6a>
 	mov    %rax,%rbp
-	jmp    114af <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>
+	jmp    114af <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>
 	mov    %rax,%rbp
-	jmp    114b7 <_GLOBAL__sub_I_tmpxft_00000876_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x8>
+	jmp    114b7 <_GLOBAL__sub_I_tmpxft_000009f8_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x8>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000012520 <__sti____cudaRegisterAll()>:
 __sti____cudaRegisterAll():
 	push   %rbp
 	lea    0xa4540(%rip),%rdi        
 	call   10400 <__cudaRegisterFatBinary@plt>
@@ -1079,37 +1079,37 @@
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	lea    0x2314f(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
-	mov    0xa3918(%rip),%rsi        # b5e68 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x978a8>
+	mov    0xa3830(%rip),%rsi        # b5d80 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x977c0>
 	mov    %rcx,%rdx
 	push   $0x0
 	mov    %rax,0xa4704(%rip)        
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x23184(%rip),%rcx        
-	mov    0xa3a65(%rip),%rsi        # b5fe0 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x97af0>
+	mov    0xa3a6d(%rip),%rsi        # b5fe8 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x97af8>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x231ae(%rip),%rcx        
-	mov    0xa375f(%rip),%rsi        # b5d08 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97678>
+	mov    0xa3737(%rip),%rsi        # b5ce0 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97650>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -1128,23 +1128,23 @@
 	call   10ed0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0x96b4(%rip),%rdi        
 	pop    %rbp
 	jmp    32c40 <atexit>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000012610 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp>:
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp():
+0000000000012610 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp>:
+_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp():
 	push   %r12
 	lea    0xa46c7(%rip),%rdi        
 	push   %rbp
 	push   %rbx
 	sub    $0x60,%rsp
 	call   11260 <std::ios_base::Init::Init()@plt>
-	mov    0xa3915(%rip),%rdi        
+	mov    0xa391d(%rip),%rdi        
 	lea    0x10(%rsp),%rbp
 	lea    0xa2d41(%rip),%rdx        
 	lea    0xa46a2(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	mov    $0x31,%eax
 	movb   $0x0,0xb(%rsp)
 	mov    %rbp,%rdi
@@ -1162,77 +1162,77 @@
 	lea    0x2329c(%rip),%r8        
 	lea    0xa45ed(%rip),%rdi        
 	call   10640 <torch::Library::Library(torch::Library::Kind, std::string, std::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x10(%rsp),%rax
 	mov    0xa3684(%rip),%rbx        
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
-	jne    12779 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp+0x169>
+	jne    12779 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp+0x169>
 	mov    $0x18,%edi
 	movb   $0x0,0x12(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	movq   $0x0,0x8(%rax)
 	mov    %rax,%rsi
 	lea    0x18(%rsp),%r12
 	mov    0xa3811(%rip),%rax        # b5ee8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >@@Base+0x618>
 	mov    %r12,%rdi
 	add    $0x10,%rax
 	mov    %rax,(%rsi)
-	mov    0xa3890(%rip),%rax        
+	mov    0xa3850(%rip),%rax        
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	lea    0x48(%rsp),%rdi
 	movb   $0x1,0x40(%rsp)
-	mov    0xa35ee(%rip),%rax        # b5cf0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x92d70>
+	mov    0xa35f6(%rip),%rax        # b5cf8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x92d78>
 	movq   $0x0,0x30(%rsp)
 	mov    %rax,0x20(%rsp)
 	mov    0xa35a9(%rip),%rax        # b5cc0 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, at::Tensor (at::Tensor const&, at::Tensor const&, double)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor const&, at::Tensor const&, double)@@Base+0x97ca0>
 	mov    %rax,0x28(%rsp)
-	mov    0xa365d(%rip),%rax        
+	mov    0xa3665(%rip),%rax        
 	mov    %rax,0x38(%rsp)
 	call   10d70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double)>()@plt>
 	lea    0x18(%rbx),%rax
 	xor    %ecx,%ecx
 	lea    0x22ae9(%rip),%rsi        
 	mov    %rbp,%rdx
 	lea    0xa453c(%rip),%rdi        
 	mov    %rax,0x50(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa36eb(%rip),%rdi        
+	mov    0xa36f3(%rip),%rdi        
 	lea    0xa2c14(%rip),%rdx        
 	lea    0xa4515(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x60,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
-	cmpq   $0x0,0xa3687(%rip)        
-	je     127a2 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp+0x192>
+	cmpq   $0x0,0xa368f(%rip)        
+	je     127a2 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp+0x192>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
-	jg     126b1 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
+	jg     126b1 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
 	lea    0x6(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
-	jmp    126b1 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
+	jmp    126b1 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
 	mov    -0x8(%rax),%edx
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
-	jmp    1278b <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp+0x17b>
+	jmp    1278b <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp+0x17b>
 	mov    %rax,%rbp
-	jmp    118db <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold>
+	jmp    118db <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold>
 	mov    %rax,%rbx
-	jmp    118ff <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x24>
+	jmp    118ff <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x24>
 	mov    %rax,%rbp
-	jmp    1190c <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x31>
+	jmp    1190c <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x31>
 	mov    %rax,%rbp
-	jmp    11914 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
+	jmp    11914 <_GLOBAL__sub_I_tmpxft_000009f9_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
 	nopl   (%rax)
 
 00000000000127d0 <_GLOBAL__sub_I_fp6_llm.cpp>:
 _GLOBAL__sub_I_fp6_llm.cpp():
 	push   %r15
 	lea    0x20feb(%rip),%rsi        
 	push   %r14
@@ -1420,15 +1420,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    12b73 <_GLOBAL__sub_I_fp6_llm.cpp+0x3a3>
 	mov    0x20(%rsp),%rdi
 	test   %rdi,%rdi
 	je     12b2b <_GLOBAL__sub_I_fp6_llm.cpp+0x35b>
 	call   10520 <operator delete(void*)@plt>
-	mov    0xa3316(%rip),%rdi        
+	mov    0xa331e(%rip),%rdi        
 	lea    0xa283f(%rip),%rdx        
 	lea    0xa41c0(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x98,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
@@ -1437,124 +1437,124 @@
 	pop    %r15
 	ret
 	movq   %rax,%xmm2
 	movb   $0x1,0xa41cd(%rip)        
 	punpcklqdq %xmm2,%xmm0
 	movaps %xmm0,0xa41b2(%rip)        
 	jmp    12875 <_GLOBAL__sub_I_fp6_llm.cpp+0xa5>
-	cmpq   $0x0,0xa328d(%rip)        
+	cmpq   $0x0,0xa3295(%rip)        
 	je     12e42 <_GLOBAL__sub_I_fp6_llm.cpp+0x672>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12b1c <_GLOBAL__sub_I_fp6_llm.cpp+0x34c>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12b1c <_GLOBAL__sub_I_fp6_llm.cpp+0x34c>
-	cmpq   $0x0,0xa3269(%rip)        
+	cmpq   $0x0,0xa3271(%rip)        
 	je     12e34 <_GLOBAL__sub_I_fp6_llm.cpp+0x664>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	lea    0x18(%rsp),%r12
 	test   %edx,%edx
 	jg     12845 <_GLOBAL__sub_I_fp6_llm.cpp+0x75>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12845 <_GLOBAL__sub_I_fp6_llm.cpp+0x75>
-	cmpq   $0x0,0xa3239(%rip)        
+	cmpq   $0x0,0xa3241(%rip)        
 	je     12e26 <_GLOBAL__sub_I_fp6_llm.cpp+0x656>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     128bb <_GLOBAL__sub_I_fp6_llm.cpp+0xeb>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    128bb <_GLOBAL__sub_I_fp6_llm.cpp+0xeb>
-	cmpq   $0x0,0xa320c(%rip)        
+	cmpq   $0x0,0xa3214(%rip)        
 	je     12dae <_GLOBAL__sub_I_fp6_llm.cpp+0x5de>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12910 <_GLOBAL__sub_I_fp6_llm.cpp+0x140>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12910 <_GLOBAL__sub_I_fp6_llm.cpp+0x140>
-	cmpq   $0x0,0xa31e1(%rip)        
+	cmpq   $0x0,0xa31e9(%rip)        
 	je     12da0 <_GLOBAL__sub_I_fp6_llm.cpp+0x5d0>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12922 <_GLOBAL__sub_I_fp6_llm.cpp+0x152>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12922 <_GLOBAL__sub_I_fp6_llm.cpp+0x152>
-	cmpq   $0x0,0xa31b6(%rip)        
+	cmpq   $0x0,0xa31be(%rip)        
 	je     12e18 <_GLOBAL__sub_I_fp6_llm.cpp+0x648>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12972 <_GLOBAL__sub_I_fp6_llm.cpp+0x1a2>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12972 <_GLOBAL__sub_I_fp6_llm.cpp+0x1a2>
-	cmpq   $0x0,0xa3189(%rip)        
+	cmpq   $0x0,0xa3191(%rip)        
 	je     12e0a <_GLOBAL__sub_I_fp6_llm.cpp+0x63a>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     129ba <_GLOBAL__sub_I_fp6_llm.cpp+0x1ea>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    129ba <_GLOBAL__sub_I_fp6_llm.cpp+0x1ea>
-	cmpq   $0x0,0xa315e(%rip)        
+	cmpq   $0x0,0xa3166(%rip)        
 	je     12dfc <_GLOBAL__sub_I_fp6_llm.cpp+0x62c>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     129cc <_GLOBAL__sub_I_fp6_llm.cpp+0x1fc>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    129cc <_GLOBAL__sub_I_fp6_llm.cpp+0x1fc>
-	cmpq   $0x0,0xa3133(%rip)        
+	cmpq   $0x0,0xa313b(%rip)        
 	je     12dee <_GLOBAL__sub_I_fp6_llm.cpp+0x61e>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12a1c <_GLOBAL__sub_I_fp6_llm.cpp+0x24c>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12a1c <_GLOBAL__sub_I_fp6_llm.cpp+0x24c>
-	cmpq   $0x0,0xa3106(%rip)        
+	cmpq   $0x0,0xa310e(%rip)        
 	je     12de0 <_GLOBAL__sub_I_fp6_llm.cpp+0x610>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12a64 <_GLOBAL__sub_I_fp6_llm.cpp+0x294>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12a64 <_GLOBAL__sub_I_fp6_llm.cpp+0x294>
-	cmpq   $0x0,0xa30db(%rip)        
+	cmpq   $0x0,0xa30e3(%rip)        
 	je     12dd2 <_GLOBAL__sub_I_fp6_llm.cpp+0x602>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12a76 <_GLOBAL__sub_I_fp6_llm.cpp+0x2a6>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12a76 <_GLOBAL__sub_I_fp6_llm.cpp+0x2a6>
-	cmpq   $0x0,0xa30b0(%rip)        
+	cmpq   $0x0,0xa30b8(%rip)        
 	je     12dc7 <_GLOBAL__sub_I_fp6_llm.cpp+0x5f7>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12ac6 <_GLOBAL__sub_I_fp6_llm.cpp+0x2f6>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12ac6 <_GLOBAL__sub_I_fp6_llm.cpp+0x2f6>
-	cmpq   $0x0,0xa3087(%rip)        
+	cmpq   $0x0,0xa308f(%rip)        
 	je     12dbc <_GLOBAL__sub_I_fp6_llm.cpp+0x5ec>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12b0e <_GLOBAL__sub_I_fp6_llm.cpp+0x33e>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -1670,50 +1670,50 @@
 	jne    13003 <_GLOBAL__sub_I_weight_prepacking.cpp+0x143>
 	mov    $0x18,%edi
 	movb   $0x0,0x12(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	movq   $0x0,0x8(%rax)
 	mov    %rax,%rsi
 	lea    0x18(%rsp),%r12
-	mov    0xa2e77(%rip),%rax        # b5dd8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >@@Base+0x6b0>
+	mov    0xa2e7f(%rip),%rax        # b5de0 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >@@Base+0x6b8>
 	mov    %r12,%rdi
 	add    $0x10,%rax
 	mov    %rax,(%rsi)
-	mov    0xa2e7e(%rip),%rax        
+	mov    0xa2e86(%rip),%rax        
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	lea    0x48(%rsp),%rdi
 	movb   $0x1,0x40(%rsp)
 	mov    0xa3024(%rip),%rax        # b5fb0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9a7d0>
 	movq   $0x0,0x30(%rsp)
 	mov    %rax,0x20(%rsp)
-	mov    0xa2e0f(%rip),%rax        # b5db0 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor)@@Base+0x9ad10>
+	mov    0xa2e17(%rip),%rax        # b5db8 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor)@@Base+0x9ad18>
 	mov    %rax,0x28(%rsp)
 	mov    0xa2ecb(%rip),%rax        
 	mov    %rax,0x38(%rsp)
 	call   110f0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor)>()@plt>
 	lea    0x18(%rbx),%rax
 	xor    %ecx,%ecx
 	lea    0x23546(%rip),%rsi        
 	mov    %rbp,%rdx
 	lea    0xa3d92(%rip),%rdi        
 	mov    %rax,0x50(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa2e61(%rip),%rdi        
+	mov    0xa2e69(%rip),%rdi        
 	lea    0xa238a(%rip),%rdx        
 	lea    0xa3d6b(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x60,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
-	cmpq   $0x0,0xa2dfd(%rip)        
+	cmpq   $0x0,0xa2e05(%rip)        
 	je     1302c <_GLOBAL__sub_I_weight_prepacking.cpp+0x16c>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12f3b <_GLOBAL__sub_I_weight_prepacking.cpp+0x7b>
 	lea    0x6(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -1733,15 +1733,15 @@
 	nopw   0x0(%rax,%rax,1)
 
 0000000000013060 <_GLOBAL__sub_I_init.cpp>:
 _GLOBAL__sub_I_init.cpp():
 	sub    $0x8,%rsp
 	lea    0xa3dbd(%rip),%rdi        
 	call   11260 <std::ios_base::Init::Init()@plt>
-	mov    0xa2ec9(%rip),%rdi        
+	mov    0xa2ed1(%rip),%rdi        
 	add    $0x8,%rsp
 	lea    0xa22f6(%rip),%rdx        
 	lea    0xa3d9f(%rip),%rsi        
 	jmp    10740 <__cxa_atexit@plt>
 	xchg   %ax,%ax
 
 0000000000013090 <_GLOBAL__sub_I_nms.cpp>:
@@ -1813,58 +1813,58 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    1321c <_GLOBAL__sub_I_nms.cpp+0x18c>
 	mov    0x10(%rsp),%rdi
 	test   %rdi,%rdi
 	je     131d8 <_GLOBAL__sub_I_nms.cpp+0x148>
 	call   10520 <operator delete(void*)@plt>
-	mov    0xa2c69(%rip),%rdi        
+	mov    0xa2c71(%rip),%rdi        
 	lea    0xa2192(%rip),%rdx        
 	lea    0xa3c73(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	movq   %rax,%xmm2
 	movb   $0x1,0xa3c84(%rip)        
 	punpcklqdq %xmm2,%xmm0
 	movaps %xmm0,0xa3c69(%rip)        
 	jmp    13131 <_GLOBAL__sub_I_nms.cpp+0xa1>
-	cmpq   $0x0,0xa2be4(%rip)        
+	cmpq   $0x0,0xa2bec(%rip)        
 	je     132c7 <_GLOBAL__sub_I_nms.cpp+0x237>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     131c9 <_GLOBAL__sub_I_nms.cpp+0x139>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    131c9 <_GLOBAL__sub_I_nms.cpp+0x139>
-	cmpq   $0x0,0xa2bc0(%rip)        
+	cmpq   $0x0,0xa2bc8(%rip)        
 	je     132bc <_GLOBAL__sub_I_nms.cpp+0x22c>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	lea    0x8(%rsp),%r12
 	test   %edx,%edx
 	jg     13101 <_GLOBAL__sub_I_nms.cpp+0x71>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    13101 <_GLOBAL__sub_I_nms.cpp+0x71>
-	cmpq   $0x0,0xa2b94(%rip)        
+	cmpq   $0x0,0xa2b9c(%rip)        
 	je     132e0 <_GLOBAL__sub_I_nms.cpp+0x250>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     13174 <_GLOBAL__sub_I_nms.cpp+0xe4>
 	lea    0x2(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    13174 <_GLOBAL__sub_I_nms.cpp+0xe4>
-	cmpq   $0x0,0xa2b6b(%rip)        
+	cmpq   $0x0,0xa2b73(%rip)        
 	je     132d5 <_GLOBAL__sub_I_nms.cpp+0x245>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     131bb <_GLOBAL__sub_I_nms.cpp+0x12b>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -1916,15 +1916,15 @@
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
 	je     13378 <register_tm_clones+0x38>
-	mov    0xa2ac5(%rip),%rax        
+	mov    0xa2acd(%rip),%rax        
 	test   %rax,%rax
 	je     13378 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
@@ -1967,15 +1967,15 @@
 	push   %rbx
 	mov    %r9,%rbx
 	sub    $0xe8,%rsp
 	movzbl 0xa36a6(%rip),%eax        # b6aa0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     13488 <void Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0xb8>
 	mov    0xa36a0(%rip),%edx        # b6aa8 <Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
-	mov    0xa29f1(%rip),%rdi        # b5e00 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0190>
+	mov    0xa29f9(%rip),%rdi        # b5e08 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0198>
 	mov    $0x8,%esi
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    0x120(%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa367d(%rip),%r8        # b6aa8 <Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
@@ -2054,15 +2054,15 @@
 	mov    %rax,0x70(%rsp)
 	mov    %rax,0x7c(%rsp)
 	movaps %xmm0,0xd0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13471 <void Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0xa1>
 	push   0x50(%rsp)
-	mov    0xa282f(%rip),%rdi        # b5e00 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0190>
+	mov    0xa2837(%rip),%rdi        # b5e08 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0198>
 	push   0x50(%rsp)
 	mov    0x8c(%rsp),%rcx
 	mov    0x94(%rsp),%r8d
 	mov    0x80(%rsp),%rsi
 	mov    0x88(%rsp),%edx
 	lea    0xb0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2192,15 +2192,15 @@
 	pop    %rdx
 	jmp    136b8 <void Kernel_Ex<TilingConfig<4, 1, 8>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int) [clone .constprop.0]+0x98>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000013850 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa25b0(%rip)        
+	cmpq   $0x0,0xa25b8(%rip)        
 	je     13870 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    1387d <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -2447,15 +2447,15 @@
 	jne    13efd <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x56d>
 	movzbl 0xa2db7(%rip),%eax        # b6ad0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 1>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     143b0 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xa20>
 	mov    0xa2db1(%rip),%edx        # b6ad8 <Kernel_Ex<TilingConfig<4, 1, 1>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa20a8(%rip),%rdi        # b5de0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0530>
+	mov    0xa20b0(%rip),%rdi        # b5de8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0538>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa2d8d(%rip),%r8        # b6ad8 <Kernel_Ex<TilingConfig<4, 1, 1>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2515,15 +2515,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13a41 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xb1>
 	push   0x60(%rsp)
-	mov    0xa1f2a(%rip),%rdi        # b5de0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0530>
+	mov    0xa1f32(%rip),%rdi        # b5de8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0538>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2784,15 +2784,15 @@
 	jne    14602 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xc72>
 	movzbl 0xa26bf(%rip),%eax        # b6b00 <guard variable for Kernel_Ex<TilingConfig<4, 1, 2>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     14820 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xe90>
 	mov    0xa26b9(%rip),%edx        # b6b08 <Kernel_Ex<TilingConfig<4, 1, 2>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa19e0(%rip),%rdi        # b5e40 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff50>
+	mov    0xa19e8(%rip),%rdi        # b5e48 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff58>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa2695(%rip),%r8        # b6b08 <Kernel_Ex<TilingConfig<4, 1, 2>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2849,15 +2849,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13aa9 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x119>
 	push   0x60(%rsp)
-	mov    0xa1876(%rip),%rdi        # b5e40 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff50>
+	mov    0xa187e(%rip),%rdi        # b5e48 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff58>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2869,15 +2869,15 @@
 	jne    14329 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x999>
 	movzbl 0xa24f7(%rip),%eax        # b6b10 <guard variable for Kernel_Ex<TilingConfig<4, 1, 1>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     14860 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xed0>
 	mov    0xa24f1(%rip),%edx        # b6b18 <Kernel_Ex<TilingConfig<4, 1, 1>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa1758(%rip),%rdi        # b5d90 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe0>
+	mov    0xa1760(%rip),%rdi        # b5d98 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe8>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa24cd(%rip),%r8        # b6b18 <Kernel_Ex<TilingConfig<4, 1, 1>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2934,15 +2934,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13aa9 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x119>
 	push   0x60(%rsp)
-	mov    0xa15ee(%rip),%rdi        # b5d90 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe0>
+	mov    0xa15f6(%rip),%rdi        # b5d98 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe8>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -3913,15 +3913,15 @@
 	push   %r12
 	mov    %rdi,%r12
 	call   10410 <c10::TensorType::get()@plt>
 	movq   (%rax),%xmm0
 	mov    0x8(%rax),%rax
 	test   %rax,%rax
 	je     15786 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()+0x26>
-	cmpq   $0x0,0xa0689(%rip)        
+	cmpq   $0x0,0xa0691(%rip)        
 	je     157a0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()+0x40>
 	lock addl $0x1,0x8(%rax)
 	movq   %rax,%xmm1
 	mov    %r12,%rax
 	punpcklqdq %xmm1,%xmm0
 	movups %xmm0,(%r12)
 	pop    %r12
@@ -3936,15 +3936,15 @@
 	push   %r12
 	mov    %rdi,%r12
 	call   10410 <c10::TensorType::get()@plt>
 	movq   (%rax),%xmm0
 	mov    0x8(%rax),%rax
 	test   %rax,%rax
 	je     157d6 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()+0x26>
-	cmpq   $0x0,0xa0639(%rip)        
+	cmpq   $0x0,0xa0641(%rip)        
 	je     157f0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()+0x40>
 	lock addl $0x1,0x8(%rax)
 	movq   %rax,%xmm1
 	mov    %r12,%rax
 	punpcklqdq %xmm1,%xmm0
 	movups %xmm0,(%r12)
 	pop    %r12
@@ -4055,15 +4055,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    159df <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0xa0427(%rip),%rdi        # b5de0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0530>
+	mov    0xa042f(%rip),%rdi        # b5de8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0538>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4247,15 +4247,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    15d9f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0xa0087(%rip),%rdi        # b5e00 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0190>
+	mov    0xa008f(%rip),%rdi        # b5e08 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0198>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4311,15 +4311,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    15edf <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0x9fed7(%rip),%rdi        # b5d90 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe0>
+	mov    0x9fedf(%rip),%rdi        # b5d98 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ffe8>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4375,15 +4375,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1601f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0x9fe47(%rip),%rdi        # b5e40 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff50>
+	mov    0x9fe4f(%rip),%rdi        # b5e48 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff58>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4801,15 +4801,15 @@
 	lea    0x1d075(%rip),%rsi        
 	call   10a70 <std::basic_string<char, std::char_traits<char>, std::allocator<char> >::basic_string(char const*, std::allocator<char> const&)@plt>
 	jmp    1652c <c10::IValue::tagKind() const+0x3c>
 	nopl   0x0(%rax)
 	lea    0x1d106(%rip),%rsi        
 	call   10a70 <std::basic_string<char, std::char_traits<char>, std::allocator<char> >::basic_string(char const*, std::allocator<char> const&)@plt>
 	jmp    1652c <c10::IValue::tagKind() const+0x3c>
-	mov    0x9f628(%rip),%rsi        
+	mov    0x9f630(%rip),%rsi        
 	lea    0x10(%rsp),%rbp
 	lea    0x1d0ee(%rip),%rcx        
 	xor    %eax,%eax
 	mov    $0x10,%edx
 	mov    %rbp,%rdi
 	call   10d80 <std::string __gnu_cxx::__to_xstring<std::string, char>(int (*)(char*, unsigned long, char const*, __va_list_tag*), unsigned long, char const*, ...)@plt>
 	mov    $0xb,%ecx
@@ -4908,15 +4908,15 @@
 	movaps %xmm0,0x10(%rsp)
 	jne    169a0 <c10::detail::_str_wrapper<char const*, int const&>::call(char const* const&, int const&)+0x130>
 	mov    0x9f684(%rip),%rax        # b5fa0 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9f51a(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9f522(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9f670(%rip),%rax        # b5fc8 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -4956,15 +4956,15 @@
 	push   %rbp
 	push   %rbx
 	sub    $0x20,%rsp
 	mov    0x8(%rdi),%ecx
 	cmp    $0x1,%ecx
 	jne    16a10 <c10::IValue::destroy()+0x40>
 	mov    (%rdi),%rbp
-	cmp    0x9f2fe(%rip),%rbp        
+	cmp    0x9f306(%rip),%rbp        
 	je     169fd <c10::IValue::destroy()+0x2d>
 	lea    0x8(%rbp),%rax
 	mov    0x8(%rbp),%edx
 	test   %edx,%edx
 	jne    16a70 <c10::IValue::destroy()+0xa0>
 	lock subl $0x1,(%rax)
 	je     16a30 <c10::IValue::destroy()+0x60>
@@ -5257,15 +5257,15 @@
 	movaps %xmm0,0x10(%rsp)
 	jne    16ef0 <c10::detail::_str_wrapper<char const*, unsigned int const&>::call(char const* const&, unsigned int const&)+0x130>
 	mov    0x9f134(%rip),%rax        # b5fa0 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9efca(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9efd2(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9f120(%rip),%rax        # b5fc8 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -5361,96 +5361,96 @@
 	mov    $0x10,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000017010 <c10::VariableVersion::VersionCounter::~VersionCounter()>:
 :VariableVersion::VersionCounter::~VersionCounter():
-	mov    0x9ed81(%rip),%rax        
+	mov    0x9ed89(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000017030 <c10::VariableVersion::VersionCounter::~VersionCounter()>:
 :VariableVersion::VersionCounter::~VersionCounter():
-	mov    0x9ed61(%rip),%rax        
+	mov    0x9ed69(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000017060 <c10::OperatorKernel::~OperatorKernel()>:
 :OperatorKernel::~OperatorKernel():
-	mov    0x9ed91(%rip),%rax        
+	mov    0x9ed99(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000017080 <c10::OperatorKernel::~OperatorKernel()>:
 :OperatorKernel::~OperatorKernel():
-	mov    0x9ed71(%rip),%rax        
+	mov    0x9ed79(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x10,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 00000000000170b0 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ed41(%rip),%rax        
+	mov    0x9ed49(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 00000000000170d0 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ed21(%rip),%rax        
+	mov    0x9ed29(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000017100 <c10::SymNodeImpl::~SymNodeImpl()>:
 :SymNodeImpl::~SymNodeImpl():
-	mov    0x9ecc1(%rip),%rax        
+	mov    0x9ecc9(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000017120 <c10::SymNodeImpl::~SymNodeImpl()>:
 :SymNodeImpl::~SymNodeImpl():
-	mov    0x9eca1(%rip),%rax        
+	mov    0x9eca9(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x10,%esi
@@ -5503,15 +5503,15 @@
 	movaps %xmm0,0x10(%rsp)
 	jne    17280 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)+0x130>
 	mov    0x9ed9f(%rip),%rax        # b5fa0 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9ec35(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9ec3d(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9ed8b(%rip),%rax        # b5fc8 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -5560,31 +5560,31 @@
 	mov    (%rdi),%rax
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     172f8 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x48>
 	mov    (%rdi),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9eb73(%rip),%rax        
+	cmp    0x9eb7b(%rip),%rax        
 	jne    17340 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x90>
 	lock subl $0x1,0xc(%rdi)
 	je     172f8 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x48>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	mov    (%rbx),%rbp
 	test   %rbp,%rbp
 	je     172ee <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x3e>
 	mov    0x0(%rbp),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x9ead9(%rip),%rax        
+	cmp    0x9eae1(%rip),%rax        
 	jne    17347 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x97>
-	mov    0x9eab0(%rip),%rax        
+	mov    0x9eab8(%rip),%rax        
 	mov    %rbp,%rdi
 	add    $0x10,%rax
 	mov    %rax,0x0(%rbp)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	add    $0x8,%rsp
 	mov    %rbp,%rdi
 	mov    $0x10,%esi
@@ -5659,15 +5659,15 @@
 
 0000000000017400 <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()>:
 std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release():
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	sub    $0x8,%rsp
-	mov    0x9e9f8(%rip),%rbx        
+	mov    0x9ea00(%rip),%rbx        
 	test   %rbx,%rbx
 	je     17430 <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()+0x30>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rdi)
 	cmp    $0x1,%eax
 	je     1743e <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()+0x3e>
 	add    $0x8,%rsp
@@ -5716,15 +5716,15 @@
 	mov    %rdi,%rbx
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     174c0 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x40>
 	mov    (%rdi),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9e9a8(%rip),%rax        
+	cmp    0x9e9b0(%rip),%rax        
 	jne    174d8 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x58>
 	lock subl $0x1,0xc(%rdi)
 	je     174c0 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x40>
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
@@ -5739,15 +5739,15 @@
 	mov    (%rbx),%rdi
 	jmp    174b2 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x32>
 	nop
 
 00000000000174e0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()>:
 :intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_():
 	mov    (%rdi),%rax
-	cmp    0x9e7fe(%rip),%rax        
+	cmp    0x9e806(%rip),%rax        
 	je     174f3 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()+0x13>
 	lock subl $0x1,0x8(%rax)
 	je     174f8 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()+0x18>
 	ret
 	nopl   0x0(%rax)
 	push   %rbx
 	mov    (%rdi),%rax
@@ -5779,15 +5779,15 @@
 	push   %r14
 	mov    %rsi,%r10
 	push   %r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	sub    $0x38,%rsp
-	mov    0x9e790(%rip),%rax        
+	mov    0x9e798(%rip),%rax        
 	mov    (%r8),%rsi
 	mov    (%rcx),%rdx
 	mov    (%r9),%rdi
 	lea    0x28(%rsp),%rbp
 	lea    0x20(%rsp),%r13
 	lea    0x18(%rsp),%r14
 	mov    %rax,(%r8)
@@ -5858,15 +5858,15 @@
 	mov    0x9e8b3(%rip),%rdx        
 	mov    %rax,%rbp
 	lea    0x10(%rdx),%rcx
 	lea    0x18(%r14),%rax
 	movb   $0x0,0x7a(%rbp)
 	movq   %rax,%xmm1
 	movq   %rcx,%xmm0
-	mov    0x9e66b(%rip),%rax        
+	mov    0x9e673(%rip),%rax        
 	movq   $0x0,0x18(%rbp)
 	punpcklqdq %xmm1,%xmm0
 	movq   $0x0,0x70(%rbp)
 	movups %xmm0,0x0(%rbp)
 	pxor   %xmm0,%xmm0
 	mov    %rax,0x10(%rbp)
 	xor    %eax,%eax
@@ -5941,15 +5941,15 @@
 	mov    0x40(%rbp),%rdi
 	test   %rdi,%rdi
 	je     177c2 <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x192>
 	call   10310 <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()@plt>
 	mov    0x30(%rbp),%rdi
 	test   %rdi,%rdi
 	je     177eb <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x1bb>
-	cmpq   $0x0,0x9e635(%rip)        
+	cmpq   $0x0,0x9e63d(%rip)        
 	lea    0xc(%rdi),%rdx
 	je     1784d <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x21d>
 	or     $0xffffffff,%eax
 	lock xadd %eax,(%rdx)
 	sub    $0x1,%eax
 	jne    177eb <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x1bb>
 	mov    (%rdi),%rax
@@ -6231,26 +6231,26 @@
 	movzbl 0x40(%r12),%edx
 	test   %dl,%dl
 	jne    180a0 <c10::FunctionSchema::~FunctionSchema()+0x6c0>
 	cmpq   $0x0,0x20(%r12)
 	je     17c27 <c10::FunctionSchema::~FunctionSchema()+0x247>
 	mov    0x20(%r12),%rbp
 	je     17c27 <c10::FunctionSchema::~FunctionSchema()+0x247>
-	mov    0x9e1fd(%rip),%r13        
+	mov    0x9e205(%rip),%r13        
 	test   %r13,%r13
 	je     181d8 <c10::FunctionSchema::~FunctionSchema()+0x7f8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     181a0 <c10::FunctionSchema::~FunctionSchema()+0x7c0>
 	cmpq   $0x0,0x10(%r12)
 	je     17c59 <c10::FunctionSchema::~FunctionSchema()+0x279>
 	mov    0x10(%r12),%rbp
 	je     17c59 <c10::FunctionSchema::~FunctionSchema()+0x279>
-	mov    0x9e1cb(%rip),%r13        
+	mov    0x9e1d3(%rip),%r13        
 	test   %r13,%r13
 	je     18188 <c10::FunctionSchema::~FunctionSchema()+0x7a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     18150 <c10::FunctionSchema::~FunctionSchema()+0x770>
 	mov    (%r12),%rax
@@ -6384,26 +6384,26 @@
 	movzbl 0x40(%r12),%edx
 	test   %dl,%dl
 	jne    17fa0 <c10::FunctionSchema::~FunctionSchema()+0x5c0>
 	cmpq   $0x0,0x20(%r12)
 	je     17eb7 <c10::FunctionSchema::~FunctionSchema()+0x4d7>
 	mov    0x20(%r12),%rbp
 	je     17eb7 <c10::FunctionSchema::~FunctionSchema()+0x4d7>
-	mov    0x9df6d(%rip),%r13        
+	mov    0x9df75(%rip),%r13        
 	test   %r13,%r13
 	je     18088 <c10::FunctionSchema::~FunctionSchema()+0x6a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     18050 <c10::FunctionSchema::~FunctionSchema()+0x670>
 	cmpq   $0x0,0x10(%r12)
 	je     17ee5 <c10::FunctionSchema::~FunctionSchema()+0x505>
 	mov    0x10(%r12),%rbp
 	je     17ee5 <c10::FunctionSchema::~FunctionSchema()+0x505>
-	mov    0x9df3b(%rip),%r13        
+	mov    0x9df43(%rip),%r13        
 	test   %r13,%r13
 	je     17f88 <c10::FunctionSchema::~FunctionSchema()+0x5a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     17f50 <c10::FunctionSchema::~FunctionSchema()+0x570>
 	mov    (%r12),%rax
@@ -6462,15 +6462,15 @@
 	cmp    $0x1a,%ecx
 	ja     1834f <c10::FunctionSchema::~FunctionSchema()+0x96f>
 	mov    $0x1,%eax
 	shl    %cl,%eax
 	test   $0x7ddfdd4,%eax
 	je     17e85 <c10::FunctionSchema::~FunctionSchema()+0x4a5>
 	mov    0x30(%r12),%rbp
-	cmp    0x9dd11(%rip),%rbp        
+	cmp    0x9dd19(%rip),%rbp        
 	je     17e85 <c10::FunctionSchema::~FunctionSchema()+0x4a5>
 	lea    0x8(%rbp),%rax
 	mov    0x8(%rbp),%ecx
 	test   %ecx,%ecx
 	jne    182e8 <c10::FunctionSchema::~FunctionSchema()+0x908>
 	lock subl $0x1,(%rax)
 	jne    17e85 <c10::FunctionSchema::~FunctionSchema()+0x4a5>
@@ -6523,15 +6523,15 @@
 	cmp    $0x1a,%ecx
 	ja     1839b <c10::FunctionSchema::~FunctionSchema()+0x9bb>
 	mov    $0x1,%eax
 	shl    %cl,%eax
 	test   $0x7ddfdd4,%eax
 	je     17bf5 <c10::FunctionSchema::~FunctionSchema()+0x215>
 	mov    0x30(%r12),%rbp
-	cmp    0x9dc11(%rip),%rbp        
+	cmp    0x9dc19(%rip),%rbp        
 	je     17bf5 <c10::FunctionSchema::~FunctionSchema()+0x215>
 	lea    0x8(%rbp),%rax
 	mov    0x8(%rbp),%ecx
 	test   %ecx,%ecx
 	jne    182b0 <c10::FunctionSchema::~FunctionSchema()+0x8d0>
 	lock subl $0x1,(%rax)
 	jne    17bf5 <c10::FunctionSchema::~FunctionSchema()+0x215>
@@ -6592,25 +6592,25 @@
 	jmp    17c27 <c10::FunctionSchema::~FunctionSchema()+0x247>
 	nopl   (%rax)
 	mov    0x8(%rbp),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x8(%rbp)
 	jmp    17c1e <c10::FunctionSchema::~FunctionSchema()+0x23e>
 	cs nopw 0x0(%rax,%rax,1)
-	cmpq   $0x0,0x9dc10(%rip)        
+	cmpq   $0x0,0x9dc18(%rip)        
 	je     18250 <c10::FunctionSchema::~FunctionSchema()+0x870>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     17c6e <c10::FunctionSchema::~FunctionSchema()+0x28e>
 	lea    0x28(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    17c6e <c10::FunctionSchema::~FunctionSchema()+0x28e>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x9dbe0(%rip)        
+	cmpq   $0x0,0x9dbe8(%rip)        
 	je     18260 <c10::FunctionSchema::~FunctionSchema()+0x880>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     17efd <c10::FunctionSchema::~FunctionSchema()+0x51d>
 	lea    0x28(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -6729,15 +6729,15 @@
 	mov    %rdi,%rbx
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     18450 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()+0x40>
 	mov    (%rdi),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9da18(%rip),%rax        
+	cmp    0x9da20(%rip),%rax        
 	jne    18468 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()+0x58>
 	lock subl $0x1,0xc(%rdi)
 	je     18450 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()+0x40>
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
@@ -6838,15 +6838,15 @@
 	push   %r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	sub    $0x38,%rsp
 	mov    (%rsi),%rax
-	mov    0x9d75d(%rip),%rbx        
+	mov    0x9d765(%rip),%rbx        
 	mov    %dl,0xc(%rsp)
 	cmp    %rbx,%rax
 	je     18780 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x210>
 	mov    0x8(%rax),%eax
 	mov    %ecx,%ebp
 	cmp    $0x1,%eax
 	jne    18640 <torch::autograd::make_variable(at::Tensor, bool, bool)+0xd0>
@@ -6892,15 +6892,15 @@
 	lea    0x10(%rsp),%r14
 	mov    (%r15),%rax
 	mov    0xd8(%rax),%r8
 	mov    %r8,(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	mov    %r13,%rdi
 	mov    %rax,%rsi
-	mov    0x9d726(%rip),%rax        
+	mov    0x9d72e(%rip),%rax        
 	movq   $0x0,0x8(%rsi)
 	add    $0x10,%rax
 	movl   $0x0,0x10(%rsi)
 	mov    %rax,(%rsi)
 	call   11020 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::intrusive_ptr(c10::VariableVersion::VersionCounter*)@plt>
 	mov    (%rsp),%r8
 	movzbl %bpl,%ecx
@@ -7034,16 +7034,16 @@
 	call   104b0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, char const*)@plt>
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x1bde6(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%r15
 	call   102e0 <std::runtime_error::runtime_error(char const*)@plt>
-	mov    0x9d6a4(%rip),%rdx        
-	mov    0x9d54d(%rip),%rsi        
+	mov    0x9d6ac(%rip),%rdx        
+	mov    0x9d555(%rip),%rsi        
 	mov    %r15,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbp
 	jmp    188e5 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x375>
 	mov    %rax,%rbp
 	jmp    18905 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x395>
 	mov    0x28(%rsp),%rdi
@@ -7061,16 +7061,16 @@
 	call   10650 <_Unwind_Resume@plt>
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x1bd7a(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%r14
 	call   102e0 <std::runtime_error::runtime_error(char const*)@plt>
-	mov    0x9d638(%rip),%rdx        
-	mov    0x9d4e1(%rip),%rsi        
+	mov    0x9d640(%rip),%rdx        
+	mov    0x9d4e9(%rip),%rsi        
 	mov    %r14,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbp
 	jmp    189c4 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x454>
 	mov    %rax,%rbx
 	jmp    189ee <torch::autograd::make_variable(at::Tensor, bool, bool)+0x47e>
 	mov    %rax,%rbp
@@ -7349,20 +7349,20 @@
 std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long)>():
 	push   %r12
 	mov    $0x1,%r8d
 	mov    %rdi,%r12
 	mov    $0x4,%edx
 	push   %rbp
 	sub    $0xa8,%rsp
-	movq   0x9d0d0(%rip),%xmm0        # b5e10 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b0>
+	movq   0x9d0d8(%rip),%xmm0        # b5e18 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b8>
 	movq   0x9d250(%rip),%xmm1        # b5f98 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<long>()@@Base+0xa0878>
 	lea    0x50(%rsp),%rbp
 	mov    %rsp,%rcx
 	lea    0x10(%rsp),%rsi
-	movhps 0x9cf84(%rip),%xmm0        # b5ce0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0530>
+	movhps 0x9cf8c(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	movhps 0x9d245(%rip),%xmm1        # b5fa8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<long>()@@Base+0xa0868>
 	mov    %rbp,%rdi
 	movaps %xmm0,0x10(%rsp)
 	movaps %xmm0,0x20(%rsp)
 	movaps %xmm0,0x30(%rsp)
 	movaps %xmm1,0x40(%rsp)
 	movaps %xmm0,(%rsp)
@@ -7409,15 +7409,15 @@
 	mov    0x8(%rcx),%rdi
 	mov    -0x8(%rdi),%eax
 	cmp    $0x5,%eax
 	je     18ec0 <std::decay<c10::guts::infer_function_traits<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> > >::type::return_type>::type c10::impl::call_functor_with_args_from_stack_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false, 0ul, 1ul, 2ul, 3ul, at::Tensor, at::Tensor, at::Tensor, long>(c10::OperatorKernel*, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*, std::integer_sequence<unsigned long, 0ul, 1ul, 2ul, 3ul>, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long>*)+0xc0>
 	cmp    $0x6,%eax
 	jne    190d1 <std::decay<c10::guts::infer_function_traits<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> > >::type::return_type>::type c10::impl::call_functor_with_args_from_stack_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false, 0ul, 1ul, 2ul, 3ul, at::Tensor, at::Tensor, at::Tensor, long>(c10::OperatorKernel*, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*, std::integer_sequence<unsigned long, 0ul, 1ul, 2ul, 3ul>, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long>*)+0x2d1>
 	mov    -0x10(%rdi),%rax
-	cmp    0x9ceb0(%rip),%rax        
+	cmp    0x9ceb8(%rip),%rax        
 	mov    %rcx,%rbx
 	je     18fe8 <std::decay<c10::guts::infer_function_traits<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> > >::type::return_type>::type c10::impl::call_functor_with_args_from_stack_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false, 0ul, 1ul, 2ul, 3ul, at::Tensor, at::Tensor, at::Tensor, long>(c10::OperatorKernel*, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*, std::integer_sequence<unsigned long, 0ul, 1ul, 2ul, 3ul>, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long>*)+0x1e8>
 	test   %rax,%rax
 	je     18e5f <std::decay<c10::guts::infer_function_traits<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> > >::type::return_type>::type c10::impl::call_functor_with_args_from_stack_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false, 0ul, 1ul, 2ul, 3ul, at::Tensor, at::Tensor, at::Tensor, long>(c10::OperatorKernel*, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*, std::integer_sequence<unsigned long, 0ul, 1ul, 2ul, 3ul>, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long>*)+0x5f>
 	lock addl $0x1,0x8(%rax)
 	mov    -0x10(%rdi),%rax
 	test   %rax,%rax
@@ -7457,15 +7457,15 @@
 	mov    -0x30(%rdi),%rcx
 	cmpl   $0x1,-0x38(%rdi)
 	mov    %rcx,0x10(%rsp)
 	movq   $0x0,-0x30(%rdi)
 	movl   $0x0,-0x28(%rdi)
 	jne    19060 <std::decay<c10::guts::infer_function_traits<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> > >::type::return_type>::type c10::impl::call_functor_with_args_from_stack_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false, 0ul, 1ul, 2ul, 3ul, at::Tensor, at::Tensor, at::Tensor, long>(c10::OperatorKernel*, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*, std::integer_sequence<unsigned long, 0ul, 1ul, 2ul, 3ul>, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long>*)+0x260>
 	mov    -0x40(%rdi),%rsi
-	mov    0x9cdcb(%rip),%rdx        
+	mov    0x9cdd3(%rip),%rdx        
 	lea    0x48(%rsp),%rbp
 	mov    %r15,%r8
 	lea    0x40(%rsp),%r14
 	lea    0x38(%rsp),%rbx
 	movq   $0x0,-0x40(%rdi)
 	movl   $0x0,-0x38(%rdi)
 	mov    %r12,%rdi
@@ -7660,15 +7660,15 @@
 	cmp    $0x1a,%ecx
 	ja     19435 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x235>
 	mov    $0x1,%eax
 	shl    %cl,%eax
 	test   $0x7ddfdd4,%eax
 	je     19242 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x42>
 	mov    0x0(%rbp),%r13
-	cmp    0x9ca72(%rip),%r13        
+	cmp    0x9ca7a(%rip),%r13        
 	je     19242 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x42>
 	lea    0x8(%r13),%rax
 	mov    0x8(%r13),%edx
 	test   %edx,%edx
 	je     19238 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x38>
 	mov    0xc(%r13),%edx
 	test   %edx,%edx
@@ -7677,15 +7677,15 @@
 	lea    0x1a806(%rip),%rcx        
 	mov    $0x1e3,%edx
 	lea    0x1a912(%rip),%rsi        
 	lea    0x1a66a(%rip),%rdi        
 	call   104b0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x18(%rsp),%rax
-	mov    0x9ca24(%rip),%r13        
+	mov    0x9ca2c(%rip),%r13        
 	mov    %r15,0x8(%r12)
 	movl   $0x1,0x38(%rsp)
 	mov    %r13,0x18(%rsp)
 	mov    %rax,0x30(%rsp)
 	cmp    0x10(%r12),%r15
 	je     19380 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x180>
 	mov    0x38(%rsp),%eax
@@ -7843,15 +7843,15 @@
 __cudaUnregisterBinaryUtil():
 	mov    0x9d669(%rip),%rdi        
 	jmp    10210 <__cudaUnregisterFatBinary@plt>
 	nopl   0x0(%rax)
 
 0000000000019560 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0x9c8a0(%rip)        
+	cmpq   $0x0,0x9c8a8(%rip)        
 	je     19580 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    1958d <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -9248,15 +9248,15 @@
 	movaps %xmm0,0x10(%rsp)
 	jne    1afc0 <c10::detail::_str_wrapper<char const*, c10::ScalarType const&, char const*>::call(char const* const&, c10::ScalarType const&, char const* const&)+0x500>
 	mov    0x9b3c1(%rip),%rax        # b5fa0 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9b257(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9b25f(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9b3ad(%rip),%rax        # b5fc8 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -9436,48 +9436,48 @@
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 000000000001b000 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9adf1(%rip),%rax        
+	mov    0x9adf9(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 000000000001b020 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9add1(%rip),%rax        
+	mov    0x9add9(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 000000000001b050 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ada1(%rip),%rax        
+	mov    0x9ada9(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 000000000001b070 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ad81(%rip),%rax        
+	mov    0x9ad89(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
@@ -9490,15 +9490,15 @@
 :impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor):
 	push   %r12
 	mov    %rsi,%r8
 	mov    %rdi,%r12
 	push   %rbp
 	sub    $0x18,%rsp
 	mov    (%rcx),%rdx
-	mov    0x9ac31(%rip),%rax        
+	mov    0x9ac39(%rip),%rax        
 	lea    0x8(%rsp),%rbp
 	mov    %rax,(%rcx)
 	mov    %rbp,%rsi
 	mov    %rdx,0x8(%rsp)
 	mov    %rax,(%rsp)
 	call   *0x10(%r8)
 	mov    %rbp,%rdi
@@ -9524,15 +9524,15 @@
 :impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, at::Tensor (at::Tensor, at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor, at::Tensor):
 	push   %r13
 	mov    %rsi,%r9
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	sub    $0x20,%rsp
-	mov    0x9abc2(%rip),%rax        
+	mov    0x9abca(%rip),%rax        
 	mov    (%r8),%rsi
 	mov    (%rcx),%rdx
 	lea    0x10(%rsp),%rbp
 	lea    0x18(%rsp),%r13
 	mov    %rsi,0x10(%rsp)
 	mov    %r13,%rsi
 	mov    %rdx,0x18(%rsp)
@@ -9603,15 +9603,15 @@
 	cmp    $0x1a,%ecx
 	ja     1b481 <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0x2c1>
 	mov    $0x1,%eax
 	shl    %cl,%eax
 	test   $0x7ddfdd4,%eax
 	je     1b25b <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0x9b>
 	mov    0x0(%rbp),%r13
-	cmp    0x9aaa9(%rip),%r13        
+	cmp    0x9aab1(%rip),%r13        
 	je     1b25b <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0x9b>
 	lea    0x8(%r13),%rax
 	mov    0x8(%r13),%ecx
 	test   %ecx,%ecx
 	jne    1b398 <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0x1d8>
 	lock subl $0x1,(%rax)
 	je     1b3d0 <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0x210>
@@ -9644,15 +9644,15 @@
 	cmp    $0x1a,%ecx
 	ja     1b435 <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0x275>
 	mov    $0x1,%edx
 	shl    %cl,%edx
 	and    $0x7ddfdd4,%edx
 	je     1b2aa <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0xea>
 	mov    (%rbx),%rbp
-	cmp    0x9aa0b(%rip),%rbp        
+	cmp    0x9aa13(%rip),%rbp        
 	je     1b2aa <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0xea>
 	lea    0x8(%rbp),%rdx
 	mov    0x8(%rbp),%eax
 	test   %eax,%eax
 	je     1b2a0 <std::vector<c10::IValue, std::allocator<c10::IValue> >::_M_erase(__gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >, __gnu_cxx::__normal_iterator<c10::IValue*, std::vector<c10::IValue, std::allocator<c10::IValue> > >)+0xe0>
 	mov    0xc(%rbp),%eax
 	test   %eax,%eax
@@ -9789,15 +9789,15 @@
 	jne    1b6e0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x1f0>
 	mov    -0x10(%rdi),%rdx
 	cmpl   $0x1,-0x18(%rdi)
 	mov    %rdx,0x20(%rsp)
 	movq   $0x0,-0x10(%rdi)
 	movl   $0x0,-0x8(%rdi)
 	jne    1b6f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x200>
-	mov    0x9a7b0(%rip),%rbx        
+	mov    0x9a7b8(%rip),%rbx        
 	mov    %rcx,%rbp
 	mov    -0x20(%rdi),%rcx
 	lea    0x10(%rsp),%r14
 	lea    0x38(%rsp),%r13
 	lea    0x40(%rsp),%r12
 	movq   $0x0,-0x20(%rdi)
 	movl   $0x0,-0x18(%rdi)
@@ -9972,15 +9972,15 @@
 	push   %rbp
 	push   %rbx
 	sub    $0x38,%rsp
 	mov    0x8(%rcx),%rdi
 	cmpl   $0x1,-0x8(%rdi)
 	jne    1b970 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x190>
 	mov    -0x10(%rdi),%rdx
-	mov    0x9a4de(%rip),%rbx        
+	mov    0x9a4e6(%rip),%rbx        
 	mov    %rcx,%rbp
 	lea    0x8(%rsp),%r13
 	lea    0x20(%rsp),%r12
 	movq   $0x0,-0x10(%rdi)
 	movl   $0x0,-0x8(%rdi)
 	mov    %r12,%rsi
 	mov    %r13,%rdi
@@ -10248,15 +10248,15 @@
 __cudaUnregisterBinaryUtil():
 	mov    0x9afa9(%rip),%rdi        
 	jmp    10210 <__cudaUnregisterFatBinary@plt>
 	nopl   0x0(%rax)
 
 000000000001bcc0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0x9a140(%rip)        
+	cmpq   $0x0,0x9a148(%rip)        
 	je     1bce0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    1bced <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -10311,21 +10311,21 @@
 	nopl   (%rax)
 	mov    0xc(%rbp),%eax
 	lea    0xc(%rbp),%rbx
 	cmp    $0x1,%eax
 	je     1bdb3 <c10::SymInt::release_() [clone .part.0]+0xb3>
 	mov    0x0(%rbp),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9a0ad(%rip),%rax        
+	cmp    0x9a0b5(%rip),%rax        
 	jne    1be20 <c10::SymInt::release_() [clone .part.0]+0x120>
 	lock subl $0x1,(%rbx)
 	jne    1bd51 <c10::SymInt::release_() [clone .part.0]+0x51>
 	mov    0x0(%rbp),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x9a026(%rip),%rax        
+	cmp    0x9a02e(%rip),%rax        
 	jne    1be10 <c10::SymInt::release_() [clone .part.0]+0x110>
 	mov    0x9a14d(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,0x0(%rbp)
 	mov    0x8(%rbp),%eax
 	test   %eax,%eax
 	je     1bde8 <c10::SymInt::release_() [clone .part.0]+0xe8>
@@ -10588,22 +10588,22 @@
 	mov    $0x101,%edx
 	mov    %r14,%rsi
 	lea    -0x190(%rbp),%r12
 	mov    %r12,%rdi
 	call   10620 <at::_ops::sort_stable::call(at::Tensor const&, std::optional<bool>, long, bool)@plt>
 	mov    -0x190(%rbp),%rax
 	mov    %rax,-0x288(%rbp)
-	mov    0x99a5c(%rip),%rax        
+	mov    0x99a64(%rip),%rax        
 	mov    %rax,-0x190(%rbp)
 	lea    -0x188(%rbp),%rax
 	mov    %rax,%rdi
 	mov    %rax,-0x2f0(%rbp)
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    -0x190(%rbp),%rax
-	cmp    0x99a31(%rip),%rax        
+	cmp    0x99a39(%rip),%rax        
 	je     1c2c4 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x3f4>
 	lock subl $0x1,0x8(%rax)
 	je     1d693 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x17c3>
 	lea    -0x288(%rbp),%rax
 	lea    -0x1b0(%rbp),%rdi
 	xor    %edx,%edx
 	mov    %r13,%rsi
@@ -10629,15 +10629,15 @@
 	lea    0xb0(%rbx),%rdi
 	mov    $0x341,%edx
 	lea    0x16eee(%rip),%rsi        
 	call   101f0 <c10::SymBool::guard_bool(char const*, long) const@plt>
 	test   %al,%al
 	je     1c410 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x540>
 	mov    -0x1b0(%rbp),%rax
-	cmp    0x9998b(%rip),%rax        
+	cmp    0x99993(%rip),%rax        
 	mov    %rax,-0x190(%rbp)
 	je     1ce50 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0xf80>
 	mov    $0x1,%edx
 	lock xadd %edx,0x8(%rax)
 	test   %edx,%edx
 	jne    1c421 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x551>
 	lea    0x1834d(%rip),%r8        
@@ -10667,15 +10667,15 @@
 	nopw   0x0(%rax,%rax,1)
 	mov    -0x2d8(%rbp),%rsi
 	xor    %edx,%edx
 	mov    %r12,%rdi
 	call   10550 <at::TensorBase::__dispatch_contiguous(c10::MemoryFormat) const@plt>
 	mov    -0x190(%rbp),%rdx
 	mov    -0x1b0(%rbp),%rax
-	cmp    0x998b2(%rip),%rax        
+	cmp    0x998ba(%rip),%rax        
 	mov    %rdx,-0x280(%rbp)
 	je     1c44a <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x57a>
 	lock subl $0x1,0x8(%rax)
 	je     1d6dc <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x180c>
 	mov    0x0(%r13),%r14
 	movzbl 0xae(%r14),%eax
 	shr    $0x2,%al
@@ -11112,15 +11112,15 @@
 	mov    -0x218(%rbp),%rax
 	mov    -0x2e8(%rbp),%rsi
 	mov    %r12,%rdx
 	mov    $0x1,%ecx
 	mov    -0x2b0(%rbp),%rdi
 	movl   $0x5,-0x160(%rbp)
 	mov    %rax,-0x168(%rbp)
-	mov    0x99044(%rip),%rax        
+	mov    0x9904c(%rip),%rax        
 	mov    %rax,-0x218(%rbp)
 	call   10730 <at::Tensor::index(std::initializer_list<at::indexing::TensorIndex>) const@plt>
 	lea    -0x168(%rbp),%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	movabs $0xc000000000000000,%rax
 	cmp    %rax,-0x170(%rbp)
 	jl     1d2c0 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x13f0>
@@ -11187,15 +11187,15 @@
 	lea    0x183c3(%rip),%rdi        
 	call   11150 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	movzbl 0xad(%rdi),%eax
 	and    $0x1,%eax
 	jmp    1c347 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x477>
 	nop
-	mov    0x98e91(%rip),%rax        
+	mov    0x98e99(%rip),%rax        
 	mov    %rax,-0x280(%rbp)
 	jmp    1c44a <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x57a>
 	lea    -0x180(%rbp),%rdi
 	call   1bd00 <c10::SymInt::release_() [clone .part.0]>
 	jmp    1cb86 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0xcb6>
 	nopl   0x0(%rax)
 	xor    %edx,%edx
@@ -11290,15 +11290,15 @@
 	mov    -0x1d8(%rbp),%edx
 	mov    %r12,%r9
 	mov    -0x1e0(%rbp),%rsi
 	push   -0x218(%rbp)
 	mov    -0x1d0(%rbp),%rcx
 	mov    %edx,-0x1a8(%rbp)
 	mov    -0x1c8(%rbp),%r8d
-	mov    0x98de1(%rip),%rdi        # b5e68 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x978a8>
+	mov    0x98cf9(%rip),%rdi        # b5d80 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x977c0>
 	mov    %rsi,-0x1b0(%rbp)
 	mov    %rcx,-0x1c0(%rbp)
 	mov    %r8d,-0x1b8(%rbp)
 	call   111d0 <cudaLaunchKernel@plt>
 	jmp    1d231 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1361>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    -0x1f4(%rbp),%ecx
@@ -11354,15 +11354,15 @@
 	mov    -0x1d8(%rbp),%edx
 	mov    %r12,%r9
 	mov    -0x1e0(%rbp),%rsi
 	push   -0x218(%rbp)
 	mov    -0x1d0(%rbp),%rcx
 	mov    %edx,-0x1a8(%rbp)
 	mov    -0x1c8(%rbp),%r8d
-	mov    0x98dc9(%rip),%rdi        # b5fe0 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x97af0>
+	mov    0x98dd1(%rip),%rdi        # b5fe8 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x97af8>
 	mov    %rsi,-0x1b0(%rbp)
 	mov    %rcx,-0x1c0(%rbp)
 	mov    %r8d,-0x1b8(%rbp)
 	call   111d0 <cudaLaunchKernel@plt>
 	pop    %r10
 	pop    %r11
 	jmp    1c672 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x7a2>
@@ -11435,15 +11435,15 @@
 	mov    %al,-0x2a8(%rbp)
 	shr    $0x2,%al
 	and    $0x3,%eax
 	cmp    $0x1,%al
 	jbe    1bfc7 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0xf7>
 	mov    (%rcx),%rax
 	mov    0x30(%rax),%rdx
-	cmp    0x98c35(%rip),%rdx        
+	cmp    0x98c2d(%rip),%rdx        
 	jne    1d986 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1ab6>
 	mov    %rcx,%rdi
 	mov    $0x8,%ebx
 	call   *0x60(%rax)
 	cmp    $0x1,%rax
 	jle    1d9ba <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1aea>
 	mov    (%r15),%rax
@@ -11480,30 +11480,30 @@
 	lea    0x184c1(%rip),%rsi        
 	lea    0x17d22(%rip),%rdi        
 	call   11150 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, std::string const&)@plt>
 	nopl   0x0(%rax,%rax,1)
 	mov    (%r15),%rax
 	mov    %r15,%rdi
 	mov    0x30(%rax),%rdx
-	cmp    0x98b5f(%rip),%rdx        
+	cmp    0x98b57(%rip),%rdx        
 	jne    1d995 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1ac5>
 	call   *0x60(%rax)
 	xor    %ebx,%ebx
 	test   %rax,%rax
 	jle    1d9a1 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1ad1>
 	mov    (%r15),%rax
 	mov    %r15,%rdi
 	call   *0x40(%rax)
 	mov    (%rbx,%rax,1),%rbx
 	jmp    1c062 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x192>
 	nop
 	mov    (%r15),%rax
 	mov    %r15,%rdi
 	mov    0x30(%rax),%rdx
-	cmp    0x98b27(%rip),%rdx        
+	cmp    0x98b1f(%rip),%rdx        
 	jne    1d97d <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1aad>
 	call   *0x60(%rax)
 	xor    %r12d,%r12d
 	test   %rax,%rax
 	jle    1d9d6 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b06>
 	mov    (%r15),%rax
 	mov    %r15,%rdi
@@ -11574,15 +11574,15 @@
 	mov    %rcx,%r14
 	cmp    %rcx,%rdi
 	jne    1da1a <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b4a>
 	mov    -0x1d0(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r14,%rdi
 	je     1c23d <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x36d>
-	cmpq   $0x0,0x987d4(%rip)        
+	cmpq   $0x0,0x987dc(%rip)        
 	je     1da47 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b77>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1c23d <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x36d>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -11673,26 +11673,26 @@
 	mov    -0x1d8(%rbp),%edx
 	mov    %r12,%r9
 	mov    -0x1e0(%rbp),%rsi
 	push   -0x218(%rbp)
 	mov    -0x1d0(%rbp),%rcx
 	mov    %edx,-0x1a8(%rbp)
 	mov    -0x1c8(%rbp),%r8d
-	mov    0x984b1(%rip),%rdi        # b5d08 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97678>
+	mov    0x98489(%rip),%rdi        # b5ce0 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97650>
 	mov    %rsi,-0x1b0(%rbp)
 	mov    %rcx,-0x1c0(%rbp)
 	mov    %r8d,-0x1b8(%rbp)
 	call   111d0 <cudaLaunchKernel@plt>
 	jmp    1d231 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1361>
 	mov    (%rdi),%rax
 	call   *0x70(%rax)
 	jmp    1c1c7 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x2f7>
 	mov    (%r14),%rdx
 	mov    0x30(%rdx),%rax
-	cmp    0x98759(%rip),%rax        
+	cmp    0x98751(%rip),%rax        
 	jne    1d9ef <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b1f>
 	mov    %r14,%rdi
 	call   *0x60(%rdx)
 	mov    %rax,%rsi
 	xor    %ebx,%ebx
 	test   %rax,%rax
 	jle    1da09 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b39>
@@ -11784,15 +11784,15 @@
 	mov    %rax,%rbx
 	jmp    1c492 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x5c2>
 	xor    %edx,%edx
 	xor    %edi,%edi
 	call   111b0 <long c10::detail::maybe_wrap_dim_slow<long>(long, long, bool)@plt>
 	mov    %rax,%rbx
 	jmp    1d8a9 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x19d9>
-	cmpq   $0x0,0x983e6(%rip)        
+	cmpq   $0x0,0x983ee(%rip)        
 	je     1da55 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b85>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1d618 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1748>
 	lea    -0x210(%rbp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -12581,15 +12581,15 @@
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1e5b4 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)+0xc4>
 	push   0x28(%rsp)
-	mov    0x97a4f(%rip),%rdi        # b5fe0 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x97af0>
+	mov    0x97a57(%rip),%rdi        # b5fe8 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x97af8>
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -12627,15 +12627,15 @@
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1e684 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)+0xc4>
 	push   0x28(%rsp)
-	mov    0x97807(%rip),%rdi        # b5e68 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x978a8>
+	mov    0x9771f(%rip),%rdi        # b5d80 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x977c0>
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -12673,15 +12673,15 @@
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1e754 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)+0xc4>
 	push   0x28(%rsp)
-	mov    0x975d7(%rip),%rdi        # b5d08 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97678>
+	mov    0x975af(%rip),%rdi        # b5ce0 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97650>
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -12710,26 +12710,26 @@
 	jne    1e920 <c10::ValueError::~ValueError()+0x1c0>
 	mov    0x38(%r12),%rbp
 	test   %rbp,%rbp
 	jne    1e8f0 <c10::ValueError::~ValueError()+0x190>
 	mov    0x30(%r12),%rbp
 	test   %rbp,%rbp
 	je     1e7d0 <c10::ValueError::~ValueError()+0x70>
-	mov    0x97654(%rip),%r13        
+	mov    0x9765c(%rip),%r13        
 	test   %r13,%r13
 	je     1e888 <c10::ValueError::~ValueError()+0x128>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     1e89a <c10::ValueError::~ValueError()+0x13a>
 	mov    0x18(%r12),%r13
 	mov    0x10(%r12),%rbp
 	cmp    %rbp,%r13
 	je     1e80f <c10::ValueError::~ValueError()+0xaf>
-	cmpq   $0x0,0x97621(%rip)        
+	cmpq   $0x0,0x97629(%rip)        
 	lea    0xf(%rsp),%r14
 	je     1e848 <c10::ValueError::~ValueError()+0xe8>
 	xchg   %ax,%ax
 	mov    0x0(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    1e8d0 <c10::ValueError::~ValueError()+0x170>
@@ -12809,25 +12809,25 @@
 	cmp    %rbx,%rdi
 	jne    1e9b0 <c10::ValueError::~ValueError()+0x250>
 	mov    $0x8,%esi
 	mov    %rbp,%rdi
 	call   10de0 <operator delete(void*, unsigned long)@plt>
 	jmp    1e7a3 <c10::ValueError::~ValueError()+0x43>
 	nopl   0x0(%rax)
-	cmpq   $0x0,0x974e0(%rip)        
+	cmpq   $0x0,0x974e8(%rip)        
 	je     1e9a0 <c10::ValueError::~ValueError()+0x240>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1e795 <c10::ValueError::~ValueError()+0x35>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    1e795 <c10::ValueError::~ValueError()+0x35>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x974b0(%rip)        
+	cmpq   $0x0,0x974b8(%rip)        
 	je     1e990 <c10::ValueError::~ValueError()+0x230>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1e82e <c10::ValueError::~ValueError()+0xce>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -12844,15 +12844,15 @@
 	jmp    1e964 <c10::ValueError::~ValueError()+0x204>
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x8(%rax),%edx
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
 	jmp    1e934 <c10::ValueError::~ValueError()+0x1d4>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x97450(%rip)        
+	cmpq   $0x0,0x97458(%rip)        
 	je     1e9e0 <c10::ValueError::~ValueError()+0x280>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1e90a <c10::ValueError::~ValueError()+0x1aa>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -12883,26 +12883,26 @@
 	jne    1ebc0 <c10::ValueError::~ValueError()+0x1d0>
 	mov    0x38(%rbp),%r12
 	test   %r12,%r12
 	jne    1eb90 <c10::ValueError::~ValueError()+0x1a0>
 	mov    0x30(%rbp),%r12
 	test   %r12,%r12
 	je     1ea60 <c10::ValueError::~ValueError()+0x70>
-	mov    0x973c6(%rip),%r13        
+	mov    0x973ce(%rip),%r13        
 	test   %r13,%r13
 	je     1eb20 <c10::ValueError::~ValueError()+0x130>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     1eb36 <c10::ValueError::~ValueError()+0x146>
 	mov    0x18(%rbp),%r13
 	mov    0x10(%rbp),%r12
 	cmp    %r12,%r13
 	je     1ea9e <c10::ValueError::~ValueError()+0xae>
-	cmpq   $0x0,0x97393(%rip)        
+	cmpq   $0x0,0x9739b(%rip)        
 	lea    0xf(%rsp),%r14
 	je     1eae0 <c10::ValueError::~ValueError()+0xf0>
 	nopl   0x0(%rax)
 	mov    (%r12),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    1eb70 <c10::ValueError::~ValueError()+0x180>
@@ -12985,25 +12985,25 @@
 	cmp    %rbx,%rdi
 	jne    1ec58 <c10::ValueError::~ValueError()+0x268>
 	mov    $0x8,%esi
 	mov    %r12,%rdi
 	call   10de0 <operator delete(void*, unsigned long)@plt>
 	jmp    1ea32 <c10::ValueError::~ValueError()+0x42>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x97240(%rip)        
+	cmpq   $0x0,0x97248(%rip)        
 	je     1ec48 <c10::ValueError::~ValueError()+0x258>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1ea25 <c10::ValueError::~ValueError()+0x35>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    1ea25 <c10::ValueError::~ValueError()+0x35>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x97210(%rip)        
+	cmpq   $0x0,0x97218(%rip)        
 	je     1ec38 <c10::ValueError::~ValueError()+0x248>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1eabc <c10::ValueError::~ValueError()+0xcc>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13020,15 +13020,15 @@
 	jmp    1ec04 <c10::ValueError::~ValueError()+0x214>
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x8(%rax),%edx
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
 	jmp    1ebd4 <c10::ValueError::~ValueError()+0x1e4>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x971a8(%rip)        
+	cmpq   $0x0,0x971b0(%rip)        
 	je     1ec88 <c10::ValueError::~ValueError()+0x298>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1eba9 <c10::ValueError::~ValueError()+0x1b9>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13139,15 +13139,15 @@
 	call   111b0 <long c10::detail::maybe_wrap_dim_slow<long>(long, long, bool)@plt>
 	mov    0x40(%r12),%rsi
 	mov    %rax,%rbp
 	jmp    1edae <c10::TensorImpl::size(long) const+0x3e>
 	nopl   0x0(%rax)
 	mov    (%rdi),%rax
 	mov    0x30(%rax),%rdx
-	cmp    0x971fa(%rip),%rdx        
+	cmp    0x971f2(%rip),%rdx        
 	jne    1ee30 <c10::TensorImpl::size(long) const+0xc0>
 	call   *0x60(%rax)
 	mov    %rax,%rsi
 	neg    %rax
 	cmp    %rax,%rbp
 	jl     1ee40 <c10::TensorImpl::size(long) const+0xd0>
 	cmp    %rsi,%rbp
@@ -13324,15 +13324,15 @@
 	add    $0x10,%rax
 	mov    %rax,(%rbx)
 	call   11230 <std::locale::~locale()@plt>
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
-	cmpq   $0x0,0x96d28(%rip)        
+	cmpq   $0x0,0x96d30(%rip)        
 	je     1f100 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x70>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f0b7 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x27>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13364,15 +13364,15 @@
 	mov    %rbp,%rdi
 	mov    $0x50,%esi
 	call   10de0 <operator delete(void*, unsigned long)@plt>
 	add    $0x10,%rsp
 	pop    %rbp
 	ret
 	nopw   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x96c98(%rip)        
+	cmpq   $0x0,0x96ca0(%rip)        
 	je     1f190 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x80>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f137 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x27>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13405,15 +13405,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x170(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x180(%rsp)
 	mov    %rax,0x88(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x168(%rsp)
-	mov    0x96c45(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96c4d(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x160(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x30(%rsp)
 	mov    %rax,(%rsp)
 	add    %rbx,%rdi
@@ -13531,15 +13531,15 @@
 	jmp    1f2f3 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x153>
 	nopl   0x0(%rax)
 	lea    0x80(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    1f349 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x1a9>
 	nopl   (%rax)
-	cmpq   $0x0,0x969c0(%rip)        
+	cmpq   $0x0,0x969c8(%rip)        
 	je     1f470 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x2d0>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f394 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x1f4>
 	mov    %r13,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13604,15 +13604,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x170(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x180(%rsp)
 	mov    %rax,0x88(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x168(%rsp)
-	mov    0x968e5(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x968ed(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x160(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x30(%rsp)
 	mov    %rax,(%rsp)
 	add    %rbx,%rdi
@@ -13745,15 +13745,15 @@
 	jmp    1f653 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x153>
 	nopl   0x0(%rax)
 	lea    0x80(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    1f6c0 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x1c0>
 	nopl   (%rax)
-	cmpq   $0x0,0x96620(%rip)        
+	cmpq   $0x0,0x96628(%rip)        
 	je     1f810 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x310>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f70b <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x20b>
 	mov    %r13,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -14355,15 +14355,15 @@
 00000000000201d0 <at::indexing::TensorIndex::~TensorIndex()>:
 at::indexing::TensorIndex::~TensorIndex():
 	push   %rbp
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x38,%rsp
 	mov    0x28(%rdi),%rax
-	cmp    0x95b04(%rip),%rax        
+	cmp    0x95b0c(%rip),%rax        
 	je     201f1 <at::indexing::TensorIndex::~TensorIndex()+0x21>
 	lock subl $0x1,0x8(%rax)
 	je     205b0 <at::indexing::TensorIndex::~TensorIndex()+0x3e0>
 	movabs $0xc000000000000000,%rdx
 	mov    0x20(%rbx),%rax
 	cmp    %rdx,%rax
 	jl     20250 <at::indexing::TensorIndex::~TensorIndex()+0x80>
@@ -14406,21 +14406,21 @@
 	jne    20204 <at::indexing::TensorIndex::~TensorIndex()+0x34>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbp
 	cmp    $0x1,%eax
 	je     202ca <at::indexing::TensorIndex::~TensorIndex()+0xfa>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x95b9f(%rip),%rax        
+	cmp    0x95ba7(%rip),%rax        
 	jne    2060f <at::indexing::TensorIndex::~TensorIndex()+0x43f>
 	lock subl $0x1,0x0(%rbp)
 	jne    20204 <at::indexing::TensorIndex::~TensorIndex()+0x34>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95b10(%rip),%rax        
+	cmp    0x95b18(%rip),%rax        
 	jne    2063f <at::indexing::TensorIndex::~TensorIndex()+0x46f>
 	mov    0x95c33(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     20301 <at::indexing::TensorIndex::~TensorIndex()+0x131>
@@ -14459,21 +14459,21 @@
 	jne    2021b <at::indexing::TensorIndex::~TensorIndex()+0x4b>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbp
 	cmp    $0x1,%eax
 	je     203a2 <at::indexing::TensorIndex::~TensorIndex()+0x1d2>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x95ac7(%rip),%rax        
+	cmp    0x95acf(%rip),%rax        
 	jne    205fe <at::indexing::TensorIndex::~TensorIndex()+0x42e>
 	lock subl $0x1,0x0(%rbp)
 	jne    2021b <at::indexing::TensorIndex::~TensorIndex()+0x4b>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95a38(%rip),%rax        
+	cmp    0x95a40(%rip),%rax        
 	jne    20631 <at::indexing::TensorIndex::~TensorIndex()+0x461>
 	mov    0x95b5b(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     203d9 <at::indexing::TensorIndex::~TensorIndex()+0x209>
@@ -14512,21 +14512,21 @@
 	jne    20232 <at::indexing::TensorIndex::~TensorIndex()+0x62>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbp
 	cmp    $0x1,%eax
 	je     2047a <at::indexing::TensorIndex::~TensorIndex()+0x2aa>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x959ef(%rip),%rax        
+	cmp    0x959f7(%rip),%rax        
 	jne    205ed <at::indexing::TensorIndex::~TensorIndex()+0x41d>
 	lock subl $0x1,0x0(%rbp)
 	jne    20232 <at::indexing::TensorIndex::~TensorIndex()+0x62>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95960(%rip),%rax        
+	cmp    0x95968(%rip),%rax        
 	jne    20638 <at::indexing::TensorIndex::~TensorIndex()+0x468>
 	mov    0x95a83(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     204b1 <at::indexing::TensorIndex::~TensorIndex()+0x2e1>
@@ -14565,21 +14565,21 @@
 	jne    20248 <at::indexing::TensorIndex::~TensorIndex()+0x78>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbx
 	cmp    $0x1,%eax
 	je     20551 <at::indexing::TensorIndex::~TensorIndex()+0x381>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x95917(%rip),%rax        
+	cmp    0x9591f(%rip),%rax        
 	jne    20620 <at::indexing::TensorIndex::~TensorIndex()+0x450>
 	lock subl $0x1,(%rbx)
 	jne    20248 <at::indexing::TensorIndex::~TensorIndex()+0x78>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95889(%rip),%rax        
+	cmp    0x95891(%rip),%rax        
 	jne    20646 <at::indexing::TensorIndex::~TensorIndex()+0x476>
 	mov    0x959ac(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     20588 <at::indexing::TensorIndex::~TensorIndex()+0x3b8>
@@ -14810,15 +14810,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x180(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x178(%rsp)
-	mov    0x95488(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x95490(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x170(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x40(%rsp)
 	mov    %rax,(%rsp)
 	add    %rbp,%rdi
@@ -14931,15 +14931,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    0x95132(%rip),%rdi        
 	jne    20c8d <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x35d>
 	mov    0x18(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0x9511c(%rip),%rdi        
 	je     20952 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x22>
-	cmpq   $0x0,0x951ee(%rip)        
+	cmpq   $0x0,0x951f6(%rip)        
 	je     20ce1 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x3b1>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20952 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x22>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -14960,24 +14960,24 @@
 	call   10080 <std::basic_ios<char, std::char_traits<char> >::clear(std::_Ios_Iostate)@plt>
 	jmp    20ac2 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x192>
 	nopl   0x0(%rax)
 	lea    0x90(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    20b0e <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x1de>
-	cmpq   $0x0,0x95173(%rip)        
+	cmpq   $0x0,0x9517b(%rip)        
 	je     20cef <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x3bf>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20bfc <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x2cc>
 	lea    0x17(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    20bfc <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x2cc>
-	cmpq   $0x0,0x95148(%rip)        
+	cmpq   $0x0,0x95150(%rip)        
 	je     20cfa <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x3ca>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20b59 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x229>
 	mov    %r15,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15093,15 +15093,15 @@
 	xor    %edx,%edx
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %dx,0x478(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x398(%rsp)
-	mov    0x94fca(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94fd2(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x480(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x490(%rsp)
 	movq   $0x0,0x470(%rsp)
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x340(%rsp)
@@ -15221,15 +15221,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21c57 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xee7>
 	mov    0x70(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20de3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x73>
-	cmpq   $0x0,0x94ce3(%rip)        
+	cmpq   $0x0,0x94ceb(%rip)        
 	je     21db3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1043>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20de3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x73>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15248,15 +15248,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x5e0(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x4f8(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x5d8(%rsp)
-	mov    0x94ca2(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94caa(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x5f0(%rsp)
 	movq   $0x0,0x5d0(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x4a0(%rsp)
 	mov    %rax,0x28(%rsp)
@@ -15375,15 +15375,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21d12 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xfa2>
 	mov    0x78(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20df7 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x87>
-	cmpq   $0x0,0x949c3(%rip)        
+	cmpq   $0x0,0x949cb(%rip)        
 	je     21e07 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1097>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20df7 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x87>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15402,15 +15402,15 @@
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %si,0x1b8(%rsp)
 	xor    %esi,%esi
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0xd8(%rsp)
-	mov    0x94985(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9498d(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x1c0(%rsp)
 	mov    0x8(%rax),%rcx
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x1d0(%rsp)
 	movq   $0x0,0x1b0(%rsp)
 	mov    -0x18(%rcx),%rdi
 	mov    %rcx,0x80(%rsp)
@@ -15532,15 +15532,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21c25 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xeb5>
 	mov    0x60(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20da8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x38>
-	cmpq   $0x0,0x9468b(%rip)        
+	cmpq   $0x0,0x94693(%rip)        
 	je     21d9a <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x102a>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20da8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x38>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15559,15 +15559,15 @@
 	xor    %ecx,%ecx
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %cx,0x318(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x238(%rsp)
-	mov    0x9464d(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94655(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x320(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x330(%rsp)
 	movq   $0x0,0x310(%rsp)
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x1e0(%rsp)
@@ -15687,15 +15687,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21ce3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xf73>
 	mov    0x68(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20dba <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x4a>
-	cmpq   $0x0,0x9435d(%rip)        
+	cmpq   $0x0,0x94365(%rip)        
 	je     21dcf <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x105f>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20dba <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x4a>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15771,78 +15771,78 @@
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    21015 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x2a5>
 	nopl   (%rax)
 	lea    0x230(%rsp),%rsi
 	mov    %r15,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    21996 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xc26>
-	cmpq   $0x0,0x941db(%rip)        
+	cmpq   $0x0,0x941e3(%rip)        
 	je     21dc1 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1051>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     21763 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x9f3>
 	lea    0x1e0(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    21763 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x9f3>
-	cmpq   $0x0,0x941a9(%rip)        
+	cmpq   $0x0,0x941b1(%rip)        
 	je     21deb <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x107b>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2110b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x39b>
 	lea    0x1e0(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    2110b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x39b>
-	cmpq   $0x0,0x94177(%rip)        
+	cmpq   $0x0,0x9417f(%rip)        
 	je     21e23 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x10b3>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     216a9 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x939>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    216a9 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x939>
-	cmpq   $0x0,0x9414a(%rip)        
+	cmpq   $0x0,0x94152(%rip)        
 	je     21ddd <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x106d>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2105b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x2eb>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    2105b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x2eb>
-	cmpq   $0x0,0x9411d(%rip)        
+	cmpq   $0x0,0x94125(%rip)        
 	je     21e15 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x10a5>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     21a91 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xd21>
 	mov    0x28(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    21a91 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xd21>
-	cmpq   $0x0,0x940ee(%rip)        
+	cmpq   $0x0,0x940f6(%rip)        
 	je     21df9 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1089>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2142b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x6bb>
 	lea    0x1e0(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    2142b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x6bb>
-	cmpq   $0x0,0x940bc(%rip)        
+	cmpq   $0x0,0x940c4(%rip)        
 	je     21e31 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x10c1>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     219dc <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xc6c>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    219dc <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xc6c>
-	cmpq   $0x0,0x9408f(%rip)        
+	cmpq   $0x0,0x94097(%rip)        
 	je     21da8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1038>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2137b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x60b>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16019,15 +16019,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x180(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x178(%rsp)
-	mov    0x93dee(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93df6(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x170(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x40(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    %rbp,%rdi
@@ -16164,15 +16164,15 @@
 	jmp    22151 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x161>
 	nopl   0x0(%rax)
 	lea    0x90(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    221ce <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x1de>
 	nopl   (%rax)
-	cmpq   $0x0,0x93b18(%rip)        
+	cmpq   $0x0,0x93b20(%rip)        
 	je     22318 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x328>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     22219 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x229>
 	mov    %r14,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16480,15 +16480,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x180(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x178(%rsp)
-	mov    0x9367e(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93686(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x170(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x40(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    %rbp,%rdi
@@ -16625,15 +16625,15 @@
 	jmp    228c1 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x161>
 	nopl   0x0(%rax)
 	lea    0x90(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    2293e <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x1de>
 	nopl   (%rax)
-	cmpq   $0x0,0x933a8(%rip)        
+	cmpq   $0x0,0x933b0(%rip)        
 	je     22a88 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x328>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     22989 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x229>
 	mov    %r14,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16702,15 +16702,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x190(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x1a0(%rsp)
 	mov    %rax,0xa8(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x188(%rsp)
-	mov    0x932b6(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x932be(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x180(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x50(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    %rbp,%rdi
@@ -16886,15 +16886,15 @@
 	jmp    22cae <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x18e>
 	nopl   0x0(%rax)
 	lea    0xa0(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    22d67 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x247>
 	nopl   (%rax)
-	cmpq   $0x0,0x92f40(%rip)        
+	cmpq   $0x0,0x92f48(%rip)        
 	je     22ef0 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x3d0>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     22db2 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x292>
 	mov    %r14,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16952,15 +16952,15 @@
 	mov    0x8(%rcx),%rsi
 	mov    -0x8(%rsi),%eax
 	cmp    $0x3,%eax
 	je     23050 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0xd0>
 	cmp    $0x7,%eax
 	jne    235a1 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x621>
 	mov    -0x10(%rsi),%rdi
-	cmp    0x92d30(%rip),%rdi        
+	cmp    0x92d38(%rip),%rdi        
 	je     233b0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x430>
 	test   %rdi,%rdi
 	je     22fdc <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x5c>
 	lock addl $0x1,0x8(%rdi)
 	mov    -0x10(%rsi),%rdi
 	test   %rdi,%rdi
 	je     22fdc <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x5c>
@@ -17018,15 +17018,15 @@
 	cmp    $0x1a,%ecx
 	ja     23555 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x5d5>
 	mov    $0x1,%eax
 	shl    %cl,%eax
 	test   $0x7ddfdd4,%eax
 	je     2309a <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x11a>
 	mov    (%rbx),%r14
-	cmp    0x92c1b(%rip),%r14        
+	cmp    0x92c23(%rip),%r14        
 	je     2309a <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x11a>
 	lea    0x8(%r14),%rax
 	mov    0x8(%r14),%edx
 	test   %edx,%edx
 	je     23090 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x110>
 	mov    0xc(%r14),%edx
 	test   %edx,%edx
@@ -17035,15 +17035,15 @@
 	lea    0x109af(%rip),%rcx        
 	mov    $0x1e3,%edx
 	lea    0x10abb(%rip),%rsi        
 	lea    0x10813(%rip),%rdi        
 	call   104b0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, char const*)@plt>
 	nopl   0x0(%rax)
 	mov    0x18(%rsp),%rax
-	mov    0x92bcc(%rip),%rbx        
+	mov    0x92bd4(%rip),%rbx        
 	mov    %r15,0x8(%rbp)
 	movl   $0x1,0x38(%rsp)
 	mov    %rbx,0x18(%rsp)
 	mov    %rax,0x30(%rsp)
 	cmp    0x10(%rbp),%r15
 	je     231e8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x268>
 	mov    0x38(%rsp),%eax
@@ -17164,24 +17164,24 @@
 	mov    0x38(%rsp),%rax
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     23339 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x3b9>
 	mov    0x38(%rsp),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x92b30(%rip),%rax        
+	cmp    0x92b38(%rip),%rax        
 	jne    233f8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x478>
 	lock subl $0x1,0xc(%rdi)
 	jne    23044 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0xc4>
 	mov    0x38(%rsp),%rdi
 	test   %rdi,%rdi
 	je     23044 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0xc4>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x92a93(%rip),%rax        
+	cmp    0x92a9b(%rip),%rax        
 	jne    234a4 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x524>
 	mov    0x92bb6(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     2337e <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x3fe>
@@ -17221,24 +17221,24 @@
 	mov    0x18(%rsp),%rax
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     23441 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x4c1>
 	mov    0x18(%rsp),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x92a28(%rip),%rax        
+	cmp    0x92a30(%rip),%rax        
 	jne    23500 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x580>
 	lock subl $0x1,0xc(%rdi)
 	jne    23019 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x99>
 	mov    0x18(%rsp),%rdi
 	test   %rdi,%rdi
 	je     23019 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x99>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x9298b(%rip),%rax        
+	cmp    0x92993(%rip),%rax        
 	jne    2350c <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x58c>
 	mov    0x92aae(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     23486 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x506>
@@ -17409,21 +17409,21 @@
 std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double)>():
 	push   %r12
 	mov    $0x1,%r8d
 	mov    %rdi,%r12
 	mov    $0x3,%edx
 	push   %rbp
 	sub    $0x98,%rsp
-	movq   0x92670(%rip),%xmm0        # b5e10 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b0>
+	movq   0x92678(%rip),%xmm0        # b5e18 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b8>
 	movq   0x92848(%rip),%xmm1        # b5ff0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<double>()@@Base+0x97b80>
 	lea    0x40(%rsp),%rbp
 	mov    %rsp,%rcx
 	lea    0x10(%rsp),%rsi
-	movhps 0x92524(%rip),%xmm0        # b5ce0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0530>
-	movhps 0x927a5(%rip),%xmm1        # b5f68 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<double>()@@Base+0x97b18>
+	movhps 0x9252c(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
+	movhps 0x927ad(%rip),%xmm1        # b5f70 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<double>()@@Base+0x97b20>
 	mov    %rbp,%rdi
 	movaps %xmm0,0x10(%rsp)
 	movaps %xmm0,0x20(%rsp)
 	movaps %xmm1,0x30(%rsp)
 	movaps %xmm0,(%rsp)
 	call   10250 <c10::detail::infer_schema::make_function_schema(c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>, c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>)@plt>
 	mov    $0x48,%edi
@@ -17576,27 +17576,27 @@
 	movzbl 0x40(%rbp),%eax
 	test   %al,%al
 	jne    23b10 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x2c0>
 	cmpq   $0x0,0x20(%rbp)
 	je     23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
 	mov    0x20(%rbp),%r12
 	je     23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
-	mov    0x9239e(%rip),%rbx        
+	mov    0x923a6(%rip),%rbx        
 	test   %rbx,%rbx
 	je     23bf8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x3a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     23c0e <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x3be>
 	nopl   0x0(%rax,%rax,1)
 	cmpq   $0x0,0x10(%rbp)
 	je     23ac8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x278>
 	mov    0x10(%rbp),%r12
 	je     23ac8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x278>
-	mov    0x92364(%rip),%rbx        
+	mov    0x9236c(%rip),%rbx        
 	test   %rbx,%rbx
 	je     23ba8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x358>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     23bbe <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x36e>
 	nopw   0x0(%rax,%rax,1)
@@ -17627,15 +17627,15 @@
 	cmp    $0x1,%ecx
 	je     23b2f <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x2df>
 	mov    $0x1,%edx
 	shl    %cl,%edx
 	and    $0x7ddfdd4,%edx
 	je     23a56 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x206>
 	mov    0x30(%rbp),%r12
-	cmp    0x921ae(%rip),%r12        
+	cmp    0x921b6(%rip),%r12        
 	je     23a56 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x206>
 	lock subl $0x1,0x8(%r12)
 	jne    23a56 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x206>
 	mov    0xc(%r12),%edx
 	lea    0xc(%r12),%rbx
 	cmp    $0x1,%edx
 	je     23b6d <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x31d>
@@ -17692,15 +17692,15 @@
 	cmp    $0x1,%eax
 	jne    23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x18(%rax)
 	jmp    23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
 	nopl   0x0(%rax)
-	cmpq   $0x0,0x921b8(%rip)        
+	cmpq   $0x0,0x921c0(%rip)        
 	je     23c78 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x428>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     23add <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x28d>
 	lea    0x1f(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -18577,15 +18577,15 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0xa8(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x188(%rsp)
-	mov    0x9136c(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x91374(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x1a0(%rsp)
 	movq   $0x0,0x180(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x50(%rsp)
 	mov    %rbx,0x28(%rsp)
@@ -18704,15 +18704,15 @@
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %si,0x188(%rsp)
 	xor    %esi,%esi
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0xa8(%rsp)
-	mov    0x910ec(%rip),%rax        # b5e50 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x910f4(%rip),%rax        # b5e58 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x190(%rsp)
 	mov    0x8(%rax),%r13
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x1a0(%rsp)
 	movq   $0x0,0x180(%rsp)
 	mov    -0x18(%r13),%rdi
 	mov    %r13,0x50(%rsp)
@@ -18812,15 +18812,15 @@
 	mov    $0xce,%edx
 	lea    0x114f2(%rip),%rsi        
 	lea    0x11580(%rip),%rdi        
 	call   11150 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, std::string const&)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    (%r12),%rax
 	mov    0x30(%rax),%rdx
-	cmp    0x91061(%rip),%rdx        
+	cmp    0x91059(%rip),%rdx        
 	jne    25088 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x778>
 	mov    %r12,%rdi
 	xor    %ebx,%ebx
 	call   *0x60(%rax)
 	test   %rax,%rax
 	jle    25118 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x808>
 	mov    (%r12),%rax
@@ -18831,15 +18831,15 @@
 	movzbl 0xae(%r15),%edx
 	shr    $0x2,%dl
 	and    $0x3,%edx
 	jmp    24967 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x57>
 	nopl   0x0(%rax,%rax,1)
 	mov    (%r15),%rax
 	mov    0x30(%rax),%rdx
-	cmp    0x91012(%rip),%rdx        
+	cmp    0x9100a(%rip),%rdx        
 	jne    25070 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x760>
 	mov    %r15,%rdi
 	mov    $0x8,%ebx
 	call   *0x60(%rax)
 	cmp    $0x1,%rax
 	jle    250f8 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x7e8>
 	mov    (%r15),%rax
@@ -18889,15 +18889,15 @@
 	jmp    24967 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x57>
 	nopl   0x0(%rax)
 	lea    0xa0(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    24ed4 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x5c4>
 	nopl   (%rax)
-	cmpq   $0x0,0x90d38(%rip)        
+	cmpq   $0x0,0x90d40(%rip)        
 	je     2515a <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x84a>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     24cb2 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x3a2>
 	mov    %r15,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -18912,15 +18912,15 @@
 	nopl   0x0(%rax)
 	xor    %edx,%edx
 	mov    %rax,%rsi
 	xor    %edi,%edi
 	call   111b0 <long c10::detail::maybe_wrap_dim_slow<long>(long, long, bool)@plt>
 	lea    0x0(,%rax,8),%rbx
 	jmp    24f9e <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x68e>
-	cmpq   $0x0,0x90ccf(%rip)        
+	cmpq   $0x0,0x90cd7(%rip)        
 	je     25168 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x858>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     24f13 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x603>
 	mov    %r15,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -19083,19 +19083,19 @@
 std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor)>():
 	push   %r12
 	mov    $0x1,%r8d
 	mov    %rdi,%r12
 	mov    $0x1,%edx
 	push   %rbp
 	sub    $0x78,%rsp
-	movq   0x90a83(%rip),%xmm0        # b5e10 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b0>
+	movq   0x90a8b(%rip),%xmm0        # b5e18 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06b8>
 	lea    0x20(%rsp),%rbp
 	lea    0x10(%rsp),%rcx
 	mov    %rsp,%rsi
-	movhps 0x9093f(%rip),%xmm0        # b5ce0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0530>
+	movhps 0x90947(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	mov    %rbp,%rdi
 	movaps %xmm0,(%rsp)
 	movaps %xmm0,0x10(%rsp)
 	call   10250 <c10::detail::infer_schema::make_function_schema(c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>, c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>)@plt>
 	mov    $0x48,%edi
 	call   10b80 <operator new(unsigned long)@plt>
 	movzwl 0x60(%rsp),%edx
@@ -19121,15 +19121,15 @@
 	call   11180 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000025420 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0x909e0(%rip)        
+	cmpq   $0x0,0x909e8(%rip)        
 	je     25440 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    2544d <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -19228,15 +19228,15 @@
 	push   %r12
 	push   %rbp
 	sub    $0x18,%rsp
 	call   111f0 <Py_GetVersion@plt>
 	cmpb   $0x33,(%rax)
 	mov    %rax,%rcx
 	je     255e0 <PyInit__C+0x40>
-	mov    0x908a5(%rip),%rax        
+	mov    0x908ad(%rip),%rax        
 	lea    0x117f0(%rip),%rdx        
 	lea    0x117f7(%rip),%rsi        
 	mov    (%rax),%rdi
 	xor    %eax,%eax
 	call   112f0 <PyErr_Format@plt>
 	xor    %eax,%eax
 	add    $0x18,%rsp
@@ -19326,15 +19326,15 @@
 
 0000000000025740 <pybind11::cast_error::set_error() const>:
 pybind11::cast_error::set_error() const:
 	sub    $0x8,%rsp
 	mov    (%rdi),%rax
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x905ac(%rip),%rax        
+	mov    0x905b4(%rip),%rax        
 	mov    (%rax),%rdi
 	add    $0x8,%rsp
 	jmp    10c40 <PyErr_SetString@plt>
 
 0000000000025760 <pybind11::cast_error::~cast_error()>:
 pybind11::cast_error::~cast_error():
 	lea    0x90281(%rip),%rax        
@@ -19472,15 +19472,15 @@
 	mov    (%rax),%rbx
 	lea    0x18(%r13),%rdx
 	mov    %rdx,(%rax)
 	mov    0x8(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    25958 <pybind11_object_init+0x88>
-	mov    0x9048f(%rip),%rax        
+	mov    0x90497(%rip),%rax        
 	mov    %rbx,%rsi
 	mov    (%rax),%rdi
 	call   10c40 <PyErr_SetString@plt>
 	lea    -0x18(%rbx),%rdi
 	cmp    %r13,%rdi
 	jne    25968 <pybind11_object_init+0x98>
 	add    $0x18,%rsp
@@ -19533,15 +19533,15 @@
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	mov    0x10(%rdi),%r12
 	mov    %rax,(%rdi)
 	test   %r12,%r12
 	je     25a07 <pybind11::error_already_set::~error_already_set()+0x37>
-	mov    0x90417(%rip),%rbx        
+	mov    0x9041f(%rip),%rbx        
 	test   %rbx,%rbx
 	je     25a20 <pybind11::error_already_set::~error_already_set()+0x50>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     25a32 <pybind11::error_already_set::~error_already_set()+0x62>
 	mov    %rbp,%rdi
@@ -19584,15 +19584,15 @@
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	mov    0x10(%rdi),%r12
 	mov    %rax,(%rdi)
 	test   %r12,%r12
 	je     25aa7 <pybind11::error_already_set::~error_already_set()+0x37>
-	mov    0x90377(%rip),%rbx        
+	mov    0x9037f(%rip),%rbx        
 	test   %rbx,%rbx
 	je     25ab8 <pybind11::error_already_set::~error_already_set()+0x48>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     25aca <pybind11::error_already_set::~error_already_set()+0x5a>
 	pop    %rbx
@@ -22676,15 +22676,15 @@
 	lea    -0x18(%rax),%rdx
 	cmp    %rbx,%rdx
 	jne    28890 <pybind11::detail::error_fetch_and_normalize::format_value_and_trace() const+0x450>
 	mov    0x14(%rsp),%r8d
 	mov    $0x10,%edx
 	mov    %r14,%rdi
 	xor    %eax,%eax
-	mov    0x8d70f(%rip),%rsi        
+	mov    0x8d717(%rip),%rsi        
 	lea    0xb1da(%rip),%rcx        
 	call   25460 <std::string __gnu_cxx::__to_xstring<std::string, char>(int (*)(char*, unsigned long, char const*, __va_list_tag*), unsigned long, char const*, ...) [clone .constprop.0]>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	call   106f0 <std::string::append(std::string const&)@plt>
 	mov    0x68(%rsp),%rax
 	lea    -0x18(%rax),%rdi
@@ -23079,54 +23079,54 @@
 	lea    0xdc99(%rip),%rdx        
 	mov    %r12,%rdi
 	movslq (%rdx,%rax,4),%rax
 	add    %rdx,%rax
 	jmp    *%rax
 	mov    %r12,%rdi
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d04a(%rip),%rax        
+	mov    0x8d052(%rip),%rax        
 	lea    0xdc57(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	call   11030 <__cxa_end_catch@plt>
 	add    $0x18,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	mov    %rax,%rbp
 	jmp    28d2d <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0xdd>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d132(%rip),%rdx        
+	mov    0x8d13a(%rip),%rdx        
 	mov    0x8d043(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28d0f <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0xbf>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x8cfdd(%rip),%rax        
+	mov    0x8cfe5(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	jmp    28dee <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x19e>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d0ca(%rip),%rdx        
+	mov    0x8d0d2(%rip),%rdx        
 	mov    0x8d12b(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23138,15 +23138,15 @@
 	call   *0x10(%rax)
 	mov    %rax,%rsi
 	mov    0x8d115(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d074(%rip),%rdx        
+	mov    0x8d07c(%rip),%rdx        
 	mov    0x8d24d(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23167,15 +23167,15 @@
 	mov    %rax,%rbp
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	jmp    29075 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x425>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cff9(%rip),%rdx        
+	mov    0x8d001(%rip),%rdx        
 	mov    0x8cf2a(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23187,15 +23187,15 @@
 	call   *0x10(%rax)
 	mov    %rax,%rsi
 	mov    0x8d124(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cfa3(%rip),%rdx        
+	mov    0x8cfab(%rip),%rdx        
 	mov    0x8d0ac(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23210,15 +23210,15 @@
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
 	mov    %rax,%r12
 	test   %rax,%rax
 	je     28ef9 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x2a9>
-	mov    0x8cf45(%rip),%rdx        
+	mov    0x8cf4d(%rip),%rdx        
 	mov    %rax,%rdi
 	mov    $0xfffffffffffffffe,%rcx
 	lea    0x8ca7c(%rip),%rsi        
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28ef9 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x2a9>
@@ -23233,15 +23233,15 @@
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cee4(%rip),%rdx        
+	mov    0x8ceec(%rip),%rdx        
 	mov    0x8cfbd(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23253,15 +23253,15 @@
 	call   *0x10(%rax)
 	mov    %rax,%rsi
 	mov    0x8cf17(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8ce8e(%rip),%rdx        
+	mov    0x8ce96(%rip),%rdx        
 	mov    0x8cf37(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23275,30 +23275,30 @@
 	mov    0x8cec1(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	mov    %rax,%rbp
 	jmp    290d6 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x486>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8ce30(%rip),%rdx        
+	mov    0x8ce38(%rip),%rdx        
 	mov    $0xfffffffffffffffe,%rcx
 	lea    0x8c9b2(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%rbx
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     29011 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x3c1>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    0x8(%rbx),%rdi
 	call   28bc0 <pybind11::detail::error_fetch_and_normalize::restore()>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cded(%rip),%rdx        
+	mov    0x8cdf5(%rip),%rdx        
 	mov    0x8cd2e(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23318,15 +23318,15 @@
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	jmp    290e8 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x498>
 	call   100c0 <__cxa_begin_catch@plt>
 	mov    %rbp,%rsi
 	mov    %rax,%rdi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
-	mov    0x8cc62(%rip),%rax        
+	mov    0x8cc6a(%rip),%rax        
 	lea    0xd84b(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	mov    %rax,%rbp
 	jmp    290bc <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x46c>
 	mov    %rax,%rbp
@@ -24165,15 +24165,15 @@
 	mov    %r15,%rdi
 	call   25cc0 <pybind11::handle::dec_ref() const &>
 	mov    0x8cf41(%rip),%rax        
 	mov    %rbx,0x1c0(%rbp)
 	mov    (%rax),%r14
 	jmp    2996d <pybind11::detail::get_internals()+0x13d>
 	xchg   %ax,%ax
-	mov    0x8c031(%rip),%rax        
+	mov    0x8c039(%rip),%rax        
 	lea    0xcbb2(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   25d80 <pybind11::raise_from(_object*, char const*)>
 	mov    $0x18,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	mov    %rax,%rdi
 	mov    %rax,%rbp
@@ -24201,15 +24201,15 @@
 	mov    %rdx,(%rax)
 	call   11c53 <pybind11::pybind11_fail(std::string const&)>
 	nopl   0x0(%rax)
 	movq   $0x0,0x348(%rbx)
 	jmp    29e54 <pybind11::detail::get_internals()+0x624>
 	movq   $0x0,0x348(%rbp)
 	jmp    29d48 <pybind11::detail::get_internals()+0x518>
-	mov    0x8bf71(%rip),%rax        
+	mov    0x8bf79(%rip),%rax        
 	lea    0xcb62(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   25d80 <pybind11::raise_from(_object*, char const*)>
 	mov    $0x18,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	mov    %rax,%rdi
 	mov    %rax,%rbp
@@ -27057,15 +27057,15 @@
 	mov    %ax,0x5c(%r15)
 	mov    0x78(%r15),%rax
 	test   %rax,%rax
 	je     2cd7e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9ee>
 	mov    0x8(%rax),%rdi
 	cmp    0x8928f(%rip),%rdi        
 	je     2d358 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0xfc8>
-	mov    0x89402(%rip),%rsi        
+	mov    0x8940a(%rip),%rsi        
 	cmp    %rsi,%rdi
 	je     2cd70 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9e0>
 	call   10140 <PyType_IsSubtype@plt>
 	mov    %eax,%r8d
 	mov    0x78(%r15),%rax
 	test   %r8d,%r8d
 	jne    2cd70 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9e0>
@@ -27198,15 +27198,15 @@
 	cmpq   $0x0,0x8(%rsp)
 	jne    2ccb3 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x923>
 	test   %al,%al
 	jne    2d3f0 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x1060>
 	mov    0x8(%rsp),%r8
 	movzbl %al,%eax
 	lea    0xa0(%rsp),%r14
-	mov    0x890de(%rip),%rsi        
+	mov    0x890e6(%rip),%rsi        
 	lea    0xa326(%rip),%rcx        
 	mov    $0x20,%edx
 	mov    %r14,%rdi
 	sub    %rax,%r8
 	xor    %eax,%eax
 	call   25460 <std::string __gnu_cxx::__to_xstring<std::string, char>(int (*)(char*, unsigned long, char const*, __va_list_tag*), unsigned long, char const*, ...) [clone .constprop.0]>
 	mov    $0x3,%ecx
@@ -27310,15 +27310,15 @@
 	je     2cfbd <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0xc2d>
 	test   %r12d,%r12d
 	jne    2d150 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0xdc0>
 	cmpq   $0x0,0x8(%rsp)
 	lea    0x78(%rsp),%rbp
 	je     2cf7d <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0xbed>
 	add    $0x1,%r12d
-	mov    0x88ebb(%rip),%rsi        
+	mov    0x88ec3(%rip),%rsi        
 	mov    %r14,%rdi
 	xor    %eax,%eax
 	mov    %r12d,%r8d
 	lea    0x697e(%rip),%rcx        
 	mov    $0x10,%edx
 	call   25460 <std::string __gnu_cxx::__to_xstring<std::string, char>(int (*)(char*, unsigned long, char const*, __va_list_tag*), unsigned long, char const*, ...) [clone .constprop.0]>
 	mov    $0x2,%edx
@@ -27526,15 +27526,15 @@
 	cmp    %rbp,%rax
 	jne    2cc5e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x8ce>
 	jmp    2d030 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0xca0>
 	xchg   %ax,%ax
 	mov    0x18(%rax),%rdi
 	test   %rdi,%rdi
 	je     2cd7e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9ee>
-	mov    0x88c8c(%rip),%rax        
+	mov    0x88c94(%rip),%rax        
 	cmp    %rax,0x8(%rdi)
 	jne    2cd7e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9ee>
 	mov    %rdi,0xc0(%rsp)
 	addq   $0x1,(%rdi)
 	call   10b50 <PyCapsule_GetName@plt>
 	test   %rax,%rax
 	je     2dad7 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x1747>
@@ -27559,15 +27559,15 @@
 	jmp    2c844 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x4b4>
 	nopl   0x0(%rax)
 	mov    0x10(%rax),%rax
 	mov    %rax,0x78(%r15)
 	test   %rax,%rax
 	je     2cd7e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9ee>
 	mov    0x8(%rax),%rdi
-	mov    0x88ac4(%rip),%rsi        
+	mov    0x88acc(%rip),%rsi        
 	cmp    %rsi,%rdi
 	jne    2ca3f <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x6af>
 	jmp    2cd70 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9e0>
 	nopw   0x0(%rax,%rax,1)
 	lea    0x80(%rsp),%rdi
 	mov    %r14,%rdx
 	call   110a0 <void std::vector<char*, std::allocator<char*> >::_M_realloc_insert<char* const&>(__gnu_cxx::__normal_iterator<char**, std::vector<char*, std::allocator<char*> > >, char* const&)@plt>
@@ -28869,15 +28869,15 @@
 	nopl   0x0(%rax)
 	mov    0x0(%r13),%rax
 	lea    0x17(%rsp),%rbp
 	lea    0x18(%rsp),%rdi
 	mov    %rbp,%rdx
 	mov    0x18(%rax),%rsi
 	call   10a70 <std::basic_string<char, std::char_traits<char>, std::allocator<char> >::basic_string(char const*, std::allocator<char> const&)@plt>
-	mov    0x87367(%rip),%rax        
+	mov    0x8736f(%rip),%rax        
 	mov    0x18(%rsp),%rdx
 	lea    0x8813(%rip),%rsi        
 	mov    (%rax),%rdi
 	xor    %eax,%eax
 	call   112f0 <PyErr_Format@plt>
 	mov    0x18(%rsp),%rax
 	lea    -0x18(%rax),%rdi
@@ -30113,15 +30113,15 @@
 	mov    $0x10,%edi
 	lea    0x18(%rsp),%r12
 	movq   $0x0,0x10(%rsp)
 	call   10d60 <__cxa_allocate_exception@plt>
 	xor    %r8d,%r8d
 	mov    $0x20,%edx
 	mov    %r12,%rdi
-	mov    0x86076(%rip),%rsi        
+	mov    0x8607e(%rip),%rsi        
 	mov    %rax,%rbp
 	xor    %eax,%eax
 	lea    0x72b9(%rip),%rcx        
 	call   25460 <std::string __gnu_cxx::__to_xstring<std::string, char>(int (*)(char*, unsigned long, char const*, __va_list_tag*), unsigned long, char const*, ...) [clone .constprop.0]>
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
 	call   26040 <pybind11::cast_error_unable_to_convert_call_arg(std::string const&)>
@@ -30184,15 +30184,15 @@
 	jne    2fe88 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x98>
 	movq   $0x0,0x100(%rsp)
 	pxor   %xmm0,%xmm0
 	movq   $0x0,0x108(%rsp)
 	movaps %xmm0,0x110(%rsp)
 	testb  $0x1,0x59(%rax)
 	je     30b83 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0xd93>
-	mov    0x85f63(%rip),%rax        
+	mov    0x85f6b(%rip),%rax        
 	lea    0x7694(%rip),%rsi        
 	xor    %r13d,%r13d
 	mov    (%rax),%rdi
 	call   10c40 <PyErr_SetString@plt>
 	add    $0x208,%rsp
 	mov    %r13,%rax
 	pop    %rbx
@@ -30997,15 +30997,15 @@
 	mov    0x80(%r13),%r13
 	test   %r13,%r13
 	je     318b9 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x1ac9>
 	add    $0x1,%ebx
 	mov    0x28(%rsp),%rdi
 	mov    $0x10,%edx
 	xor    %eax,%eax
-	mov    0x84f16(%rip),%rsi        
+	mov    0x84f1e(%rip),%rsi        
 	mov    %ebx,%r8d
 	lea    0x29de(%rip),%rcx        
 	call   25460 <std::string __gnu_cxx::__to_xstring<std::string, char>(int (*)(char*, unsigned long, char const*, __va_list_tag*), unsigned long, char const*, ...) [clone .constprop.0]>
 	mov    0x28(%rsp),%rdi
 	mov    $0x4,%ecx
 	lea    0x65f6(%rip),%rdx        
 	xor    %esi,%esi
@@ -31267,15 +31267,15 @@
 	and    $0x1,%eax
 	jmp    30b68 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0xd78>
 	movabs $0xfffffffffffffff,%rax
 	cmp    %rax,%rdx
 	cmova  %rax,%rdx
 	lea    0x0(,%rdx,8),%r13
 	jmp    30a01 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0xc11>
-	mov    0x84b32(%rip),%rax        
+	mov    0x84b3a(%rip),%rax        
 	addq   $0x1,(%rax)
 	mov    %rax,%r13
 	jmp    2fe6f <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x7f>
 	shr    $0x2,%al
 	and    $0x1,%eax
 	jmp    30c4d <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0xe5d>
 	mov    0x18(%rsp),%r13
@@ -31673,15 +31673,15 @@
 	call   110b0 <std::string::find(char const*, unsigned long, unsigned long) const@plt>
 	cmp    $0xffffffffffffffff,%rax
 	je     31cf3 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x1f03>
 	lea    0x58b5(%rip),%rsi        
 	mov    %r15,%rdi
 	call   10f40 <std::string::operator+=(char const*)@plt>
 	call   10a00 <PyErr_Occurred@plt>
-	mov    0x840c1(%rip),%rdx        
+	mov    0x840c9(%rip),%rdx        
 	mov    0x80(%rsp),%rsi
 	mov    (%rdx),%rdi
 	test   %rax,%rax
 	je     3216e <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x237e>
 	call   25d80 <pybind11::raise_from(_object*, char const*)>
 	lea    0x88(%rsp),%rdi
 	call   25cc0 <pybind11::handle::dec_ref() const &>
@@ -31773,15 +31773,15 @@
 	mov    $0x5,%ecx
 	lea    0x55c0(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   110b0 <std::string::find(char const*, unsigned long, unsigned long) const@plt>
 	cmp    $0xffffffffffffffff,%rax
 	jne    32042 <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x2252>
 	call   10a00 <PyErr_Occurred@plt>
-	mov    0x83e89(%rip),%rdx        
+	mov    0x83e91(%rip),%rdx        
 	mov    0x190(%rsp),%rsi
 	mov    (%rdx),%rdi
 	test   %rax,%rax
 	je     321ad <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x23bd>
 	call   25d80 <pybind11::raise_from(_object*, char const*)>
 	mov    0x190(%rsp),%rax
 	lea    -0x18(%rax),%rdi
@@ -31997,15 +31997,15 @@
 	test   %al,%al
 	jne    323db <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x25eb>
 	call   29830 <pybind11::detail::get_internals()>
 	lea    0x150(%rax),%rdi
 	call   26180 <pybind11::detail::apply_exception_translators(std::forward_list<void (*)(std::__exception_ptr::exception_ptr), std::allocator<void (*)(std::__exception_ptr::exception_ptr)> >&)>
 	test   %al,%al
 	jne    323db <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x25eb>
-	mov    0x83b9f(%rip),%rax        
+	mov    0x83ba7(%rip),%rax        
 	lea    0x5328(%rip),%rsi        
 	mov    (%rax),%rdi
 	call   10c40 <PyErr_SetString@plt>
 	jmp    323db <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x25eb>
 	mov    %rbp,%rdi
 	call   100c0 <__cxa_begin_catch@plt>
 	mov    0x8(%rax),%rdi
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,12 +1,12 @@
 
 Hex dump of section '.rodata':
   0x00033000 4e594900 00000000 2f5f5f77 2f5f7465 NYI...../__w/_te
   0x00033010 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033020 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00033020 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00033030 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033040 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033050 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00033060 72652f53 796d4e6f 6465496d 706c2e68 re/SymNodeImpl.h
   0x00033070 00686173 5f68696e 7400626f 6f6c5f00 .has_hint.bool_.
   0x00033080 696e745f 00677561 72645f66 6c6f6174 int_.guard_float
   0x00033090 00677561 72645f62 6f6f6c00 67756172 .guard_bool.guar
@@ -32,16 +32,16 @@
   0x000331d0 77007472 75656469 76006d75 6c007375 w.truediv.mul.su
   0x000331e0 62006164 64006973 5f666c6f 61740069 b.add.is_float.i
   0x000331f0 735f626f 6f6c0069 735f696e 74007465 s_bool.is_int.te
   0x00033200 6e736f72 20646f65 73206e6f 74206861 nsor does not ha
   0x00033210 76652061 20646576 69636500 64657669 ve a device.devi
   0x00033220 63655f64 65666175 6c740000 00000000 ce_default......
   0x00033230 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00033240 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x00033250 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x00033240 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x00033250 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x00033260 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00033270 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00033280 652f6331 302f636f 72652f54 656e736f e/c10/core/Tenso
   0x00033290 72496d70 6c2e6800 63756461 4572726f rImpl.h.cudaErro
   0x000332a0 725f7420 6670365f 6c696e65 61725f6b r_t fp6_linear_k
   0x000332b0 65726e65 6c286375 64615374 7265616d ernel(cudaStream
   0x000332c0 5f742c20 636f6e73 74207569 6e74342a _t, const uint4*
@@ -148,24 +148,24 @@
   0x00033910 69766550 74720072 65636c61 696d0000 ivePtr.reclaim..
   0x00033920 73746174 69635f63 6173743c 75696e74 static_cast<uint
   0x00033930 33325f74 3e287461 6729203c 206b4e75 32_t>(tag) < kNu
   0x00033940 6d546167 7320494e 5445524e 414c2041 mTags INTERNAL A
   0x00033950 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00033960 222f5f5f 772f5f74 656d702f 636f6e64 "/__w/_temp/cond
   0x00033970 615f656e 7669726f 6e6d656e 745f3932 a_environment_92
-  0x00033980 30303230 32373636 2f6c6962 2f707974 00202766/lib/pyt
+  0x00033980 31363635 33373035 2f6c6962 2f707974 16653705/lib/pyt
   0x00033990 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
   0x000339a0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x000339b0 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x000339c0 6c75652e 68223a31 3331352c 20706c65 lue.h":1315, ple
   0x000339d0 61736520 7265706f 72742061 20627567 ase report a bug
   0x000339e0 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x000339f0 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00033a00 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x00033a10 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x00033a00 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x00033a10 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x00033a20 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00033a30 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00033a40 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00033a50 75652e68 00000000 54546172 67657420 ue.h....TTarget 
   0x00033a60 76696f6c 61746573 20746865 20696e76 violates the inv
   0x00033a70 61726961 6e742074 68617420 72656663 ariant that refc
   0x00033a80 6f756e74 203e2030 20203d3e 20207765 ount > 0  =>  we
@@ -176,39 +176,39 @@
   0x00033ad0 722d3e72 6566636f 756e745f 2e6c6f61 r->refcount_.loa
   0x00033ae0 64282920 3d3d2030 207c7c20 6f776e69 d() == 0 || owni
   0x00033af0 6e675f70 74722d3e 7765616b 636f756e ng_ptr->weakcoun
   0x00033b00 745f2e6c 6f616428 2920494e 5445524e t_.load() INTERN
   0x00033b10 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00033b20 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x00033b30 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x00033b40 745f3932 30303230 32373636 2f6c6962 t_9200202766/lib
+  0x00033b40 745f3932 31363635 33373035 2f6c6962 t_9216653705/lib
   0x00033b50 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x00033b60 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00033b70 6e636c75 64652f63 31302f75 74696c2f nclude/c10/util/
   0x00033b80 696e7472 75736976 655f7074 722e6822 intrusive_ptr.h"
   0x00033b90 3a343833 2c20706c 65617365 20726570 :483, please rep
   0x00033ba0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x00033bb0 6f726368 2e200000 2f5f5f77 2f5f7465 orch. ../__w/_te
   0x00033bc0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033bd0 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00033bd0 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00033be0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033bf0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033c00 682f696e 636c7564 652f6331 302f7574 h/include/c10/ut
   0x00033c10 696c2f69 6e747275 73697665 5f707472 il/intrusive_ptr
   0x00033c20 2e680000 00000000 4f706572 61746f72 .h......Operator
   0x00033c30 73207461 6b696e67 2054656e 736f724f s taking TensorO
   0x00033c40 7074696f 6e732063 616e6e6f 74207461 ptions cannot ta
   0x00033c50 6b652061 2054656e 736f724f 7074696f ke a TensorOptio
   0x00033c60 6e732077 69746820 6f707469 6f6e732e ns with options.
   0x00033c70 72657175 69726573 5f677261 64207365 requires_grad se
   0x00033c80 74206173 20747275 652e2054 68697320 t as true. This 
   0x00033c90 69736e27 7420696d 706c656d 656e7465 isn't implemente
   0x00033ca0 64207965 742e0000 2f5f5f77 2f5f7465 d yet.../__w/_te
   0x00033cb0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033cc0 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00033cc0 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00033cd0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033ce0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033cf0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x00033d00 6f72652f 43686563 6b4d656d 6f727946 ore/CheckMemoryF
   0x00033d10 6f726d61 742e6800 63686563 6b5f7465 ormat.h.check_te
   0x00033d20 6e736f72 5f6f7074 696f6e73 5f616e64 nsor_options_and
   0x00033d30 5f657874 72616374 5f6d656d 6f72795f _extract_memory_
@@ -221,16 +221,16 @@
   0x00033da0 72656475 6e64616e 74207365 74746572 redundant setter
   0x00033db0 2e000000 00000000 496e7441 72726179 ........IntArray
   0x00033dc0 52656620 636f6e74 61696e73 20616e20 Ref contains an 
   0x00033dd0 696e7420 74686174 2063616e 6e6f7420 int that cannot 
   0x00033de0 62652072 65707265 73656e74 65642061 be represented a
   0x00033df0 73206120 53796d49 6e743a20 00000000 s a SymInt: ....
   0x00033e00 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00033e10 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x00033e20 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x00033e10 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x00033e20 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x00033e30 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00033e40 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00033e50 652f6331 302f636f 72652f53 796d496e e/c10/core/SymIn
   0x00033e60 74417272 61795265 662e6800 00000000 tArrayRef.h.....
   0x00033e70 63726561 74656420 41727261 79526566 created ArrayRef
   0x00033e80 20776974 68206e75 6c6c7074 7220616e  with nullptr an
   0x00033e90 64206e6f 6e2d7a65 726f206c 656e6774 d non-zero lengt
@@ -238,24 +238,24 @@
   0x00033eb0 2072656c 69657320 6f6e2074 68697320  relies on this 
   0x00033ec0 6265696e 6720696c 6c656761 6c000000 being illegal...
   0x00033ed0 44617461 20213d20 6e756c6c 70747220 Data != nullptr 
   0x00033ee0 7c7c204c 656e6774 68203d3d 20302049 || Length == 0 I
   0x00033ef0 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x00033f00 41494c45 44206174 20222f5f 5f772f5f AILED at "/__w/_
   0x00033f10 74656d70 2f636f6e 64615f65 6e766972 temp/conda_envir
-  0x00033f20 6f6e6d65 6e745f39 32303032 30323736 onment_920020276
-  0x00033f30 362f6c69 622f7079 74686f6e 332e392f 6/lib/python3.9/
+  0x00033f20 6f6e6d65 6e745f39 32313636 35333730 onment_921665370
+  0x00033f30 352f6c69 622f7079 74686f6e 332e392f 5/lib/python3.9/
   0x00033f40 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00033f50 7263682f 696e636c 7564652f 6331302f rch/include/c10/
   0x00033f60 7574696c 2f417272 61795265 662e6822 util/ArrayRef.h"
   0x00033f70 3a36322c 20706c65 61736520 7265706f :62, please repo
   0x00033f80 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x00033f90 7263682e 20000000 2f5f5f77 2f5f7465 rch. .../__w/_te
   0x00033fa0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033fb0 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00033fb0 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00033fc0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033fd0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033fe0 682f696e 636c7564 652f6331 302f7574 h/include/c10/ut
   0x00033ff0 696c2f41 72726179 5265662e 68006672 il/ArrayRef.h.fr
   0x00034000 6f6d496e 74417272 61795265 66536c6f omIntArrayRefSlo
   0x00034010 77006465 62756743 6865636b 4e756c6c w.debugCheckNull
   0x00034020 70747249 6e766172 69616e74 00000000 ptrInvariant....
@@ -270,15 +270,15 @@
   0x000340b0 745f2e6c 6f616428 29203e3d 20646574 t_.load() >= det
   0x000340c0 61696c3a 3a6b496d 70726163 74696361 ail::kImpractica
   0x000340d0 6c6c7948 75676552 65666572 656e6365 llyHugeReference
   0x000340e0 436f756e 7420494e 5445524e 414c2041 Count INTERNAL A
   0x000340f0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00034100 222f5f5f 772f5f74 656d702f 636f6e64 "/__w/_temp/cond
   0x00034110 615f656e 7669726f 6e6d656e 745f3932 a_environment_92
-  0x00034120 30303230 32373636 2f6c6962 2f707974 00202766/lib/pyt
+  0x00034120 31363635 33373035 2f6c6962 2f707974 16653705/lib/pyt
   0x00034130 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
   0x00034140 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00034150 64652f63 31302f75 74696c2f 696e7472 de/c10/util/intr
   0x00034160 75736976 655f7074 722e6822 3a313138 usive_ptr.h":118
   0x00034170 2c20706c 65617365 20726570 6f727420 , please report 
   0x00034180 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00034190 2e200000 00000000 54726965 6420746f . ......Tried to
@@ -298,38 +298,38 @@
   0x00034270 6e745f2e 6c6f6164 2829203d 3d206465 nt_.load() == de
   0x00034280 7461696c 3a3a6b49 6d707261 63746963 tail::kImpractic
   0x00034290 616c6c79 48756765 52656665 72656e63 allyHugeReferenc
   0x000342a0 65436f75 6e742049 4e544552 4e414c20 eCount INTERNAL 
   0x000342b0 41535345 52542046 41494c45 44206174 ASSERT FAILED at
   0x000342c0 20222f5f 5f772f5f 74656d70 2f636f6e  "/__w/_temp/con
   0x000342d0 64615f65 6e766972 6f6e6d65 6e745f39 da_environment_9
-  0x000342e0 32303032 30323736 362f6c69 622f7079 200202766/lib/py
+  0x000342e0 32313636 35333730 352f6c69 622f7079 216653705/lib/py
   0x000342f0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
   0x00034300 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00034310 7564652f 6331302f 7574696c 2f696e74 ude/c10/util/int
   0x00034320 72757369 76655f70 74722e68 223a3133 rusive_ptr.h":13
   0x00034330 332c2070 6c656173 65207265 706f7274 3, please report
   0x00034340 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x00034350 682e2000 7e696e74 72757369 76655f70 h. .~intrusive_p
   0x00034360 74725f74 61726765 74000000 00000000 tr_target.......
   0x00034370 73656c66 5f696d70 6c20494e 5445524e self_impl INTERN
   0x00034380 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00034390 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x000343a0 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x000343b0 745f3932 30303230 32373636 2f6c6962 t_9200202766/lib
+  0x000343b0 745f3932 31363635 33373035 2f6c6962 t_9216653705/lib
   0x000343c0 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x000343d0 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x000343e0 6e636c75 64652f74 6f726368 2f637372 nclude/torch/csr
   0x000343f0 632f6175 746f6772 61642f76 61726961 c/autograd/varia
   0x00034400 626c652e 68223a33 30352c20 706c6561 ble.h":305, plea
   0x00034410 73652072 65706f72 74206120 62756720 se report a bug 
   0x00034420 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x00034430 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00034440 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x00034450 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x00034440 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x00034450 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x00034460 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00034470 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00034480 652f746f 7263682f 63737263 2f617574 e/torch/csrc/aut
   0x00034490 6f677261 642f7661 72696162 6c652e68 ograd/variable.h
   0x000344a0 00000000 00000000 4f6e6c79 2054656e ........Only Ten
   0x000344b0 736f7273 206f6620 666c6f61 74696e67 sors of floating
   0x000344c0 20706f69 6e742061 6e642063 6f6d706c  point and compl
@@ -349,16 +349,16 @@
   0x000345a0 6d206074 68697360 3f000000 00000000 m `this`?.......
   0x000345b0 74617267 65745f2d 3e726566 636f756e target_->refcoun
   0x000345c0 745f203d 3d203020 26262074 61726765 t_ == 0 && targe
   0x000345d0 745f2d3e 7765616b 636f756e 745f203d t_->weakcount_ =
   0x000345e0 3d203020 494e5445 524e414c 20415353 = 0 INTERNAL ASS
   0x000345f0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00034600 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00034610 656e7669 726f6e6d 656e745f 39323030 environment_9200
-  0x00034620 32303237 36362f6c 69622f70 7974686f 202766/lib/pytho
+  0x00034610 656e7669 726f6e6d 656e745f 39323136 environment_9216
+  0x00034620 36353337 30352f6c 69622f70 7974686f 653705/lib/pytho
   0x00034630 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00034640 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00034650 2f633130 2f757469 6c2f696e 74727573 /c10/util/intrus
   0x00034660 6976655f 7074722e 68223a33 31392c20 ive_ptr.h":319, 
   0x00034670 706c6561 73652072 65706f72 74206120 please report a 
   0x00034680 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00034690 00696e74 72757369 76655f70 74720000 .intrusive_ptr..
@@ -369,30 +369,30 @@
   0x000346e0 616e6e6f 7420696e 63726561 73652072 annot increase r
   0x000346f0 6566636f 756e7420 61667465 72206974 efcount after it
   0x00034700 20726561 63686564 207a6572 6f2e0000  reached zero...
   0x00034710 6e65775f 72656663 6f756e74 20213d20 new_refcount != 
   0x00034720 3120494e 5445524e 414c2041 53534552 1 INTERNAL ASSER
   0x00034730 54204641 494c4544 20617420 222f5f5f T FAILED at "/__
   0x00034740 772f5f74 656d702f 636f6e64 615f656e w/_temp/conda_en
-  0x00034750 7669726f 6e6d656e 745f3932 30303230 vironment_920020
-  0x00034760 32373636 2f6c6962 2f707974 686f6e33 2766/lib/python3
+  0x00034750 7669726f 6e6d656e 745f3932 31363635 vironment_921665
+  0x00034760 33373035 2f6c6962 2f707974 686f6e33 3705/lib/python3
   0x00034770 2e392f73 6974652d 7061636b 61676573 .9/site-packages
   0x00034780 2f746f72 63682f69 6e636c75 64652f63 /torch/include/c
   0x00034790 31302f75 74696c2f 696e7472 75736976 10/util/intrusiv
   0x000347a0 655f7074 722e6822 3a323734 2c20706c e_ptr.h":274, pl
   0x000347b0 65617365 20726570 6f727420 61206275 ease report a bu
   0x000347c0 6720746f 20507954 6f726368 2e200072 g to PyTorch. .r
   0x000347d0 65746169 6e5f0076 6563746f 723a3a5f etain_.vector::_
   0x000347e0 4d5f7265 616c6c6f 635f696e 73657274 M_realloc_insert
   0x000347f0 00657870 65637465 6420696e 7400746f .expected int.to
   0x00034800 496e7400 00000000 3020494e 5445524e Int.....0 INTERN
   0x00034810 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00034820 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x00034830 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x00034840 745f3932 30303230 32373636 2f6c6962 t_9200202766/lib
+  0x00034840 745f3932 31363635 33373035 2f6c6962 t_9216653705/lib
   0x00034850 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x00034860 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00034870 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x00034880 2f697661 6c75652e 68223a36 35322c20 /ivalue.h":652, 
   0x00034890 706c6561 73652072 65706f72 74206120 please report a 
   0x000348a0 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x000348b0 00000000 00000000 00000000 00000000 ................
@@ -437,15 +437,15 @@
   0x00034b20 45000000 00000000 65787472 615f6d65 E.......extra_me
   0x00034b30 74615f20 26262065 78747261 5f6d6574 ta_ && extra_met
   0x00034b40 615f2d3e 73796d62 6f6c6963 5f736861 a_->symbolic_sha
   0x00034b50 70655f6d 6574615f 20494e54 45524e41 pe_meta_ INTERNA
   0x00034b60 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x00034b70 61742022 2f5f5f77 2f5f7465 6d702f63 at "/__w/_temp/c
   0x00034b80 6f6e6461 5f656e76 69726f6e 6d656e74 onda_environment
-  0x00034b90 5f393230 30323032 3736362f 6c69622f _9200202766/lib/
+  0x00034b90 5f393231 36363533 3730352f 6c69622f _9216653705/lib/
   0x00034ba0 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
   0x00034bb0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x00034bc0 636c7564 652f6331 302f636f 72652f54 clude/c10/core/T
   0x00034bd0 656e736f 72496d70 6c2e6822 3a313732 ensorImpl.h":172
   0x00034be0 332c2070 6c656173 65207265 706f7274 3, please report
   0x00034bf0 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x00034c00 682e2000 00000000 45787065 63746564 h. .....Expected
@@ -556,25 +556,25 @@
   0x00035290 1069feff 0069feff 706afeff 606afeff .i...i..pj..`j..
   0x000352a0 506afeff 406afeff 7069feff 6069feff Pj..@j..pi..`i..
   0x000352b0 5069feff 4069feff d068feff c068feff Pi..@i...h...h..
   0x000352c0 e068feff 00000000 642e6973 5f637564 .h......d.is_cud
   0x000352d0 61282920 494e5445 524e414c 20415353 a() INTERNAL ASS
   0x000352e0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x000352f0 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00035300 656e7669 726f6e6d 656e745f 39323030 environment_9200
-  0x00035310 32303237 36362f6c 69622f70 7974686f 202766/lib/pytho
+  0x00035300 656e7669 726f6e6d 656e745f 39323136 environment_9216
+  0x00035310 36353337 30352f6c 69622f70 7974686f 653705/lib/pytho
   0x00035320 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00035330 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00035340 2f633130 2f637564 612f696d 706c2f43 /c10/cuda/impl/C
   0x00035350 55444147 75617264 496d706c 2e68223a UDAGuardImpl.h":
   0x00035360 35332c20 706c6561 73652072 65706f72 53, please repor
   0x00035370 74206120 62756720 746f2050 79546f72 t a bug to PyTor
   0x00035380 63682e20 00000000 2f5f5f77 2f5f7465 ch. ..../__w/_te
   0x00035390 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x000353a0 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x000353a0 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x000353b0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x000353c0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x000353d0 682f696e 636c7564 652f6331 302f6375 h/include/c10/cu
   0x000353e0 64612f69 6d706c2f 43554441 47756172 da/impl/CUDAGuar
   0x000353f0 64496d70 6c2e6800 73657444 65766963 dImpl.h.setDevic
   0x00035400 65000000 00000000 426f7468 20657665 e.......Both eve
   0x00035410 6e747320 6d757374 20626520 7265636f nts must be reco
@@ -590,75 +590,75 @@
   0x000354b0 69732065 72726f72 206d6573 73616765 is error message
   0x000354c0 20626520 696d7072 6f766564 3f202049  be improved?  I
   0x000354d0 6620736f 2c20706c 65617365 20726570 f so, please rep
   0x000354e0 6f727420 616e2065 6e68616e 63656d65 ort an enhanceme
   0x000354f0 6e742072 65717565 73742074 6f205079 nt request to Py
   0x00035500 546f7263 682e2900 2f5f5f77 2f5f7465 Torch.)./__w/_te
   0x00035510 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035520 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00035520 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00035530 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035540 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035550 682f696e 636c7564 652f6331 302f6375 h/include/c10/cu
   0x00035560 64612f43 55444153 74726561 6d2e6800 da/CUDAStream.h.
   0x00035570 43554441 53747265 616d0073 796e6368 CUDAStream.synch
   0x00035580 726f6e69 7a654576 656e7400 71756572 ronizeEvent.quer
   0x00035590 79457665 6e74006c 61796f75 74000000 yEvent.layout...
   0x000355a0 54686572 65206973 20616e20 6572726f There is an erro
   0x000355b0 7220696e 20746865 206c6179 6f757420 r in the layout 
   0x000355c0 63616c63 756c6174 696f6e20 6c6f6769 calculation logi
   0x000355d0 632e0000 00000000 69735f6d 6b6c646e c.......is_mkldn
   0x000355e0 6e282920 494e5445 524e414c 20415353 n() INTERNAL ASS
   0x000355f0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00035600 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00035610 656e7669 726f6e6d 656e745f 39323030 environment_9200
-  0x00035620 32303237 36362f6c 69622f70 7974686f 202766/lib/pytho
+  0x00035610 656e7669 726f6e6d 656e745f 39323136 environment_9216
+  0x00035620 36353337 30352f6c 69622f70 7974686f 653705/lib/pytho
   0x00035630 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00035640 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00035650 2f633130 2f636f72 652f5465 6e736f72 /c10/core/Tensor
   0x00035660 496d706c 2e68223a 31323930 2c20706c Impl.h":1290, pl
   0x00035670 65617365 20726570 6f727420 61206275 ease report a bu
   0x00035680 6720746f 20507954 6f726368 2e200000 g to PyTorch. ..
   0x00035690 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000356a0 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000356b0 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x000356c0 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x000356b0 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x000356c0 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x000356d0 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x000356e0 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x000356f0 00000000 00000000 5f5a4e37 746f7263 ........_ZN7torc
   0x00035700 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
   0x00035710 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
-  0x00035720 63755f31 62316437 6430655f 32323030 cu_1b1d7d0e_2200
+  0x00035720 63755f31 35623935 6539315f 32353836 cu_15b95e91_2586
   0x00035730 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
   0x00035740 6c496645 45766964 504b545f 50790000 lIfEEvidPKT_Py..
   0x00035750 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x00035760 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x00035770 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x00035780 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x00035770 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x00035780 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x00035790 726e656c 5f696d70 6c496445 45766964 rnel_implIdEEvid
   0x000357a0 504b545f 50790000 5f5a4e34 315f494e PKT_Py.._ZN41_IN
   0x000357b0 5445524e 414c5f35 62326539 3235395f TERNAL_5b2e9259_
-  0x000357c0 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x000357d0 655f3232 30303674 68727573 74367379 e_22006thrust6sy
+  0x000357c0 365f6e6d 735f6375 5f313562 39356539 6_nms_cu_15b95e9
+  0x000357d0 315f3235 38363674 68727573 74367379 1_25866thrust6sy
   0x000357e0 7374656d 36646574 61696c31 30736571 stem6detail10seq
   0x000357f0 75656e74 69616c33 73657145 00000000 uential3seqE....
   0x00035800 69735f68 6561705f 616c6c6f 63617465 is_heap_allocate
   0x00035810 64282920 494e5445 524e414c 20415353 d() INTERNAL ASS
   0x00035820 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00035830 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00035840 656e7669 726f6e6d 656e745f 39323030 environment_9200
-  0x00035850 32303237 36362f6c 69622f70 7974686f 202766/lib/pytho
+  0x00035840 656e7669 726f6e6d 656e745f 39323136 environment_9216
+  0x00035850 36353337 30352f6c 69622f70 7974686f 653705/lib/pytho
   0x00035860 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00035870 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00035880 2f633130 2f636f72 652f5379 6d496e74 /c10/core/SymInt
   0x00035890 2e68223a 38392c20 706c6561 73652072 .h":89, please r
   0x000358a0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x000358b0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x000358c0 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x000358d0 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x000358e0 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x000358d0 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x000358e0 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x000358f0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00035900 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00035910 652f6331 302f636f 72652f53 796d496e e/c10/core/SymIn
   0x00035920 742e6800 00000000 2f5f5f77 2f616f2f t.h...../__w/ao/
   0x00035930 616f2f70 79746f72 63682f61 6f2f746f ao/pytorch/ao/to
   0x00035940 72636861 6f2f6373 72632f63 7564612f rchao/csrc/cuda/
   0x00035950 6e6d732e 63750000 626f7865 73207368 nms.cu..boxes sh
@@ -675,59 +675,59 @@
   0x00035a00 65206e75 6d626572 206f6620 656c656d e number of elem
   0x00035a10 656e7473 20696e20 00000000 00000000 ents in ........
   0x00035a20 74203d3d 20446576 69636554 7970653a t == DeviceType:
   0x00035a30 3a435544 4120494e 5445524e 414c2041 :CUDA INTERNAL A
   0x00035a40 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00035a50 222f5f5f 772f5f74 656d702f 636f6e64 "/__w/_temp/cond
   0x00035a60 615f656e 7669726f 6e6d656e 745f3932 a_environment_92
-  0x00035a70 30303230 32373636 2f6c6962 2f707974 00202766/lib/pyt
+  0x00035a70 31363635 33373035 2f6c6962 2f707974 16653705/lib/pyt
   0x00035a80 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
   0x00035a90 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00035aa0 64652f63 31302f63 7564612f 696d706c de/c10/cuda/impl
   0x00035ab0 2f435544 41477561 7264496d 706c2e68 /CUDAGuardImpl.h
   0x00035ac0 223a3238 2c20706c 65617365 20726570 ":28, please rep
   0x00035ad0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x00035ae0 6f726368 2e200000 63616e6e 6f742063 orch. ..cannot c
   0x00035af0 72656174 65207374 643a3a76 6563746f reate std::vecto
   0x00035b00 72206c61 72676572 20746861 6e206d61 r larger than ma
   0x00035b10 785f7369 7a652829 00000000 00000000 x_size()........
   0x00035b20 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00035b30 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x00035b40 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x00035b30 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x00035b40 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x00035b50 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00035b60 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00035b70 652f4154 656e2f54 656e736f 72496e64 e/ATen/TensorInd
   0x00035b80 6578696e 672e6800 67657444 65766963 exing.h.getDevic
   0x00035b90 65007661 6c696461 74650000 00000000 e.validate......
   0x00035ba0 44657669 63652069 6e646578 206d7573 Device index mus
   0x00035bb0 74206265 202d3120 6f72206e 6f6e2d6e t be -1 or non-n
   0x00035bc0 65676174 6976652c 20676f74 20000000 egative, got ...
   0x00035bd0 696e6465 785f203e 3d202d31 20494e54 index_ >= -1 INT
   0x00035be0 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x00035bf0 4c454420 61742022 2f5f5f77 2f5f7465 LED at "/__w/_te
   0x00035c00 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035c10 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00035c10 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00035c20 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035c30 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035c40 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00035c50 72652f44 65766963 652e6822 3a313737 re/Device.h":177
   0x00035c60 2c20706c 65617365 20726570 6f727420 , please report 
   0x00035c70 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00035c80 2e200000 00000000 2f5f5f77 2f5f7465 . ....../__w/_te
   0x00035c90 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035ca0 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00035ca0 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00035cb0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035cc0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035cd0 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00035ce0 72652f44 65766963 652e6800 00000000 re/Device.h.....
   0x00035cf0 642e6973 5f637564 61282920 494e5445 d.is_cuda() INTE
   0x00035d00 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00035d10 45442061 7420222f 5f5f772f 5f74656d ED at "/__w/_tem
   0x00035d20 702f636f 6e64615f 656e7669 726f6e6d p/conda_environm
-  0x00035d30 656e745f 39323030 32303237 36362f6c ent_9200202766/l
+  0x00035d30 656e745f 39323136 36353337 30352f6c ent_9216653705/l
   0x00035d40 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
   0x00035d50 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00035d60 2f696e63 6c756465 2f633130 2f637564 /include/c10/cud
   0x00035d70 612f696d 706c2f43 55444147 75617264 a/impl/CUDAGuard
   0x00035d80 496d706c 2e68223a 33342c20 706c6561 Impl.h":34, plea
   0x00035d90 73652072 65706f72 74206120 62756720 se report a bug 
   0x00035da0 746f2050 79546f72 63682e20 00657863 to PyTorch. .exc
@@ -746,24 +746,24 @@
   0x00035e70 6f794576 656e7400 20646576 69636573 oyEvent. devices
   0x00035e80 00676574 44657669 63654775 61726449 .getDeviceGuardI
   0x00035e90 6d706c00 71756572 79000000 00000000 mpl.query.......
   0x00035ea0 5079546f 72636820 6973206e 6f74206c PyTorch is not l
   0x00035eb0 696e6b65 64207769 74682073 7570706f inked with suppo
   0x00035ec0 72742066 6f722000 2f5f5f77 2f5f7465 rt for ./__w/_te
   0x00035ed0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035ee0 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00035ee0 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00035ef0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035f00 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035f10 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00035f20 72652f69 6d706c2f 44657669 63654775 re/impl/DeviceGu
   0x00035f30 61726449 6d706c49 6e746572 66616365 ardImplInterface
   0x00035f40 2e680073 74726561 6d5f7379 6e636872 .h.stream_synchr
   0x00035f50 6f6e697a 65000000 2f5f5f77 2f5f7465 onize.../__w/_te
   0x00035f60 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035f70 6d656e74 5f393230 30323032 3736362f ment_9200202766/
+  0x00035f70 6d656e74 5f393231 36363533 3730352f ment_9216653705/
   0x00035f80 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035f90 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035fa0 682f696e 636c7564 652f6331 302f6375 h/include/c10/cu
   0x00035fb0 64612f43 55444146 756e6374 696f6e73 da/CUDAFunctions
   0x00035fc0 2e680000 00000000 45787065 63746564 .h......Expected
   0x00035fd0 20707472 5f2d3e69 735f666c 6f617428  ptr_->is_float(
   0x00035fe0 2920746f 20626520 74727565 2c206275 ) to be true, bu
@@ -771,24 +771,24 @@
   0x00036000 6f756c64 20746869 73206572 726f7220 ould this error 
   0x00036010 6d657373 61676520 62652069 6d70726f message be impro
   0x00036020 7665643f 20204966 20736f2c 20706c65 ved?  If so, ple
   0x00036030 61736520 7265706f 72742061 6e20656e ase report an en
   0x00036040 68616e63 656d656e 74207265 71756573 hancement reques
   0x00036050 7420746f 20507954 6f726368 2e290000 t to PyTorch.)..
   0x00036060 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00036070 5f656e76 69726f6e 6d656e74 5f393230 _environment_920
-  0x00036080 30323032 3736362f 6c69622f 70797468 0202766/lib/pyth
+  0x00036070 5f656e76 69726f6e 6d656e74 5f393231 _environment_921
+  0x00036080 36363533 3730352f 6c69622f 70797468 6653705/lib/pyth
   0x00036090 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x000360a0 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x000360b0 652f6331 302f636f 72652f53 796d466c e/c10/core/SymFl
   0x000360c0 6f61742e 68000000 3020494e 5445524e oat.h...0 INTERN
   0x000360d0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x000360e0 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x000360f0 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x00036100 745f3932 30303230 32373636 2f6c6962 t_9200202766/lib
+  0x00036100 745f3932 31363635 33373035 2f6c6962 t_9216653705/lib
   0x00036110 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x00036120 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00036130 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x00036140 2f697661 6c75652e 68223a35 34302c20 /ivalue.h":540, 
   0x00036150 706c6561 73652072 65706f72 74206120 please report a 
   0x00036160 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00036170 00657870 65637465 6420646f 75626c65 .expected double
```

### readelf --wide --decompress --hex-dump=.nv_fatbin {}

```diff
@@ -26202,236 +26202,236 @@
   0x0009def8 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
   0x0009df08 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
   0x0009df18 61625f73 686e6478 002e6e76 2e756674 ab_shndx..nv.uft
   0x0009df28 2e656e74 7279002e 6e762e69 6e666f00 .entry..nv.info.
   0x0009df38 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x0009df48 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x0009df58 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x0009df68 5f316231 64376430 655f3232 30303135 _1b1d7d0e_220015
+  0x0009df68 5f313562 39356539 315f3235 38363135 _15b95e91_258615
   0x0009df78 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x0009df88 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x0009df98 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x0009dfa8 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009dfb8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009dfc8 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x0009dfd8 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x0009dfc8 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x0009dfd8 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x0009dfe8 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x0009dff8 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x0009e008 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x0009e018 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x0009e028 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x0009e038 6e6d735f 63755f31 62316437 6430655f nms_cu_1b1d7d0e_
-  0x0009e048 32323030 31356e6d 735f6b65 726e656c 220015nms_kernel
+  0x0009e038 6e6d735f 63755f31 35623935 6539315f nms_cu_15b95e91_
+  0x0009e048 32353836 31356e6d 735f6b65 726e656c 258615nms_kernel
   0x0009e058 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x0009e068 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x0009e078 2e676c6f 62616c00 2e6e762e 636f6e73 .global..nv.cons
   0x0009e088 74616e74 302e5f5a 4e37746f 72636861 tant0._ZN7torcha
   0x0009e098 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x0009e0a8 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x0009e0b8 5f316231 64376430 655f3232 30303135 _1b1d7d0e_220015
+  0x0009e0b8 5f313562 39356539 315f3235 38363135 _15b95e91_258615
   0x0009e0c8 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x0009e0d8 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x0009e0e8 504b545f 5079002e 74657874 2e5f5a4e PKT_Py..text._ZN
   0x0009e0f8 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x0009e108 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x0009e118 5f6e6d73 5f63755f 31623164 37643065 _nms_cu_1b1d7d0e
-  0x0009e128 5f323230 3031356e 6d735f6b 65726e65 _220015nms_kerne
+  0x0009e118 5f6e6d73 5f63755f 31356239 35653931 _nms_cu_15b95e91
+  0x0009e128 5f323538 3631356e 6d735f6b 65726e65 _258615nms_kerne
   0x0009e138 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x0009e148 5f507900 2e6e762e 696e666f 2e5f5a4e _Py..nv.info._ZN
   0x0009e158 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x0009e168 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x0009e178 5f6e6d73 5f63755f 31623164 37643065 _nms_cu_1b1d7d0e
-  0x0009e188 5f323230 3031356e 6d735f6b 65726e65 _220015nms_kerne
+  0x0009e178 5f6e6d73 5f63755f 31356239 35653931 _nms_cu_15b95e91
+  0x0009e188 5f323538 3631356e 6d735f6b 65726e65 _258615nms_kerne
   0x0009e198 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x0009e1a8 5f507900 2e6e762e 73686172 65642e5f _Py..nv.shared._
   0x0009e1b8 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x0009e1c8 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x0009e1d8 5f365f6e 6d735f63 755f3162 31643764 _6_nms_cu_1b1d7d
-  0x0009e1e8 30655f32 32303031 356e6d73 5f6b6572 0e_220015nms_ker
+  0x0009e1d8 5f365f6e 6d735f63 755f3135 62393565 _6_nms_cu_15b95e
+  0x0009e1e8 39315f32 35383631 356e6d73 5f6b6572 91_258615nms_ker
   0x0009e1f8 6e656c5f 696d706c 49664545 76696450 nel_implIfEEvidP
   0x0009e208 4b545f50 79002e6e 762e636f 6e737461 KT_Py..nv.consta
   0x0009e218 6e74302e 5f5a4e37 746f7263 68616f34 nt0._ZN7torchao4
   0x0009e228 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
   0x0009e238 65393235 395f365f 6e6d735f 63755f31 e9259_6_nms_cu_1
-  0x0009e248 62316437 6430655f 32323030 31356e6d b1d7d0e_220015nm
+  0x0009e248 35623935 6539315f 32353836 31356e6d 5b95e91_258615nm
   0x0009e258 735f6b65 726e656c 5f696d70 6c496645 s_kernel_implIfE
   0x0009e268 45766964 504b545f 5079002e 74657874 EvidPKT_Py..text
   0x0009e278 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x0009e288 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x0009e298 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x0009e2a8 37643065 5f323230 3031356e 6d735f6b 7d0e_220015nms_k
+  0x0009e298 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x0009e2a8 35653931 5f323538 3631356e 6d735f6b 5e91_258615nms_k
   0x0009e2b8 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x0009e2c8 64504b54 5f507900 2e6e762e 696e666f dPKT_Py..nv.info
   0x0009e2d8 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x0009e2e8 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x0009e2f8 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x0009e308 37643065 5f323230 3031356e 6d735f6b 7d0e_220015nms_k
+  0x0009e2f8 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x0009e308 35653931 5f323538 3631356e 6d735f6b 5e91_258615nms_k
   0x0009e318 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x0009e328 64504b54 5f507900 2e6e762e 73686172 dPKT_Py..nv.shar
   0x0009e338 65642e5f 5a4e3774 6f726368 616f3433 ed._ZN7torchao43
   0x0009e348 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009e358 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x0009e368 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x0009e358 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x0009e368 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x0009e378 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x0009e388 76696450 4b545f50 79002e6e 762e636f vidPKT_Py..nv.co
   0x0009e398 6e737461 6e74302e 5f5a4e37 746f7263 nstant0._ZN7torc
   0x0009e3a8 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
   0x0009e3b8 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
-  0x0009e3c8 63755f31 62316437 6430655f 32323030 cu_1b1d7d0e_2200
+  0x0009e3c8 63755f31 35623935 6539315f 32353836 cu_15b95e91_2586
   0x0009e3d8 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
   0x0009e3e8 6c496445 45766964 504b545f 5079002e lIdEEvidPKT_Py..
   0x0009e3f8 64656275 675f6672 616d6500 2e72656c debug_frame..rel
   0x0009e408 2e646562 75675f66 72616d65 002e7265 .debug_frame..re
   0x0009e418 6c612e64 65627567 5f667261 6d650000 la.debug_frame..
   0x0009e428 2e736873 74727461 62002e73 74727461 .shstrtab..strta
   0x0009e438 62002e73 796d7461 62002e73 796d7461 b..symtab..symta
   0x0009e448 625f7368 6e647800 2e6e762e 7566742e b_shndx..nv.uft.
   0x0009e458 656e7472 79002e6e 762e696e 666f005f entry..nv.info._
   0x0009e468 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x0009e478 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x0009e488 5f365f6e 6d735f63 755f3162 31643764 _6_nms_cu_1b1d7d
-  0x0009e498 30655f32 32303031 356e6d73 5f6b6572 0e_220015nms_ker
+  0x0009e488 5f365f6e 6d735f63 755f3135 62393565 _6_nms_cu_15b95e
+  0x0009e498 39315f32 35383631 356e6d73 5f6b6572 91_258615nms_ker
   0x0009e4a8 6e656c5f 696d706c 494e3363 31303448 nel_implIN3c104H
   0x0009e4b8 616c6645 45457669 64504b54 5f507900 alfEEEvidPKT_Py.
   0x0009e4c8 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x0009e4d8 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x0009e4e8 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x0009e4f8 5f316231 64376430 655f3232 30303135 _1b1d7d0e_220015
+  0x0009e4f8 5f313562 39356539 315f3235 38363135 _15b95e91_258615
   0x0009e508 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x0009e518 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x0009e528 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x0009e538 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009e548 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009e558 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x0009e568 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x0009e558 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x0009e568 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x0009e578 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x0009e588 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x0009e598 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x0009e5a8 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x0009e5b8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x0009e5c8 6e6d735f 63755f31 62316437 6430655f nms_cu_1b1d7d0e_
-  0x0009e5d8 32323030 31356e6d 735f6b65 726e656c 220015nms_kernel
+  0x0009e5c8 6e6d735f 63755f31 35623935 6539315f nms_cu_15b95e91_
+  0x0009e5d8 32353836 31356e6d 735f6b65 726e656c 258615nms_kernel
   0x0009e5e8 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x0009e5f8 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x0009e608 2e676c6f 62616c00 5f5a4e34 315f494e .global._ZN41_IN
   0x0009e618 5445524e 414c5f35 62326539 3235395f TERNAL_5b2e9259_
-  0x0009e628 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x0009e638 655f3232 30303674 68727573 74367379 e_22006thrust6sy
+  0x0009e628 365f6e6d 735f6375 5f313562 39356539 6_nms_cu_15b95e9
+  0x0009e638 315f3235 38363674 68727573 74367379 1_25866thrust6sy
   0x0009e648 7374656d 36646574 61696c31 30736571 stem6detail10seq
   0x0009e658 75656e74 69616c33 73657145 00245f5a uential3seqE.$_Z
   0x0009e668 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
   0x0009e678 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x0009e688 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x0009e698 655f3232 30303135 6e6d735f 6b65726e e_220015nms_kern
+  0x0009e688 365f6e6d 735f6375 5f313562 39356539 6_nms_cu_15b95e9
+  0x0009e698 315f3235 38363135 6e6d735f 6b65726e 1_258615nms_kern
   0x0009e6a8 656c5f69 6d706c49 4e336331 30344861 el_implIN3c104Ha
   0x0009e6b8 6c664545 45766964 504b545f 5079245f lfEEEvidPKT_Py$_
   0x0009e6c8 5f637564 615f736d 33785f64 69765f72 _cuda_sm3x_div_r
   0x0009e6d8 6e5f6e6f 66747a5f 6633325f 736c6f77 n_noftz_f32_slow
   0x0009e6e8 70617468 00245f5f 5f5a5a4e 37746f72 path.$___ZZN7tor
   0x0009e6f8 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x0009e708 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x0009e718 5f63755f 31623164 37643065 5f323230 _cu_1b1d7d0e_220
-  0x0009e728 3031356e 6d735f6b 65726e65 6c5f696d 015nms_kernel_im
+  0x0009e718 5f63755f 31356239 35653931 5f323538 _cu_15b95e91_258
+  0x0009e728 3631356e 6d735f6b 65726e65 6c5f696d 615nms_kernel_im
   0x0009e738 706c494e 33633130 3448616c 66454545 plIN3c104HalfEEE
   0x0009e748 76696450 4b545f50 79453131 626c6f63 vidPKT_PyE11bloc
   0x0009e758 6b5f626f 7865735f 5f353337 002e6e76 k_boxes__537..nv
   0x0009e768 2e636f6e 7374616e 74302e5f 5a4e3774 .constant0._ZN7t
   0x0009e778 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x0009e788 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x0009e798 6d735f63 755f3162 31643764 30655f32 ms_cu_1b1d7d0e_2
-  0x0009e7a8 32303031 356e6d73 5f6b6572 6e656c5f 20015nms_kernel_
+  0x0009e798 6d735f63 755f3135 62393565 39315f32 ms_cu_15b95e91_2
+  0x0009e7a8 35383631 356e6d73 5f6b6572 6e656c5f 58615nms_kernel_
   0x0009e7b8 696d706c 494e3363 31303448 616c6645 implIN3c104HalfE
   0x0009e7c8 45457669 64504b54 5f507900 5f706172 EEvidPKT_Py._par
   0x0009e7d8 616d005f 5a4e3774 6f726368 616f3433 am._ZN7torchao43
   0x0009e7e8 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009e7f8 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x0009e808 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x0009e7f8 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x0009e808 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x0009e818 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x0009e828 76696450 4b545f50 79002e74 6578742e vidPKT_Py..text.
   0x0009e838 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009e848 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009e858 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x0009e868 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x0009e858 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x0009e868 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x0009e878 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x0009e888 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x0009e898 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009e8a8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009e8b8 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x0009e8c8 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x0009e8b8 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x0009e8c8 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x0009e8d8 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x0009e8e8 504b545f 5079002e 6e762e73 68617265 PKT_Py..nv.share
   0x0009e8f8 642e5f5a 4e37746f 72636861 6f34335f d._ZN7torchao43_
   0x0009e908 474c4f42 414c5f5f 4e5f5f35 62326539 GLOBAL__N__5b2e9
-  0x0009e918 3235395f 365f6e6d 735f6375 5f316231 259_6_nms_cu_1b1
-  0x0009e928 64376430 655f3232 30303135 6e6d735f d7d0e_220015nms_
+  0x0009e918 3235395f 365f6e6d 735f6375 5f313562 259_6_nms_cu_15b
+  0x0009e928 39356539 315f3235 38363135 6e6d735f 95e91_258615nms_
   0x0009e938 6b65726e 656c5f69 6d706c49 66454576 kernel_implIfEEv
   0x0009e948 6964504b 545f5079 00245f5a 4e37746f idPKT_Py.$_ZN7to
   0x0009e958 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x0009e968 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x0009e978 735f6375 5f316231 64376430 655f3232 s_cu_1b1d7d0e_22
-  0x0009e988 30303135 6e6d735f 6b65726e 656c5f69 0015nms_kernel_i
+  0x0009e978 735f6375 5f313562 39356539 315f3235 s_cu_15b95e91_25
+  0x0009e988 38363135 6e6d735f 6b65726e 656c5f69 8615nms_kernel_i
   0x0009e998 6d706c49 66454576 6964504b 545f5079 mplIfEEvidPKT_Py
   0x0009e9a8 245f5f63 7564615f 736d3378 5f646976 $__cuda_sm3x_div
   0x0009e9b8 5f726e5f 6e6f6674 7a5f6633 325f736c _rn_noftz_f32_sl
   0x0009e9c8 6f777061 74680024 5f5f5f5a 5a4e3774 owpath.$___ZZN7t
   0x0009e9d8 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x0009e9e8 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x0009e9f8 6d735f63 755f3162 31643764 30655f32 ms_cu_1b1d7d0e_2
-  0x0009ea08 32303031 356e6d73 5f6b6572 6e656c5f 20015nms_kernel_
+  0x0009e9f8 6d735f63 755f3135 62393565 39315f32 ms_cu_15b95e91_2
+  0x0009ea08 35383631 356e6d73 5f6b6572 6e656c5f 58615nms_kernel_
   0x0009ea18 696d706c 49664545 76696450 4b545f50 implIfEEvidPKT_P
   0x0009ea28 79453131 626c6f63 6b5f626f 7865735f yE11block_boxes_
   0x0009ea38 5f323834 002e6e76 2e636f6e 7374616e _284..nv.constan
   0x0009ea48 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x0009ea58 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009ea68 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x0009ea78 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x0009ea68 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x0009ea78 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x0009ea88 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x0009ea98 76696450 4b545f50 79005f5a 4e37746f vidPKT_Py._ZN7to
   0x0009eaa8 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x0009eab8 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x0009eac8 735f6375 5f316231 64376430 655f3232 s_cu_1b1d7d0e_22
-  0x0009ead8 30303135 6e6d735f 6b65726e 656c5f69 0015nms_kernel_i
+  0x0009eac8 735f6375 5f313562 39356539 315f3235 s_cu_15b95e91_25
+  0x0009ead8 38363135 6e6d735f 6b65726e 656c5f69 8615nms_kernel_i
   0x0009eae8 6d706c49 64454576 6964504b 545f5079 mplIdEEvidPKT_Py
   0x0009eaf8 002e7465 78742e5f 5a4e3774 6f726368 ..text._ZN7torch
   0x0009eb08 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x0009eb18 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x0009eb28 755f3162 31643764 30655f32 32303031 u_1b1d7d0e_22001
+  0x0009eb28 755f3135 62393565 39315f32 35383631 u_15b95e91_25861
   0x0009eb38 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x0009eb48 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x0009eb58 762e696e 666f2e5f 5a4e3774 6f726368 v.info._ZN7torch
   0x0009eb68 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x0009eb78 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x0009eb88 755f3162 31643764 30655f32 32303031 u_1b1d7d0e_22001
+  0x0009eb88 755f3135 62393565 39315f32 35383631 u_15b95e91_25861
   0x0009eb98 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x0009eba8 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x0009ebb8 762e7368 61726564 2e5f5a4e 37746f72 v.shared._ZN7tor
   0x0009ebc8 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x0009ebd8 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x0009ebe8 5f63755f 31623164 37643065 5f323230 _cu_1b1d7d0e_220
-  0x0009ebf8 3031356e 6d735f6b 65726e65 6c5f696d 015nms_kernel_im
+  0x0009ebe8 5f63755f 31356239 35653931 5f323538 _cu_15b95e91_258
+  0x0009ebf8 3631356e 6d735f6b 65726e65 6c5f696d 615nms_kernel_im
   0x0009ec08 706c4964 45457669 64504b54 5f507900 plIdEEvidPKT_Py.
   0x0009ec18 245f5a4e 37746f72 6368616f 34335f47 $_ZN7torchao43_G
   0x0009ec28 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x0009ec38 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x0009ec48 37643065 5f323230 3031356e 6d735f6b 7d0e_220015nms_k
+  0x0009ec38 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x0009ec48 35653931 5f323538 3631356e 6d735f6b 5e91_258615nms_k
   0x0009ec58 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x0009ec68 64504b54 5f507924 5f5f6375 64615f73 dPKT_Py$__cuda_s
   0x0009ec78 6d32305f 6469765f 6636345f 736c6f77 m20_div_f64_slow
   0x0009ec88 70617468 5f763200 245f5f5f 5a5a4e37 path_v2.$___ZZN7
   0x0009ec98 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x0009eca8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x0009ecb8 6e6d735f 63755f31 62316437 6430655f nms_cu_1b1d7d0e_
-  0x0009ecc8 32323030 31356e6d 735f6b65 726e656c 220015nms_kernel
+  0x0009ecb8 6e6d735f 63755f31 35623935 6539315f nms_cu_15b95e91_
+  0x0009ecc8 32353836 31356e6d 735f6b65 726e656c 258615nms_kernel
   0x0009ecd8 5f696d70 6c496445 45766964 504b545f _implIdEEvidPKT_
   0x0009ece8 50794531 31626c6f 636b5f62 6f786573 PyE11block_boxes
   0x0009ecf8 5f5f3331 002e6e76 2e636f6e 7374616e __31..nv.constan
   0x0009ed08 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x0009ed18 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009ed28 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x0009ed38 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x0009ed28 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x0009ed38 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x0009ed48 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x0009ed58 76696450 4b545f50 79002e64 65627567 vidPKT_Py..debug
   0x0009ed68 5f667261 6d65002e 72656c2e 64656275 _frame..rel.debu
   0x0009ed78 675f6672 616d6500 2e72656c 612e6465 g_frame..rela.de
   0x0009ed88 6275675f 6672616d 65000000 00000000 bug_frame.......
   0x0009ed98 00000000 00000000 00000000 00000000 ................
   0x0009eda8 00000000 00000000 40000000 02100d00 ........@.......
@@ -28252,236 +28252,236 @@
   0x000a5f18 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
   0x000a5f28 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
   0x000a5f38 61625f73 686e6478 002e6e76 2e756674 ab_shndx..nv.uft
   0x000a5f48 2e656e74 7279002e 6e762e69 6e666f00 .entry..nv.info.
   0x000a5f58 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x000a5f68 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x000a5f78 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x000a5f88 5f316231 64376430 655f3232 30303135 _1b1d7d0e_220015
+  0x000a5f88 5f313562 39356539 315f3235 38363135 _15b95e91_258615
   0x000a5f98 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x000a5fa8 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x000a5fb8 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x000a5fc8 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a5fd8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a5fe8 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x000a5ff8 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x000a5fe8 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x000a5ff8 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x000a6008 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x000a6018 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x000a6028 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x000a6038 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x000a6048 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x000a6058 6e6d735f 63755f31 62316437 6430655f nms_cu_1b1d7d0e_
-  0x000a6068 32323030 31356e6d 735f6b65 726e656c 220015nms_kernel
+  0x000a6058 6e6d735f 63755f31 35623935 6539315f nms_cu_15b95e91_
+  0x000a6068 32353836 31356e6d 735f6b65 726e656c 258615nms_kernel
   0x000a6078 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x000a6088 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x000a6098 2e676c6f 62616c00 2e6e762e 636f6e73 .global..nv.cons
   0x000a60a8 74616e74 302e5f5a 4e37746f 72636861 tant0._ZN7torcha
   0x000a60b8 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x000a60c8 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x000a60d8 5f316231 64376430 655f3232 30303135 _1b1d7d0e_220015
+  0x000a60d8 5f313562 39356539 315f3235 38363135 _15b95e91_258615
   0x000a60e8 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x000a60f8 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x000a6108 504b545f 5079002e 74657874 2e5f5a4e PKT_Py..text._ZN
   0x000a6118 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x000a6128 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x000a6138 5f6e6d73 5f63755f 31623164 37643065 _nms_cu_1b1d7d0e
-  0x000a6148 5f323230 3031356e 6d735f6b 65726e65 _220015nms_kerne
+  0x000a6138 5f6e6d73 5f63755f 31356239 35653931 _nms_cu_15b95e91
+  0x000a6148 5f323538 3631356e 6d735f6b 65726e65 _258615nms_kerne
   0x000a6158 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x000a6168 5f507900 2e6e762e 696e666f 2e5f5a4e _Py..nv.info._ZN
   0x000a6178 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x000a6188 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x000a6198 5f6e6d73 5f63755f 31623164 37643065 _nms_cu_1b1d7d0e
-  0x000a61a8 5f323230 3031356e 6d735f6b 65726e65 _220015nms_kerne
+  0x000a6198 5f6e6d73 5f63755f 31356239 35653931 _nms_cu_15b95e91
+  0x000a61a8 5f323538 3631356e 6d735f6b 65726e65 _258615nms_kerne
   0x000a61b8 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x000a61c8 5f507900 2e6e762e 73686172 65642e5f _Py..nv.shared._
   0x000a61d8 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x000a61e8 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x000a61f8 5f365f6e 6d735f63 755f3162 31643764 _6_nms_cu_1b1d7d
-  0x000a6208 30655f32 32303031 356e6d73 5f6b6572 0e_220015nms_ker
+  0x000a61f8 5f365f6e 6d735f63 755f3135 62393565 _6_nms_cu_15b95e
+  0x000a6208 39315f32 35383631 356e6d73 5f6b6572 91_258615nms_ker
   0x000a6218 6e656c5f 696d706c 49664545 76696450 nel_implIfEEvidP
   0x000a6228 4b545f50 79002e6e 762e636f 6e737461 KT_Py..nv.consta
   0x000a6238 6e74302e 5f5a4e37 746f7263 68616f34 nt0._ZN7torchao4
   0x000a6248 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
   0x000a6258 65393235 395f365f 6e6d735f 63755f31 e9259_6_nms_cu_1
-  0x000a6268 62316437 6430655f 32323030 31356e6d b1d7d0e_220015nm
+  0x000a6268 35623935 6539315f 32353836 31356e6d 5b95e91_258615nm
   0x000a6278 735f6b65 726e656c 5f696d70 6c496645 s_kernel_implIfE
   0x000a6288 45766964 504b545f 5079002e 74657874 EvidPKT_Py..text
   0x000a6298 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x000a62a8 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x000a62b8 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x000a62c8 37643065 5f323230 3031356e 6d735f6b 7d0e_220015nms_k
+  0x000a62b8 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x000a62c8 35653931 5f323538 3631356e 6d735f6b 5e91_258615nms_k
   0x000a62d8 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x000a62e8 64504b54 5f507900 2e6e762e 696e666f dPKT_Py..nv.info
   0x000a62f8 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x000a6308 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x000a6318 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x000a6328 37643065 5f323230 3031356e 6d735f6b 7d0e_220015nms_k
+  0x000a6318 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x000a6328 35653931 5f323538 3631356e 6d735f6b 5e91_258615nms_k
   0x000a6338 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x000a6348 64504b54 5f507900 2e6e762e 73686172 dPKT_Py..nv.shar
   0x000a6358 65642e5f 5a4e3774 6f726368 616f3433 ed._ZN7torchao43
   0x000a6368 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6378 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x000a6388 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x000a6378 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x000a6388 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x000a6398 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x000a63a8 76696450 4b545f50 79002e6e 762e636f vidPKT_Py..nv.co
   0x000a63b8 6e737461 6e74302e 5f5a4e37 746f7263 nstant0._ZN7torc
   0x000a63c8 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
   0x000a63d8 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
-  0x000a63e8 63755f31 62316437 6430655f 32323030 cu_1b1d7d0e_2200
+  0x000a63e8 63755f31 35623935 6539315f 32353836 cu_15b95e91_2586
   0x000a63f8 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
   0x000a6408 6c496445 45766964 504b545f 5079002e lIdEEvidPKT_Py..
   0x000a6418 64656275 675f6672 616d6500 2e72656c debug_frame..rel
   0x000a6428 2e646562 75675f66 72616d65 002e7265 .debug_frame..re
   0x000a6438 6c612e64 65627567 5f667261 6d650000 la.debug_frame..
   0x000a6448 2e736873 74727461 62002e73 74727461 .shstrtab..strta
   0x000a6458 62002e73 796d7461 62002e73 796d7461 b..symtab..symta
   0x000a6468 625f7368 6e647800 2e6e762e 7566742e b_shndx..nv.uft.
   0x000a6478 656e7472 79002e6e 762e696e 666f005f entry..nv.info._
   0x000a6488 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x000a6498 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x000a64a8 5f365f6e 6d735f63 755f3162 31643764 _6_nms_cu_1b1d7d
-  0x000a64b8 30655f32 32303031 356e6d73 5f6b6572 0e_220015nms_ker
+  0x000a64a8 5f365f6e 6d735f63 755f3135 62393565 _6_nms_cu_15b95e
+  0x000a64b8 39315f32 35383631 356e6d73 5f6b6572 91_258615nms_ker
   0x000a64c8 6e656c5f 696d706c 494e3363 31303448 nel_implIN3c104H
   0x000a64d8 616c6645 45457669 64504b54 5f507900 alfEEEvidPKT_Py.
   0x000a64e8 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x000a64f8 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x000a6508 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x000a6518 5f316231 64376430 655f3232 30303135 _1b1d7d0e_220015
+  0x000a6518 5f313562 39356539 315f3235 38363135 _15b95e91_258615
   0x000a6528 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x000a6538 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x000a6548 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x000a6558 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a6568 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a6578 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x000a6588 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x000a6578 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x000a6588 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x000a6598 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x000a65a8 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x000a65b8 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x000a65c8 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x000a65d8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x000a65e8 6e6d735f 63755f31 62316437 6430655f nms_cu_1b1d7d0e_
-  0x000a65f8 32323030 31356e6d 735f6b65 726e656c 220015nms_kernel
+  0x000a65e8 6e6d735f 63755f31 35623935 6539315f nms_cu_15b95e91_
+  0x000a65f8 32353836 31356e6d 735f6b65 726e656c 258615nms_kernel
   0x000a6608 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x000a6618 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x000a6628 2e676c6f 62616c00 5f5a4e34 315f494e .global._ZN41_IN
   0x000a6638 5445524e 414c5f35 62326539 3235395f TERNAL_5b2e9259_
-  0x000a6648 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x000a6658 655f3232 30303674 68727573 74367379 e_22006thrust6sy
+  0x000a6648 365f6e6d 735f6375 5f313562 39356539 6_nms_cu_15b95e9
+  0x000a6658 315f3235 38363674 68727573 74367379 1_25866thrust6sy
   0x000a6668 7374656d 36646574 61696c31 30736571 stem6detail10seq
   0x000a6678 75656e74 69616c33 73657145 00245f5a uential3seqE.$_Z
   0x000a6688 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
   0x000a6698 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x000a66a8 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x000a66b8 655f3232 30303135 6e6d735f 6b65726e e_220015nms_kern
+  0x000a66a8 365f6e6d 735f6375 5f313562 39356539 6_nms_cu_15b95e9
+  0x000a66b8 315f3235 38363135 6e6d735f 6b65726e 1_258615nms_kern
   0x000a66c8 656c5f69 6d706c49 4e336331 30344861 el_implIN3c104Ha
   0x000a66d8 6c664545 45766964 504b545f 5079245f lfEEEvidPKT_Py$_
   0x000a66e8 5f637564 615f736d 33785f64 69765f72 _cuda_sm3x_div_r
   0x000a66f8 6e5f6e6f 66747a5f 6633325f 736c6f77 n_noftz_f32_slow
   0x000a6708 70617468 00245f5f 5f5a5a4e 37746f72 path.$___ZZN7tor
   0x000a6718 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x000a6728 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x000a6738 5f63755f 31623164 37643065 5f323230 _cu_1b1d7d0e_220
-  0x000a6748 3031356e 6d735f6b 65726e65 6c5f696d 015nms_kernel_im
+  0x000a6738 5f63755f 31356239 35653931 5f323538 _cu_15b95e91_258
+  0x000a6748 3631356e 6d735f6b 65726e65 6c5f696d 615nms_kernel_im
   0x000a6758 706c494e 33633130 3448616c 66454545 plIN3c104HalfEEE
   0x000a6768 76696450 4b545f50 79453131 626c6f63 vidPKT_PyE11bloc
   0x000a6778 6b5f626f 7865735f 5f353337 002e6e76 k_boxes__537..nv
   0x000a6788 2e636f6e 7374616e 74302e5f 5a4e3774 .constant0._ZN7t
   0x000a6798 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x000a67a8 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x000a67b8 6d735f63 755f3162 31643764 30655f32 ms_cu_1b1d7d0e_2
-  0x000a67c8 32303031 356e6d73 5f6b6572 6e656c5f 20015nms_kernel_
+  0x000a67b8 6d735f63 755f3135 62393565 39315f32 ms_cu_15b95e91_2
+  0x000a67c8 35383631 356e6d73 5f6b6572 6e656c5f 58615nms_kernel_
   0x000a67d8 696d706c 494e3363 31303448 616c6645 implIN3c104HalfE
   0x000a67e8 45457669 64504b54 5f507900 5f706172 EEvidPKT_Py._par
   0x000a67f8 616d005f 5a4e3774 6f726368 616f3433 am._ZN7torchao43
   0x000a6808 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6818 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x000a6828 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x000a6818 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x000a6828 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x000a6838 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x000a6848 76696450 4b545f50 79002e74 6578742e vidPKT_Py..text.
   0x000a6858 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a6868 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a6878 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x000a6888 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x000a6878 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x000a6888 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x000a6898 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x000a68a8 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x000a68b8 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a68c8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a68d8 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x000a68e8 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
+  0x000a68d8 395f365f 6e6d735f 63755f31 35623935 9_6_nms_cu_15b95
+  0x000a68e8 6539315f 32353836 31356e6d 735f6b65 e91_258615nms_ke
   0x000a68f8 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x000a6908 504b545f 5079002e 6e762e73 68617265 PKT_Py..nv.share
   0x000a6918 642e5f5a 4e37746f 72636861 6f34335f d._ZN7torchao43_
   0x000a6928 474c4f42 414c5f5f 4e5f5f35 62326539 GLOBAL__N__5b2e9
-  0x000a6938 3235395f 365f6e6d 735f6375 5f316231 259_6_nms_cu_1b1
-  0x000a6948 64376430 655f3232 30303135 6e6d735f d7d0e_220015nms_
+  0x000a6938 3235395f 365f6e6d 735f6375 5f313562 259_6_nms_cu_15b
+  0x000a6948 39356539 315f3235 38363135 6e6d735f 95e91_258615nms_
   0x000a6958 6b65726e 656c5f69 6d706c49 66454576 kernel_implIfEEv
   0x000a6968 6964504b 545f5079 00245f5a 4e37746f idPKT_Py.$_ZN7to
   0x000a6978 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x000a6988 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x000a6998 735f6375 5f316231 64376430 655f3232 s_cu_1b1d7d0e_22
-  0x000a69a8 30303135 6e6d735f 6b65726e 656c5f69 0015nms_kernel_i
+  0x000a6998 735f6375 5f313562 39356539 315f3235 s_cu_15b95e91_25
+  0x000a69a8 38363135 6e6d735f 6b65726e 656c5f69 8615nms_kernel_i
   0x000a69b8 6d706c49 66454576 6964504b 545f5079 mplIfEEvidPKT_Py
   0x000a69c8 245f5f63 7564615f 736d3378 5f646976 $__cuda_sm3x_div
   0x000a69d8 5f726e5f 6e6f6674 7a5f6633 325f736c _rn_noftz_f32_sl
   0x000a69e8 6f777061 74680024 5f5f5f5a 5a4e3774 owpath.$___ZZN7t
   0x000a69f8 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x000a6a08 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x000a6a18 6d735f63 755f3162 31643764 30655f32 ms_cu_1b1d7d0e_2
-  0x000a6a28 32303031 356e6d73 5f6b6572 6e656c5f 20015nms_kernel_
+  0x000a6a18 6d735f63 755f3135 62393565 39315f32 ms_cu_15b95e91_2
+  0x000a6a28 35383631 356e6d73 5f6b6572 6e656c5f 58615nms_kernel_
   0x000a6a38 696d706c 49664545 76696450 4b545f50 implIfEEvidPKT_P
   0x000a6a48 79453131 626c6f63 6b5f626f 7865735f yE11block_boxes_
   0x000a6a58 5f323834 002e6e76 2e636f6e 7374616e _284..nv.constan
   0x000a6a68 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x000a6a78 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6a88 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x000a6a98 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x000a6a88 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x000a6a98 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x000a6aa8 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x000a6ab8 76696450 4b545f50 79005f5a 4e37746f vidPKT_Py._ZN7to
   0x000a6ac8 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x000a6ad8 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x000a6ae8 735f6375 5f316231 64376430 655f3232 s_cu_1b1d7d0e_22
-  0x000a6af8 30303135 6e6d735f 6b65726e 656c5f69 0015nms_kernel_i
+  0x000a6ae8 735f6375 5f313562 39356539 315f3235 s_cu_15b95e91_25
+  0x000a6af8 38363135 6e6d735f 6b65726e 656c5f69 8615nms_kernel_i
   0x000a6b08 6d706c49 64454576 6964504b 545f5079 mplIdEEvidPKT_Py
   0x000a6b18 002e7465 78742e5f 5a4e3774 6f726368 ..text._ZN7torch
   0x000a6b28 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x000a6b38 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x000a6b48 755f3162 31643764 30655f32 32303031 u_1b1d7d0e_22001
+  0x000a6b48 755f3135 62393565 39315f32 35383631 u_15b95e91_25861
   0x000a6b58 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x000a6b68 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x000a6b78 762e696e 666f2e5f 5a4e3774 6f726368 v.info._ZN7torch
   0x000a6b88 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x000a6b98 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x000a6ba8 755f3162 31643764 30655f32 32303031 u_1b1d7d0e_22001
+  0x000a6ba8 755f3135 62393565 39315f32 35383631 u_15b95e91_25861
   0x000a6bb8 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x000a6bc8 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x000a6bd8 762e7368 61726564 2e5f5a4e 37746f72 v.shared._ZN7tor
   0x000a6be8 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x000a6bf8 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x000a6c08 5f63755f 31623164 37643065 5f323230 _cu_1b1d7d0e_220
-  0x000a6c18 3031356e 6d735f6b 65726e65 6c5f696d 015nms_kernel_im
+  0x000a6c08 5f63755f 31356239 35653931 5f323538 _cu_15b95e91_258
+  0x000a6c18 3631356e 6d735f6b 65726e65 6c5f696d 615nms_kernel_im
   0x000a6c28 706c4964 45457669 64504b54 5f507900 plIdEEvidPKT_Py.
   0x000a6c38 245f5a4e 37746f72 6368616f 34335f47 $_ZN7torchao43_G
   0x000a6c48 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x000a6c58 35395f36 5f6e6d73 5f63755f 31623164 59_6_nms_cu_1b1d
-  0x000a6c68 37643065 5f323230 3031356e 6d735f6b 7d0e_220015nms_k
+  0x000a6c58 35395f36 5f6e6d73 5f63755f 31356239 59_6_nms_cu_15b9
+  0x000a6c68 35653931 5f323538 3631356e 6d735f6b 5e91_258615nms_k
   0x000a6c78 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x000a6c88 64504b54 5f507924 5f5f6375 64615f73 dPKT_Py$__cuda_s
   0x000a6c98 6d32305f 6469765f 6636345f 736c6f77 m20_div_f64_slow
   0x000a6ca8 70617468 5f763200 245f5f5f 5a5a4e37 path_v2.$___ZZN7
   0x000a6cb8 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x000a6cc8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x000a6cd8 6e6d735f 63755f31 62316437 6430655f nms_cu_1b1d7d0e_
-  0x000a6ce8 32323030 31356e6d 735f6b65 726e656c 220015nms_kernel
+  0x000a6cd8 6e6d735f 63755f31 35623935 6539315f nms_cu_15b95e91_
+  0x000a6ce8 32353836 31356e6d 735f6b65 726e656c 258615nms_kernel
   0x000a6cf8 5f696d70 6c496445 45766964 504b545f _implIdEEvidPKT_
   0x000a6d08 50794531 31626c6f 636b5f62 6f786573 PyE11block_boxes
   0x000a6d18 5f5f3331 002e6e76 2e636f6e 7374616e __31..nv.constan
   0x000a6d28 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x000a6d38 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6d48 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x000a6d58 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
+  0x000a6d48 39323539 5f365f6e 6d735f63 755f3135 9259_6_nms_cu_15
+  0x000a6d58 62393565 39315f32 35383631 356e6d73 b95e91_258615nms
   0x000a6d68 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x000a6d78 76696450 4b545f50 79002e64 65627567 vidPKT_Py..debug
   0x000a6d88 5f667261 6d65002e 72656c2e 64656275 _frame..rel.debu
   0x000a6d98 675f6672 616d6500 2e72656c 612e6465 g_frame..rela.de
   0x000a6da8 6275675f 6672616d 65000000 00000000 bug_frame.......
   0x000a6db8 00000000 00000000 00000000 00000000 ................
   0x000a6dc8 00000000 00000000 40000000 02100d00 ........@.......
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
-  0x00000000 00746d70 7866745f 30303030 30383735 .tmpxft_00000875
+  0x00000000 00746d70 7866745f 30303030 30396637 .tmpxft_000009f7
   0x00000010 5f303030 30303030 302d365f 6670365f _00000000-6_fp6_
   0x00000020 6c696e65 61722e63 6f6d7075 74655f38 linear.compute_8
   0x00000030 362e6375 64616665 312e6370 70006661 6.cudafe1.cpp.fa
   0x00000040 7462696e 44617461 005f5a39 4b65726e tbinData._Z9Kern
   0x00000050 656c5f45 78493132 54696c69 6e67436f el_ExI12TilingCo
   0x00000060 6e666967 494c6934 454c6931 454c6938 nfigILi4ELi1ELi8
   0x00000070 45456645 76503131 43557374 7265616d EEfEvP11CUstream
@@ -133,29 +133,29 @@
   0x00000820 5f6b6579 7365745f 77697468 5f414449 _keyset_with_ADI
   0x00000830 6e706c61 63654f72 56696577 45005f5a nplaceOrViewE._Z
   0x00000840 4e37746f 72636861 6f323366 70365f6c N7torchao23fp6_l
   0x00000850 696e6561 725f666f 72776172 645f6375 inear_forward_cu
   0x00000860 6461454e 32617436 54656e73 6f724553 daEN2at6TensorES
   0x00000870 315f5331 5f6c2e63 6f6c6400 5f474c4f 1_S1_l.cold._GLO
   0x00000880 42414c5f 5f737562 5f495f74 6d707866 BAL__sub_I_tmpxf
-  0x00000890 745f3030 30303038 37355f30 30303030 t_00000875_00000
+  0x00000890 745f3030 30303039 66375f30 30303030 t_000009f7_00000
   0x000008a0 3030305f 365f6670 365f6c69 6e656172 000_6_fp6_linear
   0x000008b0 2e636f6d 70757465 5f38362e 63756461 .compute_86.cuda
   0x000008c0 6665312e 63707000 5f5a5374 4c385f5f fe1.cpp._ZStL8__
   0x000008d0 696f696e 6974005f 5a4e3774 6f726368 ioinit._ZN7torch
   0x000008e0 616f4c34 35544f52 43485f4c 49425241 aoL45TORCH_LIBRA
   0x000008f0 52595f49 4d504c5f 73746174 69635f69 RY_IMPL_static_i
   0x00000900 6e69745f 746f7263 68616f5f 43554441 nit_torchao_CUDA
   0x00000910 5f324500 5f474c4f 42414c5f 5f737562 _2E._GLOBAL__sub
-  0x00000920 5f495f74 6d707866 745f3030 30303038 _I_tmpxft_000008
-  0x00000930 37355f30 30303030 3030305f 365f6670 75_00000000_6_fp
+  0x00000920 5f495f74 6d707866 745f3030 30303039 _I_tmpxft_000009
+  0x00000930 66375f30 30303030 3030305f 365f6670 f7_00000000_6_fp
   0x00000940 365f6c69 6e656172 2e636f6d 70757465 6_linear.compute
   0x00000950 5f38362e 63756461 6665312e 6370702e _86.cudafe1.cpp.
   0x00000960 636f6c64 00746d70 7866745f 30303030 cold.tmpxft_0000
-  0x00000970 30383736 5f303030 30303030 302d365f 0876_00000000-6_
+  0x00000970 30396638 5f303030 30303030 302d365f 09f8_00000000-6_
   0x00000980 77656967 68745f71 75616e74 2e636f6d weight_quant.com
   0x00000990 70757465 5f38362e 63756461 6665312e pute_86.cudafe1.
   0x000009a0 63707000 5f5a3133 63617374 5f667031 cpp._Z13cast_fp1
   0x000009b0 365f6670 36507450 682e636f 6c64005f 6_fp6PtPh.cold._
   0x000009c0 5a323977 65696768 745f7072 65706163 Z29weight_prepac
   0x000009d0 6b696e67 5f667031 365f746f 5f667036 king_fp16_to_fp6
   0x000009e0 50745068 6d6d2e63 6f6c6400 5f5a4e37 PtPhmm.cold._ZN7
@@ -163,46 +163,46 @@
   0x00000a00 5f667036 5f637075 454e3261 74365465 _fp6_cpuEN2at6Te
   0x00000a10 6e736f72 452e636f 6c64005f 5a4e3774 nsorE.cold._ZN7t
   0x00000a20 6f726368 616f3235 77656967 68745f6d orchao25weight_m
   0x00000a30 61747269 785f6465 7175616e 745f6370 atrix_dequant_cp
   0x00000a40 75454e32 61743654 656e736f 72455331 uEN2at6TensorES1
   0x00000a50 5f2e636f 6c64005f 474c4f42 414c5f5f _.cold._GLOBAL__
   0x00000a60 7375625f 495f746d 70786674 5f303030 sub_I_tmpxft_000
-  0x00000a70 30303837 365f3030 30303030 30305f36 00876_00000000_6
+  0x00000a70 30303966 385f3030 30303030 30305f36 009f8_00000000_6
   0x00000a80 5f776569 6768745f 7175616e 742e636f _weight_quant.co
   0x00000a90 6d707574 655f3836 2e637564 61666531 mpute_86.cudafe1
   0x00000aa0 2e637070 005f5a4e 37746f72 6368616f .cpp._ZN7torchao
   0x00000ab0 4c343454 4f524348 5f4c4942 52415259 L44TORCH_LIBRARY
   0x00000ac0 5f494d50 4c5f7374 61746963 5f696e69 _IMPL_static_ini
   0x00000ad0 745f746f 72636861 6f5f4350 555f3245 t_torchao_CPU_2E
   0x00000ae0 005f474c 4f42414c 5f5f7375 625f495f ._GLOBAL__sub_I_
-  0x00000af0 746d7078 66745f30 30303030 3837365f tmpxft_00000876_
+  0x00000af0 746d7078 66745f30 30303030 3966385f tmpxft_000009f8_
   0x00000b00 30303030 30303030 5f365f77 65696768 00000000_6_weigh
   0x00000b10 745f7175 616e742e 636f6d70 7574655f t_quant.compute_
   0x00000b20 38362e63 75646166 65312e63 70702e63 86.cudafe1.cpp.c
   0x00000b30 6f6c6400 746d7078 66745f30 30303030 old.tmpxft_00000
-  0x00000b40 3837375f 30303030 30303030 2d365f6e 877_00000000-6_n
+  0x00000b40 3966395f 30303030 30303030 2d365f6e 9f9_00000000-6_n
   0x00000b50 6d732e63 6f6d7075 74655f38 362e6375 ms.compute_86.cu
   0x00000b60 64616665 312e6370 70005f5a 4e336331 dafe1.cpp._ZN3c1
   0x00000b70 304c3874 6f537472 696e6745 4e535f31 0L8toStringENS_1
   0x00000b80 30536361 6c617254 79706545 005f5a4e 0ScalarTypeE._ZN
   0x00000b90 33633130 3653796d 496e7438 72656c65 3c106SymInt8rele
   0x00000ba0 6173655f 45762e70 6172742e 30005f5a ase_Ev.part.0._Z
   0x00000bb0 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
   0x00000bc0 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x00000bd0 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x00000be0 655f3232 30303130 6e6d735f 6b65726e e_220010nms_kern
+  0x00000bd0 365f6e6d 735f6375 5f313562 39356539 6_nms_cu_15b95e9
+  0x00000be0 315f3235 38363130 6e6d735f 6b65726e 1_258610nms_kern
   0x00000bf0 656c4552 4b4e3261 74365465 6e736f72 elERKN2at6Tensor
   0x00000c00 4553345f 642e636f 6c64005f 474c4f42 ES4_d.cold._GLOB
   0x00000c10 414c5f5f 7375625f 495f746d 70786674 AL__sub_I_tmpxft
-  0x00000c20 5f303030 30303837 375f3030 30303030 _00000877_000000
+  0x00000c20 5f303030 30303966 395f3030 30303030 _000009f9_000000
   0x00000c30 30305f36 5f6e6d73 2e636f6d 70757465 00_6_nms.compute
   0x00000c40 5f38362e 63756461 6665312e 63707000 _86.cudafe1.cpp.
   0x00000c50 5f474c4f 42414c5f 5f737562 5f495f74 _GLOBAL__sub_I_t
-  0x00000c60 6d707866 745f3030 30303038 37375f30 mpxft_00000877_0
+  0x00000c60 6d707866 745f3030 30303039 66395f30 mpxft_000009f9_0
   0x00000c70 30303030 3030305f 365f6e6d 732e636f 0000000_6_nms.co
   0x00000c80 6d707574 655f3836 2e637564 61666531 mpute_86.cudafe1
   0x00000c90 2e637070 2e636f6c 64005f47 4c4f4241 .cpp.cold._GLOBA
   0x00000ca0 4c5f5f73 75625f49 5f667036 5f6c6c6d L__sub_I_fp6_llm
   0x00000cb0 2e637070 005f5a4c 3434544f 5243485f .cpp._ZL44TORCH_
   0x00000cc0 4c494252 4152595f 46524147 4d454e54 LIBRARY_FRAGMENT
   0x00000cd0 5f737461 7469635f 696e6974 5f746f72 _static_init_tor
@@ -939,95 +939,95 @@
   0x00003a80 61726765 745f6465 6661756c 745f6e75 arget_default_nu
   0x00003a90 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
   0x00003aa0 5f5a4e4b 33633130 36495661 6c756537 _ZNK3c106IValue7
   0x00003ab0 7461674b 696e6445 76005f5a 4e4b3363 tagKindEv._ZNK3c
   0x00003ac0 31303469 6d706c31 36566972 7475616c 104impl16Virtual
   0x00003ad0 47756172 64496d70 6c396765 74537472 GuardImpl9getStr
   0x00003ae0 65616d45 4e535f36 44657669 63654500 eamENS_6DeviceE.
-  0x00003af0 5f66696e 69005f5a 4e4b5374 39747970 _fini._ZNKSt9typ
-  0x00003b00 655f696e 666f3968 6173685f 636f6465 e_info9hash_code
-  0x00003b10 4576005f 5a4e3363 31303230 696e7472 Ev._ZN3c1020intr
-  0x00003b20 75736976 655f7074 725f7461 72676574 usive_ptr_target
-  0x00003b30 44314576 005f5a4e 33633130 3133696e D1Ev._ZN3c1013in
-  0x00003b40 74727573 6976655f 70747249 4e535f31 trusive_ptrINS_1
-  0x00003b50 3054656e 736f7249 6d706c45 4e535f36 0TensorImplENS_6
-  0x00003b60 64657461 696c3334 696e7472 75736976 detail34intrusiv
-  0x00003b70 655f7461 72676574 5f646566 61756c74 e_target_default
-  0x00003b80 5f6e756c 6c5f7479 70654953 315f4545 _null_typeIS1_EE
-  0x00003b90 45367265 7365745f 45760050 794f626a E6reset_Ev.PyObj
-  0x00003ba0 6563745f 53657441 74747253 7472696e ect_SetAttrStrin
-  0x00003bb0 67005f5a 4e4b3363 31303469 6d706c31 g._ZNK3c104impl1
-  0x00003bc0 36566972 7475616c 47756172 64496d70 6VirtualGuardImp
-  0x00003bd0 6c313264 65737472 6f794576 656e7445 l12destroyEventE
-  0x00003be0 50766100 50795479 70655f49 73537562 Pva.PyType_IsSub
-  0x00003bf0 74797065 006d656d 6d6f7665 40474c49 type.memmove@GLI
-  0x00003c00 42435f32 2e322e35 005f5a4e 33633130 BC_2.2.5._ZN3c10
-  0x00003c10 31386765 7446616b 65547970 65507472 18getFakeTypePtr
-  0x00003c20 436f7079 494e3261 74365465 6e736f72 CopyIN2at6Tensor
-  0x00003c30 4545454e 535f3454 79706532 3453696e EEENS_4Type24Sin
-  0x00003c40 676c6574 6f6e4f72 53686172 65645479 gletonOrSharedTy
-  0x00003c50 70655074 72495333 5f454576 005f5a4e pePtrIS3_EEv._ZN
-  0x00003c60 33633130 36646574 61696c31 325f7374 3c106detail12_st
-  0x00003c70 725f7772 61707065 72494a50 4b63524b r_wrapperIJPKcRK
-  0x00003c80 6c53335f 45453463 616c6c45 524b5333 lS3_EE4callERKS3
-  0x00003c90 5f53355f 53385f00 5f5a4e33 63313031 _S5_S8_._ZN3c101
-  0x00003ca0 39556e64 6566696e 65645465 6e736f72 9UndefinedTensor
-  0x00003cb0 496d706c 31305f73 696e676c 65746f6e Impl10_singleton
-  0x00003cc0 45005f5a 4e336331 3034696d 706c3331 E._ZN3c104impl31
-  0x00003cd0 6d616b65 5f626f78 65645f66 726f6d5f make_boxed_from_
-  0x00003ce0 756e626f 7865645f 66756e63 746f7249 unboxed_functorI
-  0x00003cf0 4e53305f 36646574 61696c33 31577261 NS0_6detail31Wra
-  0x00003d00 7046756e 6374696f 6e496e74 6f52756e pFunctionIntoRun
-  0x00003d10 74696d65 46756e63 746f725f 4950464e timeFunctor_IPFN
-  0x00003d20 32617436 54656e73 6f724552 4b53355f 2at6TensorERKS5_
-  0x00003d30 53375f64 4553355f 4e535f34 67757473 S7_dES5_NS_4guts
-  0x00003d40 38747970 656c6973 74387479 70656c69 8typelist8typeli
-  0x00003d50 7374494a 53375f53 375f6445 45454545 stIJS7_S7_dEEEEE
-  0x00003d60 4c623045 45346361 6c6c4550 4e535f31 Lb0EE4callEPNS_1
-  0x00003d70 344f7065 7261746f 724b6572 6e656c45 4OperatorKernelE
-  0x00003d80 524b4e53 5f31344f 70657261 746f7248 RKNS_14OperatorH
-  0x00003d90 616e646c 65454e53 5f313444 69737061 andleENS_14Dispa
-  0x00003da0 7463684b 65795365 74455053 74367665 tchKeySetEPSt6ve
-  0x00003db0 63746f72 494e535f 36495661 6c756545 ctorINS_6IValueE
-  0x00003dc0 53614953 4e5f4545 00507945 72725f46 SaISN_EE.PyErr_F
-  0x00003dd0 65746368 005f5a4e 33633130 34696d70 etch._ZN3c104imp
-  0x00003de0 6c323877 7261705f 6b65726e 656c5f66 l28wrap_kernel_f
-  0x00003df0 756e6374 6f725f75 6e626f78 65645f49 unctor_unboxed_I
-  0x00003e00 4e53305f 36646574 61696c33 31577261 NS0_6detail31Wra
-  0x00003e10 7046756e 6374696f 6e496e74 6f52756e pFunctionIntoRun
-  0x00003e20 74696d65 46756e63 746f725f 4950464e timeFunctor_IPFN
-  0x00003e30 32617436 54656e73 6f724553 355f5335 2at6TensorES5_S5
-  0x00003e40 5f455335 5f4e535f 34677574 73387479 _ES5_NS_4guts8ty
-  0x00003e50 70656c69 73743874 7970656c 69737449 pelist8typelistI
-  0x00003e60 4a53355f 53355f45 45454545 53365f45 JS5_S5_EEEEES6_E
-  0x00003e70 3463616c 6c45504e 535f3134 4f706572 4callEPNS_14Oper
-  0x00003e80 61746f72 4b65726e 656c454e 535f3134 atorKernelENS_14
-  0x00003e90 44697370 61746368 4b657953 65744553 DispatchKeySetES
-  0x00003ea0 355f5335 5f005079 45786365 7074696f 5_S5_.PyExceptio
-  0x00003eb0 6e5f5365 74547261 63656261 636b005f n_SetTraceback._
-  0x00003ec0 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
-  0x00003ed0 6d706c31 32636f6e 7374616e 745f696e mpl12constant_in
-  0x00003ee0 74457600 5f5f6173 73657274 5f666169 tEv.__assert_fai
-  0x00003ef0 6c40474c 4942435f 322e322e 35005f5a l@GLIBC_2.2.5._Z
-  0x00003f00 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
-  0x00003f10 706c3238 69735f6e 6f6e5f6f 7665726c pl28is_non_overl
-  0x00003f20 61707069 6e675f61 6e645f64 656e7365 apping_and_dense
-  0x00003f30 454e535f 38417272 61795265 66494e53 ENS_8ArrayRefINS
-  0x00003f40 5f313369 6e747275 73697665 5f707472 _13intrusive_ptr
-  0x00003f50 4953305f 4e535f36 64657461 696c3334 IS0_NS_6detail34
-  0x00003f60 696e7472 75736976 655f7461 72676574 intrusive_target
-  0x00003f70 5f646566 61756c74 5f6e756c 6c5f7479 _default_null_ty
-  0x00003f80 70654953 305f4545 45454545 53375f00 peIS0_EEEEEES7_.
-  0x00003f90 50794578 635f5275 6e74696d 65457272 PyExc_RuntimeErr
-  0x00003fa0 6f72005f 5a4e3774 6f726368 616f3433 or._ZN7torchao43
-  0x00003fb0 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x00003fc0 39323539 5f365f6e 6d735f63 755f3162 9259_6_nms_cu_1b
-  0x00003fd0 31643764 30655f32 32303031 356e6d73 1d7d0e_220015nms
-  0x00003fe0 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
-  0x00003ff0 76696450 4b545f50 79005f5a 4e336331 vidPKT_Py._ZN3c1
+  0x00003af0 5f66696e 69005f5a 4e37746f 72636861 _fini._ZN7torcha
+  0x00003b00 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
+  0x00003b10 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
+  0x00003b20 5f313562 39356539 315f3235 38363135 _15b95e91_258615
+  0x00003b30 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
+  0x00003b40 64454576 6964504b 545f5079 005f5a4e dEEvidPKT_Py._ZN
+  0x00003b50 4b537439 74797065 5f696e66 6f396861 KSt9type_info9ha
+  0x00003b60 73685f63 6f646545 76005f5a 4e336331 sh_codeEv._ZN3c1
+  0x00003b70 30323069 6e747275 73697665 5f707472 020intrusive_ptr
+  0x00003b80 5f746172 67657444 31457600 5f5a4e33 _targetD1Ev._ZN3
+  0x00003b90 63313031 33696e74 72757369 76655f70 c1013intrusive_p
+  0x00003ba0 7472494e 535f3130 54656e73 6f72496d trINS_10TensorIm
+  0x00003bb0 706c454e 535f3664 65746169 6c333469 plENS_6detail34i
+  0x00003bc0 6e747275 73697665 5f746172 6765745f ntrusive_target_
+  0x00003bd0 64656661 756c745f 6e756c6c 5f747970 default_null_typ
+  0x00003be0 65495331 5f454545 36726573 65745f45 eIS1_EEE6reset_E
+  0x00003bf0 76005079 4f626a65 63745f53 65744174 v.PyObject_SetAt
+  0x00003c00 74725374 72696e67 005f5a4e 4b336331 trString._ZNK3c1
+  0x00003c10 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
+  0x00003c20 75617264 496d706c 31326465 7374726f uardImpl12destro
+  0x00003c30 79457665 6e744550 76610050 79547970 yEventEPva.PyTyp
+  0x00003c40 655f4973 53756274 79706500 6d656d6d e_IsSubtype.memm
+  0x00003c50 6f766540 474c4942 435f322e 322e3500 ove@GLIBC_2.2.5.
+  0x00003c60 5f5a4e33 63313031 38676574 46616b65 _ZN3c1018getFake
+  0x00003c70 54797065 50747243 6f707949 4e326174 TypePtrCopyIN2at
+  0x00003c80 3654656e 736f7245 45454e53 5f345479 6TensorEEENS_4Ty
+  0x00003c90 70653234 53696e67 6c65746f 6e4f7253 pe24SingletonOrS
+  0x00003ca0 68617265 64547970 65507472 4953335f haredTypePtrIS3_
+  0x00003cb0 45457600 5f5a4e33 63313036 64657461 EEv._ZN3c106deta
+  0x00003cc0 696c3132 5f737472 5f777261 70706572 il12_str_wrapper
+  0x00003cd0 494a504b 63524b6c 53335f45 45346361 IJPKcRKlS3_EE4ca
+  0x00003ce0 6c6c4552 4b53335f 53355f53 385f005f llERKS3_S5_S8_._
+  0x00003cf0 5a4e3363 31303139 556e6465 66696e65 ZN3c1019Undefine
+  0x00003d00 6454656e 736f7249 6d706c31 305f7369 dTensorImpl10_si
+  0x00003d10 6e676c65 746f6e45 005f5a4e 33633130 ngletonE._ZN3c10
+  0x00003d20 34696d70 6c33316d 616b655f 626f7865 4impl31make_boxe
+  0x00003d30 645f6672 6f6d5f75 6e626f78 65645f66 d_from_unboxed_f
+  0x00003d40 756e6374 6f72494e 53305f36 64657461 unctorINS0_6deta
+  0x00003d50 696c3331 57726170 46756e63 74696f6e il31WrapFunction
+  0x00003d60 496e746f 52756e74 696d6546 756e6374 IntoRuntimeFunct
+  0x00003d70 6f725f49 50464e32 61743654 656e736f or_IPFN2at6Tenso
+  0x00003d80 7245524b 53355f53 375f6445 53355f4e rERKS5_S7_dES5_N
+  0x00003d90 535f3467 75747338 74797065 6c697374 S_4guts8typelist
+  0x00003da0 38747970 656c6973 74494a53 375f5337 8typelistIJS7_S7
+  0x00003db0 5f644545 4545454c 62304545 3463616c _dEEEEELb0EE4cal
+  0x00003dc0 6c45504e 535f3134 4f706572 61746f72 lEPNS_14Operator
+  0x00003dd0 4b65726e 656c4552 4b4e535f 31344f70 KernelERKNS_14Op
+  0x00003de0 65726174 6f724861 6e646c65 454e535f eratorHandleENS_
+  0x00003df0 31344469 73706174 63684b65 79536574 14DispatchKeySet
+  0x00003e00 45505374 36766563 746f7249 4e535f36 EPSt6vectorINS_6
+  0x00003e10 4956616c 75654553 6149534e 5f454500 IValueESaISN_EE.
+  0x00003e20 50794572 725f4665 74636800 5f5a4e33 PyErr_Fetch._ZN3
+  0x00003e30 63313034 696d706c 32387772 61705f6b c104impl28wrap_k
+  0x00003e40 65726e65 6c5f6675 6e63746f 725f756e ernel_functor_un
+  0x00003e50 626f7865 645f494e 53305f36 64657461 boxed_INS0_6deta
+  0x00003e60 696c3331 57726170 46756e63 74696f6e il31WrapFunction
+  0x00003e70 496e746f 52756e74 696d6546 756e6374 IntoRuntimeFunct
+  0x00003e80 6f725f49 50464e32 61743654 656e736f or_IPFN2at6Tenso
+  0x00003e90 72455335 5f53355f 4553355f 4e535f34 rES5_S5_ES5_NS_4
+  0x00003ea0 67757473 38747970 656c6973 74387479 guts8typelist8ty
+  0x00003eb0 70656c69 7374494a 53355f53 355f4545 pelistIJS5_S5_EE
+  0x00003ec0 45454553 365f4534 63616c6c 45504e53 EEES6_E4callEPNS
+  0x00003ed0 5f31344f 70657261 746f724b 65726e65 _14OperatorKerne
+  0x00003ee0 6c454e53 5f313444 69737061 7463684b lENS_14DispatchK
+  0x00003ef0 65795365 74455335 5f53355f 00507945 eySetES5_S5_.PyE
+  0x00003f00 78636570 74696f6e 5f536574 54726163 xception_SetTrac
+  0x00003f10 65626163 6b005f5a 4e336331 30313153 eback._ZN3c1011S
+  0x00003f20 796d4e6f 6465496d 706c3132 636f6e73 ymNodeImpl12cons
+  0x00003f30 74616e74 5f696e74 4576005f 5f617373 tant_intEv.__ass
+  0x00003f40 6572745f 6661696c 40474c49 42435f32 ert_fail@GLIBC_2
+  0x00003f50 2e322e35 005f5a4e 33633130 31315379 .2.5._ZN3c1011Sy
+  0x00003f60 6d4e6f64 65496d70 6c323869 735f6e6f mNodeImpl28is_no
+  0x00003f70 6e5f6f76 65726c61 7070696e 675f616e n_overlapping_an
+  0x00003f80 645f6465 6e736545 4e535f38 41727261 d_denseENS_8Arra
+  0x00003f90 79526566 494e535f 3133696e 74727573 yRefINS_13intrus
+  0x00003fa0 6976655f 70747249 53305f4e 535f3664 ive_ptrIS0_NS_6d
+  0x00003fb0 65746169 6c333469 6e747275 73697665 etail34intrusive
+  0x00003fc0 5f746172 6765745f 64656661 756c745f _target_default_
+  0x00003fd0 6e756c6c 5f747970 65495330 5f454545 null_typeIS0_EEE
+  0x00003fe0 45454553 375f0050 79457863 5f52756e EEES7_.PyExc_Run
+  0x00003ff0 74696d65 4572726f 72005f5a 4e336331 timeError._ZN3c1
   0x00004000 30313153 796d4e6f 6465496d 706c3977 011SymNodeImpl9w
   0x00004010 7261705f 626f6f6c 4562005f 5a4e3363 rap_boolEb._ZN3c
   0x00004020 31303131 53796d4e 6f646549 6d706c32 1011SymNodeImpl2
   0x00004030 67744552 4b4e535f 3133696e 74727573 gtERKNS_13intrus
   0x00004040 6976655f 70747249 53305f4e 535f3664 ive_ptrIS0_NS_6d
   0x00004050 65746169 6c333469 6e747275 73697665 etail34intrusive
   0x00004060 5f746172 6765745f 64656661 756c745f _target_default_
@@ -1218,602 +1218,602 @@
   0x00004bf0 5f332e34 005f5a31 37515541 4e545f47 _3.4._Z17QUANT_G
   0x00004c00 454d4d5f 4b65726e 656c4931 3254696c EMM_KernelI12Til
   0x00004c10 696e6743 6f6e6669 67494c69 34454c69 ingConfigILi4ELi
   0x00004c20 31454c69 34454566 4576504b 3575696e 1ELi4EEfEvPK5uin
   0x00004c30 7434504b 365f5f68 616c6653 375f5054 t4PK6__halfS7_PT
   0x00004c40 305f6d6d 6d69005f 5f637861 5f677561 0_mmmi.__cxa_gua
   0x00004c50 72645f61 626f7274 40435858 4142495f rd_abort@CXXABI_
-  0x00004c60 312e3300 63756461 53747265 616d5175 1.3.cudaStreamQu
-  0x00004c70 65727940 6c696263 75646172 742e736f ery@libcudart.so
-  0x00004c80 2e313200 5f5f6375 64615265 67697374 .12.__cudaRegist
-  0x00004c90 65724661 7442696e 61727940 6c696263 erFatBinary@libc
-  0x00004ca0 75646172 742e736f 2e313200 5f5a4e33 udart.so.12._ZN3
-  0x00004cb0 63313031 3054656e 736f7254 79706533 c1010TensorType3
-  0x00004cc0 67657445 76005f5a 4e4b3363 31303469 getEv._ZNK3c104i
-  0x00004cd0 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
-  0x00004ce0 64496d70 6c35626c 6f636b45 5076524b dImpl5blockEPvRK
-  0x00004cf0 4e535f36 53747265 616d4500 5f5a4e33 NS_6StreamE._ZN3
-  0x00004d00 63313036 53796d49 6e744331 454e535f c106SymIntC1ENS_
-  0x00004d10 3133696e 74727573 6976655f 70747249 13intrusive_ptrI
-  0x00004d20 4e535f31 3153796d 4e6f6465 496d706c NS_11SymNodeImpl
-  0x00004d30 454e535f 36646574 61696c33 34696e74 ENS_6detail34int
-  0x00004d40 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x00004d50 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x00004d60 53325f45 45454500 5f5a4e33 63313034 S2_EEEE._ZN3c104
-  0x00004d70 63756461 31344578 6368616e 67654465 cuda14ExchangeDe
-  0x00004d80 76696365 4561005f 5a4e3363 31303463 viceEa._ZN3c104c
-  0x00004d90 75646132 30736574 43757272 656e7443 uda20setCurrentC
-  0x00004da0 55444153 74726561 6d454e53 305f3130 UDAStreamENS0_10
-  0x00004db0 43554441 53747265 616d4500 5f5a5449 CUDAStreamE._ZTI
-  0x00004dc0 4e336331 30323069 6e747275 73697665 N3c1020intrusive
-  0x00004dd0 5f707472 5f746172 67657445 005f5a4e _ptr_targetE._ZN
-  0x00004de0 4b336331 30354572 726f7232 32776861 K3c105Error22wha
-  0x00004df0 745f7769 74686f75 745f6261 636b7472 t_without_backtr
-  0x00004e00 61636545 76005f5a 5449464e 32617436 aceEv._ZTIFN2at6
-  0x00004e10 54656e73 6f724552 4b53305f 53325f64 TensorERKS0_S2_d
-  0x00004e20 45005f5a 4e537431 3372756e 74696d65 E._ZNSt13runtime
-  0x00004e30 5f657272 6f724432 45764047 4c494243 _errorD2Ev@GLIBC
-  0x00004e40 58585f33 2e34005f 5a537431 316d616b XX_3.4._ZSt11mak
-  0x00004e50 655f756e 69717565 494e3574 6f726368 e_uniqueIN5torch
-  0x00004e60 38617574 6f677261 64313241 75746f67 8autograd12Autog
-  0x00004e70 7261644d 65746145 4a504e33 63313031 radMetaEJPN3c101
-  0x00004e80 3054656e 736f7249 6d706c45 52624545 0TensorImplERbEE
-  0x00004e90 4e537439 5f4d616b 65556e69 7149545f NSt9_MakeUniqIT_
-  0x00004ea0 4531355f 5f73696e 676c655f 6f626a65 E15__single_obje
-  0x00004eb0 63744544 704f5430 5f005f5a 54564e31 ctEDpOT0_._ZTVN1
-  0x00004ec0 305f5f63 78786162 69763132 305f5f66 0__cxxabiv120__f
-  0x00004ed0 756e6374 696f6e5f 74797065 5f696e66 unction_type_inf
-  0x00004ee0 6f454043 58584142 495f312e 33005f5a oE@CXXABI_1.3._Z
-  0x00004ef0 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
-  0x00004f00 706c3773 796d5f6e 6f744576 005f5a4e pl7sym_notEv._ZN
-  0x00004f10 32617434 5f6f7073 39746f5f 64657669 2at4_ops9to_devi
-  0x00004f20 63653463 616c6c45 524b4e53 5f365465 ce4callERKNS_6Te
-  0x00004f30 6e736f72 454e3363 31303644 65766963 nsorEN3c106Devic
-  0x00004f40 65454e53 355f3130 5363616c 61725479 eENS5_10ScalarTy
-  0x00004f50 70654562 62537438 6f707469 6f6e616c peEbbSt8optional
-  0x00004f60 494e5335 5f31324d 656d6f72 79466f72 INS5_12MemoryFor
-  0x00004f70 6d617445 45005f5a 54534e33 63313031 matEE._ZTSN3c101
-  0x00004f80 35566172 6961626c 65566572 73696f6e 5VariableVersion
-  0x00004f90 31345665 7273696f 6e436f75 6e746572 14VersionCounter
-  0x00004fa0 45005079 42797465 735f4173 53747269 E.PyBytes_AsStri
-  0x00004fb0 6e67005f 5a4e5374 31335f42 76656374 ng._ZNSt13_Bvect
-  0x00004fc0 6f725f62 61736549 53614962 45453133 or_baseISaIbEE13
-  0x00004fd0 5f4d5f64 65616c6c 6f636174 65457600 _M_deallocateEv.
-  0x00004fe0 5f5a4e53 7331325f 4d5f6c65 616b5f68 _ZNSs12_M_leak_h
-  0x00004ff0 61726445 7640474c 49424358 585f332e ardEv@GLIBCXX_3.
-  0x00005000 34005f5a 5449464e 32617436 54656e73 4._ZTIFN2at6Tens
-  0x00005010 6f724553 305f5330 5f45005f 5a4e3363 orES0_S0_E._ZN3c
-  0x00005020 31303131 53796d4e 6f646549 6d706c37 1011SymNodeImpl7
-  0x00005030 73796d5f 69746545 524b4e53 5f313369 sym_iteERKNS_13i
-  0x00005040 6e747275 73697665 5f707472 4953305f ntrusive_ptrIS0_
-  0x00005050 4e535f36 64657461 696c3334 696e7472 NS_6detail34intr
-  0x00005060 75736976 655f7461 72676574 5f646566 usive_target_def
-  0x00005070 61756c74 5f6e756c 6c5f7479 70654953 ault_null_typeIS
-  0x00005080 305f4545 45455337 5f005f5a 4e336331 0_EEEES7_._ZN3c1
-  0x00005090 30366465 7461696c 3233746f 72636849 06detail23torchI
-  0x000050a0 6e746572 6e616c41 73736572 74466169 nternalAssertFai
-  0x000050b0 6c45504b 6353325f 6a53325f 53325f00 lEPKcS2_jS2_S2_.
-  0x000050c0 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x000050d0 496d706c 3869735f 666c6f61 74457600 Impl8is_floatEv.
-  0x000050e0 5f5a3137 5155414e 545f4745 4d4d5f4b _Z17QUANT_GEMM_K
-  0x000050f0 65726e65 6c493132 54696c69 6e67436f ernelI12TilingCo
-  0x00005100 6e666967 494c6934 454c6931 454c6931 nfigILi4ELi1ELi1
-  0x00005110 4545365f 5f68616c 66457650 4b357569 EE6__halfEvPK5ui
-  0x00005120 6e743450 4b53325f 53375f50 54305f6d nt4PKS2_S7_PT0_m
-  0x00005130 6d6d6900 5f5a4e53 6f395f4d 5f696e73 mmi._ZNSo9_M_ins
-  0x00005140 65727449 6d454552 536f545f 40474c49 ertImEERSoT_@GLI
-  0x00005150 42435858 5f332e34 2e39005f 5a537431 BCXX_3.4.9._ZSt1
-  0x00005160 315f4861 73685f62 79746573 504b766d 1_Hash_bytesPKvm
-  0x00005170 6d404358 58414249 5f312e33 2e35005f m@CXXABI_1.3.5._
-  0x00005180 5a4e4b53 73357266 696e6445 504b636d ZNKSs5rfindEPKcm
-  0x00005190 6d40474c 49424358 585f332e 34005f5a m@GLIBCXX_3.4._Z
-  0x000051a0 4e4b5373 31376669 6e645f66 69727374 NKSs17find_first
-  0x000051b0 5f6e6f74 5f6f6645 504b636d 6d40474c _not_ofEPKcmm@GL
-  0x000051c0 49424358 585f332e 34005079 42797465 IBCXX_3.4.PyByte
-  0x000051d0 41727261 795f5369 7a65005f 5a4e3261 Array_Size._ZN2a
-  0x000051e0 7438696e 64657869 6e673131 54656e73 t8indexing11Tens
-  0x000051f0 6f72496e 64657844 31457600 5f5a646c orIndexD1Ev._Zdl
-  0x00005200 50764047 4c494243 58585f33 2e34005f Pv@GLIBCXX_3.4._
-  0x00005210 5a4e4b33 63313034 63756461 34696d70 ZNK3c104cuda4imp
-  0x00005220 6c313343 55444147 75617264 496d706c l13CUDAGuardImpl
-  0x00005230 32336765 74537472 65616d46 726f6d47 23getStreamFromG
-  0x00005240 6c6f6261 6c506f6f 6c454e53 5f364465 lobalPoolENS_6De
-  0x00005250 76696365 4562005f 5a4e4b33 63313034 viceEb._ZNK3c104
-  0x00005260 696d706c 31365669 72747561 6c477561 impl16VirtualGua
-  0x00005270 7264496d 706c3132 6765744e 65775374 rdImpl12getNewSt
-  0x00005280 7265616d 454e535f 36446576 69636545 reamENS_6DeviceE
-  0x00005290 69005f5a 4e537343 3145504b 636d524b i._ZNSsC1EPKcmRK
-  0x000052a0 53614963 4540474c 49424358 585f332e SaIcE@GLIBCXX_3.
-  0x000052b0 34005f5a 4e336331 30313153 796d4e6f 4._ZN3c1011SymNo
-  0x000052c0 6465496d 706c3132 6d617962 655f6173 deImpl12maybe_as
-  0x000052d0 5f696e74 4576005f 5a4e3363 31303134 _intEv._ZN3c1014
-  0x000052e0 4f706572 61746f72 4b65726e 656c4430 OperatorKernelD0
-  0x000052f0 45760050 79436170 73756c65 5f476574 Ev.PyCapsule_Get
-  0x00005300 436f6e74 65787400 5f5a4e4b 32617431 Context._ZNK2at1
-  0x00005310 3054656e 736f7242 61736532 315f5f64 0TensorBase21__d
-  0x00005320 69737061 7463685f 636f6e74 6967756f ispatch_contiguo
-  0x00005330 7573454e 33633130 31324d65 6d6f7279 usEN3c1012Memory
-  0x00005340 466f726d 61744500 5f5a4e33 63313031 FormatE._ZN3c101
-  0x00005350 3153796d 4e6f6465 496d706c 35626f6f 1SymNodeImpl5boo
-  0x00005360 6c5f4576 005f5a4e 4b336331 3034696d l_Ev._ZNK3c104im
-  0x00005370 706c3136 56697274 75616c47 75617264 pl16VirtualGuard
-  0x00005380 496d706c 31377379 6e636872 6f6e697a Impl17synchroniz
-  0x00005390 65537472 65616d45 524b4e53 5f365374 eStreamERKNS_6St
-  0x000053a0 7265616d 45005f5a 4e326174 345f6f70 reamE._ZN2at4_op
-  0x000053b0 73313965 6d707479 5f6d656d 6f72795f s19empty_memory_
-  0x000053c0 666f726d 61743463 616c6c45 4e336331 format4callEN3c1
-  0x000053d0 30384172 72617952 6566494e 53325f36 08ArrayRefINS2_6
-  0x000053e0 53796d49 6e744545 45537438 6f707469 SymIntEEESt8opti
-  0x000053f0 6f6e616c 494e5332 5f313053 63616c61 onalINS2_10Scala
-  0x00005400 72547970 65454553 365f494e 53325f36 rTypeEES6_INS2_6
-  0x00005410 4c61796f 75744545 53365f49 4e53325f LayoutEES6_INS2_
-  0x00005420 36446576 69636545 4553365f 49624553 6DeviceEES6_IbES
-  0x00005430 365f494e 53325f31 324d656d 6f727946 6_INS2_12MemoryF
-  0x00005440 6f726d61 74454500 5f5a4e33 63313031 ormatEE._ZN3c101
-  0x00005450 3153796d 4e6f6465 496d706c 35636c6f 1SymNodeImpl5clo
-  0x00005460 6e654576 005f5a54 494e3363 31303134 neEv._ZTIN3c1014
-  0x00005470 4f706572 61746f72 4b65726e 656c4500 OperatorKernelE.
-  0x00005480 5f5a4e53 73366170 70656e64 45504b63 _ZNSs6appendEPKc
-  0x00005490 6d40474c 49424358 585f332e 34005f5a m@GLIBCXX_3.4._Z
-  0x000054a0 4e336331 30323069 6e747275 73697665 N3c1020intrusive
-  0x000054b0 5f707472 5f746172 67657444 30457600 _ptr_targetD0Ev.
-  0x000054c0 5f5a4e53 73347377 61704552 53734047 _ZNSs4swapERSs@G
-  0x000054d0 4c494243 58585f33 2e34005f 5a54564e LIBCXX_3.4._ZTVN
-  0x000054e0 33633130 31355661 72696162 6c655665 3c1015VariableVe
-  0x000054f0 7273696f 6e313456 65727369 6f6e436f rsion14VersionCo
-  0x00005500 756e7465 7245005f 50795479 70655f4c unterE._PyType_L
-  0x00005510 6f6f6b75 70005079 54687265 61645374 ookup.PyThreadSt
-  0x00005520 6174655f 436c6561 72005079 4572725f ate_Clear.PyErr_
-  0x00005530 436c6561 72005f5a 4e537436 76656374 Clear._ZNSt6vect
-  0x00005540 6f724962 53614962 45453134 5f4d5f66 orIbSaIbEE14_M_f
-  0x00005550 696c6c5f 696e7365 72744553 7431335f ill_insertESt13_
-  0x00005560 4269745f 69746572 61746f72 6d62005f Bit_iteratormb._
-  0x00005570 5f637861 5f746872 6f774043 58584142 _cxa_throw@CXXAB
-  0x00005580 495f312e 33006375 64615374 7265616d I_1.3.cudaStream
-  0x00005590 53796e63 68726f6e 697a6540 6c696263 Synchronize@libc
-  0x000055a0 75646172 742e736f 2e313200 5f5a5453 udart.so.12._ZTS
-  0x000055b0 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
-  0x000055c0 305f5332 5f644500 50794361 7073756c 0_S2_dE.PyCapsul
-  0x000055d0 655f4e65 77005079 4d656d5f 43616c6c e_New.PyMem_Call
-  0x000055e0 6f63005f 5a4e3363 31303469 6d706c36 oc._ZN3c104impl6
-  0x000055f0 64657461 696c3331 57726170 46756e63 detail31WrapFunc
-  0x00005600 74696f6e 496e746f 52756e74 696d6546 tionIntoRuntimeF
-  0x00005610 756e6374 6f725f49 50464e32 61743654 unctor_IPFN2at6T
-  0x00005620 656e736f 72455334 5f53345f 4553345f ensorES4_S4_ES4_
-  0x00005630 4e535f34 67757473 38747970 656c6973 NS_4guts8typelis
-  0x00005640 74387479 70656c69 7374494a 53345f53 t8typelistIJS4_S
-  0x00005650 345f4545 45454431 4576005f 5a4e3363 4_EEEED1Ev._ZN3c
-  0x00005660 31303664 65746169 6c31325f 7374725f 106detail12_str_
-  0x00005670 77726170 70657249 4a504b63 524b6c45 wrapperIJPKcRKlE
-  0x00005680 45346361 6c6c4552 4b53335f 53355f00 E4callERKS3_S5_.
-  0x00005690 5f5a4e32 6174345f 6f707331 31736f72 _ZN2at4_ops11sor
-  0x000056a0 745f7374 61626c65 3463616c 6c45524b t_stable4callERK
-  0x000056b0 4e535f36 54656e73 6f724553 74386f70 NS_6TensorESt8op
-  0x000056c0 74696f6e 616c4962 456c6200 5f5a5374 tionalIbElb._ZSt
-  0x000056d0 32305f5f 7468726f 775f6c65 6e677468 20__throw_length
-  0x000056e0 5f657272 6f72504b 6340474c 49424358 _errorPKc@GLIBCX
-  0x000056f0 585f332e 34005f5a 4e35746f 72636837 X_3.4._ZN5torch7
-  0x00005700 4c696272 61727943 31454e53 305f344b LibraryC1ENS0_4K
-  0x00005710 696e6445 53735374 386f7074 696f6e61 indESsSt8optiona
-  0x00005720 6c494e33 63313031 31446973 70617463 lIN3c1011Dispatc
-  0x00005730 684b6579 4545504b 636a005f 556e7769 hKeyEEPKcj._Unwi
-  0x00005740 6e645f52 6573756d 65404743 435f332e nd_Resume@GCC_3.
-  0x00005750 30005f5a 4e4b3363 31303463 75646134 0._ZNK3c104cuda4
-  0x00005760 696d706c 31334355 44414775 61726449 impl13CUDAGuardI
-  0x00005770 6d706c31 31717565 72795374 7265616d mpl11queryStream
-  0x00005780 45524b4e 535f3653 74726561 6d450050 ERKNS_6StreamE.P
-  0x00005790 79427974 65735f53 697a6500 5f5a5453 yBytes_Size._ZTS
-  0x000057a0 4e336331 3034696d 706c3664 65746169 N3c104impl6detai
-  0x000057b0 6c333157 72617046 756e6374 696f6e49 l31WrapFunctionI
-  0x000057c0 6e746f52 756e7469 6d654675 6e63746f ntoRuntimeFuncto
-  0x000057d0 725f4950 464e3261 74365465 6e736f72 r_IPFN2at6Tensor
-  0x000057e0 4553345f 53345f45 53345f4e 535f3467 ES4_S4_ES4_NS_4g
-  0x000057f0 75747338 74797065 6c697374 38747970 uts8typelist8typ
-  0x00005800 656c6973 74494a53 345f5334 5f454545 elistIJS4_S4_EEE
-  0x00005810 4545005f 5a4e3363 31303131 53796d4e EE._ZN3c1011SymN
-  0x00005820 6f646549 6d706c31 366e6573 7465645f odeImpl16nested_
-  0x00005830 696e745f 636f6566 66457600 5f5a4e4b int_coeffEv._ZNK
-  0x00005840 33633130 34637564 6134696d 706c3133 3c104cuda4impl13
-  0x00005850 43554441 47756172 64496d70 6c313673 CUDAGuardImpl16s
-  0x00005860 796e6368 726f6e69 7a654576 656e7445 ynchronizeEventE
-  0x00005870 5076005f 5a4e3363 31303463 75646131 Pv._ZN3c104cuda1
-  0x00005880 32646576 6963655f 636f756e 74457600 2device_countEv.
-  0x00005890 5f5a4e4b 33633130 34637564 6134696d _ZNK3c104cuda4im
-  0x000058a0 706c3133 43554441 47756172 64496d70 pl13CUDAGuardImp
-  0x000058b0 6c396765 74446576 69636545 76005f5a l9getDeviceEv._Z
-  0x000058c0 32304269 74496e74 65726c65 6176696e 20BitInterleavin
-  0x000058d0 675f3262 69745068 005f5a4e 37746f72 g_2bitPh._ZN7tor
-  0x000058e0 6368616f 32357765 69676874 5f6d6174 chao25weight_mat
-  0x000058f0 7269785f 64657175 616e745f 63707545 rix_dequant_cpuE
-  0x00005900 4e326174 3654656e 736f7245 53315f00 N2at6TensorES1_.
-  0x00005910 76736e70 72696e74 6640474c 4942435f vsnprintf@GLIBC_
-  0x00005920 322e322e 35005f5a 4e336331 3034696d 2.2.5._ZN3c104im
-  0x00005930 706c3238 77726170 5f6b6572 6e656c5f pl28wrap_kernel_
-  0x00005940 66756e63 746f725f 756e626f 7865645f functor_unboxed_
-  0x00005950 494e5330 5f366465 7461696c 33315772 INS0_6detail31Wr
-  0x00005960 61704675 6e637469 6f6e496e 746f5275 apFunctionIntoRu
-  0x00005970 6e74696d 6546756e 63746f72 5f495046 ntimeFunctor_IPF
-  0x00005980 4e326174 3654656e 736f7245 53355f45 N2at6TensorES5_E
-  0x00005990 53355f4e 535f3467 75747338 74797065 S5_NS_4guts8type
-  0x000059a0 6c697374 38747970 656c6973 74494a53 list8typelistIJS
-  0x000059b0 355f4545 45454553 365f4534 63616c6c 5_EEEEES6_E4call
-  0x000059c0 45504e53 5f31344f 70657261 746f724b EPNS_14OperatorK
-  0x000059d0 65726e65 6c454e53 5f313444 69737061 ernelENS_14Dispa
-  0x000059e0 7463684b 65795365 74455335 5f005f5a tchKeySetES5_._Z
-  0x000059f0 4e336331 30313556 61726961 626c6556 N3c1015VariableV
-  0x00005a00 65727369 6f6e3134 56657273 696f6e43 ersion14VersionC
-  0x00005a10 6f756e74 65724430 4576005f 5a4e3363 ounterD0Ev._ZN3c
-  0x00005a20 31303131 53796d4e 6f646549 6d706c37 1011SymNodeImpl7
-  0x00005a30 73796d5f 6d617845 524b4e53 5f313369 sym_maxERKNS_13i
-  0x00005a40 6e747275 73697665 5f707472 4953305f ntrusive_ptrIS0_
-  0x00005a50 4e535f36 64657461 696c3334 696e7472 NS_6detail34intr
-  0x00005a60 75736976 655f7461 72676574 5f646566 usive_target_def
-  0x00005a70 61756c74 5f6e756c 6c5f7479 70654953 ault_null_typeIS
-  0x00005a80 305f4545 4545005f 5a544946 4e326174 0_EEEE._ZTIFN2at
-  0x00005a90 3654656e 736f7245 53305f53 305f5330 6TensorES0_S0_S0
-  0x00005aa0 5f6c4500 50794578 635f5479 70654572 _lE.PyExc_TypeEr
-  0x00005ab0 726f7200 5f5a4e33 63313031 3153796d ror._ZN3c1011Sym
-  0x00005ac0 4e6f6465 496d706c 35666c6f 6f724576 NodeImpl5floorEv
-  0x00005ad0 005f5a54 494e3363 31303463 75646134 ._ZTIN3c104cuda4
-  0x00005ae0 696d706c 31334355 44414775 61726449 impl13CUDAGuardI
-  0x00005af0 6d706c45 005f5a4e 4b336331 3034696d mplE._ZNK3c104im
-  0x00005b00 706c3136 56697274 75616c47 75617264 pl16VirtualGuard
-  0x00005b10 496d706c 3138756e 63686563 6b656453 Impl18uncheckedS
-  0x00005b20 65744465 76696365 454e535f 36446576 etDeviceENS_6Dev
-  0x00005b30 69636545 005f5a4e 4b336331 30346375 iceE._ZNK3c104cu
-  0x00005b40 64613469 6d706c31 33435544 41477561 da4impl13CUDAGua
-  0x00005b50 7264496d 706c3973 65744465 76696365 rdImpl9setDevice
-  0x00005b60 454e535f 36446576 69636545 005f5a54 ENS_6DeviceE._ZT
-  0x00005b70 564e3363 31303131 53796d4e 6f646549 VN3c1011SymNodeI
-  0x00005b80 6d706c45 005f5a54 494e3363 31303130 mplE._ZTIN3c1010
-  0x00005b90 56616c75 65457272 6f724500 5f5a5456 ValueErrorE._ZTV
-  0x00005ba0 4e336331 3034696d 706c3664 65746169 N3c104impl6detai
-  0x00005bb0 6c333157 72617046 756e6374 696f6e49 l31WrapFunctionI
-  0x00005bc0 6e746f52 756e7469 6d654675 6e63746f ntoRuntimeFuncto
-  0x00005bd0 725f4950 464e3261 74365465 6e736f72 r_IPFN2at6Tensor
-  0x00005be0 4553345f 4553345f 4e535f34 67757473 ES4_ES4_NS_4guts
-  0x00005bf0 38747970 656c6973 74387479 70656c69 8typelist8typeli
-  0x00005c00 7374494a 53345f45 45454545 00507954 stIJS4_EEEEE.PyT
-  0x00005c10 7970655f 52656164 79005f5a 54495374 ype_Ready._ZTISt
-  0x00005c20 31396261 645f6f70 74696f6e 616c5f61 19bad_optional_a
-  0x00005c30 63636573 73005f5a 54534e33 63313034 ccess._ZTSN3c104
-  0x00005c40 696d706c 36646574 61696c33 31577261 impl6detail31Wra
-  0x00005c50 7046756e 6374696f 6e496e74 6f52756e pFunctionIntoRun
-  0x00005c60 74696d65 46756e63 746f725f 4950464e timeFunctor_IPFN
-  0x00005c70 32617436 54656e73 6f724553 345f4553 2at6TensorES4_ES
-  0x00005c80 345f4e53 5f346775 74733874 7970656c 4_NS_4guts8typel
-  0x00005c90 69737438 74797065 6c697374 494a5334 ist8typelistIJS4
-  0x00005ca0 5f454545 4545005f 5a4e3363 31303131 _EEEEE._ZN3c1011
-  0x00005cb0 53796d4e 6f646549 6d706c32 67654552 SymNodeImpl2geER
-  0x00005cc0 4b4e535f 3133696e 74727573 6976655f KNS_13intrusive_
-  0x00005cd0 70747249 53305f4e 535f3664 65746169 ptrIS0_NS_6detai
-  0x00005ce0 6c333469 6e747275 73697665 5f746172 l34intrusive_tar
-  0x00005cf0 6765745f 64656661 756c745f 6e756c6c get_default_null
-  0x00005d00 5f747970 65495330 5f454545 45005f5a _typeIS0_EEEE._Z
-  0x00005d10 4e336331 30354572 726f7243 32454e53 N3c105ErrorC2ENS
-  0x00005d20 5f313453 6f757263 654c6f63 6174696f _14SourceLocatio
-  0x00005d30 6e455373 005f5a54 494e3363 31303131 nESs._ZTIN3c1011
-  0x00005d40 53796d4e 6f646549 6d706c45 005f5a53 SymNodeImplE._ZS
-  0x00005d50 7432345f 5f746872 6f775f6f 75745f6f t24__throw_out_o
-  0x00005d60 665f7261 6e67655f 666d7450 4b637a00 f_range_fmtPKcz.
-  0x00005d70 5f5a3137 5155414e 545f4745 4d4d5f4b _Z17QUANT_GEMM_K
-  0x00005d80 65726e65 6c493132 54696c69 6e67436f ernelI12TilingCo
-  0x00005d90 6e666967 494c6934 454c6931 454c6931 nfigILi4ELi1ELi1
-  0x00005da0 45456645 76504b35 75696e74 34504b36 EEfEvPK5uint4PK6
-  0x00005db0 5f5f6861 6c665337 5f505430 5f6d6d6d __halfS7_PT0_mmm
-  0x00005dc0 69005f5a 4e336331 3034696d 706c3664 i._ZN3c104impl6d
-  0x00005dd0 65746169 6c333157 72617046 756e6374 etail31WrapFunct
-  0x00005de0 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
-  0x00005df0 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
-  0x00005e00 6e736f72 4553345f 53345f53 345f6c45 nsorES4_S4_S4_lE
-  0x00005e10 53345f4e 535f3467 75747338 74797065 S4_NS_4guts8type
-  0x00005e20 6c697374 38747970 656c6973 74494a53 list8typelistIJS
-  0x00005e30 345f5334 5f53345f 6c454545 45443045 4_S4_S4_lEEEED0E
-  0x00005e40 76005f5a 4e336331 30313153 796d4e6f v._ZN3c1011SymNo
-  0x00005e50 6465496d 706c3133 69735f63 6f6e7469 deImpl13is_conti
-  0x00005e60 67756f75 73454e53 5f384172 72617952 guousENS_8ArrayR
-  0x00005e70 6566494e 535f3133 696e7472 75736976 efINS_13intrusiv
-  0x00005e80 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
-  0x00005e90 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
-  0x00005ea0 61726765 745f6465 6661756c 745f6e75 arget_default_nu
-  0x00005eb0 6c6c5f74 79706549 53305f45 45454545 ll_typeIS0_EEEEE
-  0x00005ec0 4553375f 005f5a4e 33633130 31315379 ES7_._ZN3c1011Sy
-  0x00005ed0 6d4e6f64 65496d70 6c443045 76005f5a mNodeImplD0Ev._Z
-  0x00005ee0 4e537336 61737369 676e4552 4b537340 NSs6assignERKSs@
-  0x00005ef0 474c4942 4358585f 332e3400 5f5a4e53 GLIBCXX_3.4._ZNS
-  0x00005f00 73366173 7369676e 45504b63 6d40474c s6assignEPKcm@GL
-  0x00005f10 49424358 585f332e 34005f5a 4e336331 IBCXX_3.4._ZN3c1
-  0x00005f20 30313153 796d4e6f 6465496d 706c3673 011SymNodeImpl6s
-  0x00005f30 796d5f6f 7245524b 4e535f31 33696e74 ym_orERKNS_13int
-  0x00005f40 72757369 76655f70 74724953 305f4e53 rusive_ptrIS0_NS
-  0x00005f50 5f366465 7461696c 3334696e 74727573 _6detail34intrus
-  0x00005f60 6976655f 74617267 65745f64 65666175 ive_target_defau
-  0x00005f70 6c745f6e 756c6c5f 74797065 4953305f lt_null_typeIS0_
-  0x00005f80 45454545 005f5a4e 33633130 31315379 EEEE._ZN3c1011Sy
-  0x00005f90 6d4e6f64 65496d70 6c33706f 7745524b mNodeImpl3powERK
-  0x00005fa0 4e535f31 33696e74 72757369 76655f70 NS_13intrusive_p
-  0x00005fb0 74724953 305f4e53 5f366465 7461696c trIS0_NS_6detail
-  0x00005fc0 3334696e 74727573 6976655f 74617267 34intrusive_targ
-  0x00005fd0 65745f64 65666175 6c745f6e 756c6c5f et_default_null_
-  0x00005fe0 74797065 4953305f 45454545 005f5a4e typeIS0_EEEE._ZN
-  0x00005ff0 33633130 36646574 61696c32 33746f72 3c106detail23tor
-  0x00006000 6368496e 7465726e 616c4173 73657274 chInternalAssert
-  0x00006010 4661696c 45504b63 53325f6a 53325f52 FailEPKcS2_jS2_R
-  0x00006020 4b537300 5079496e 69745f5f 43005f5a KSs.PyInit__C._Z
-  0x00006030 4e537336 61707065 6e644552 4b537340 NSs6appendERKSs@
-  0x00006040 474c4942 4358585f 332e3400 5f5a5453 GLIBCXX_3.4._ZTS
-  0x00006050 464e3261 74365465 6e736f72 4553305f FN2at6TensorES0_
-  0x00006060 53305f45 00507954 75706c65 5f476574 S0_E.PyTuple_Get
-  0x00006070 4974656d 005f5a4e 53743135 5f5f6578 Item._ZNSt15__ex
-  0x00006080 63657074 696f6e5f 7074726e 6545524b ception_ptrneERK
-  0x00006090 4e535f31 33657863 65707469 6f6e5f70 NS_13exception_p
-  0x000060a0 74724553 325f4043 58584142 495f312e trES2_@CXXABI_1.
-  0x000060b0 332e3300 5f5a4e37 746f7263 68616f32 3.3._ZN7torchao2
-  0x000060c0 38776569 6768745f 6d617472 69785f70 8weight_matrix_p
-  0x000060d0 72657061 636b696e 675f6370 75454e32 repacking_cpuEN2
-  0x000060e0 61743654 656e736f 7245005f 50794f62 at6TensorE._PyOb
-  0x000060f0 6a656374 5f476574 44696374 50747200 ject_GetDictPtr.
-  0x00006100 5f5a4e4b 32617436 54656e73 6f723569 _ZNK2at6Tensor5i
-  0x00006110 6e646578 45537431 36696e69 7469616c ndexESt16initial
-  0x00006120 697a6572 5f6c6973 74494e53 5f38696e izer_listINS_8in
-  0x00006130 64657869 6e673131 54656e73 6f72496e dexing11TensorIn
-  0x00006140 64657845 45005f5f 6378615f 61746578 dexEE.__cxa_atex
-  0x00006150 69744047 4c494243 5f322e32 2e35005f it@GLIBC_2.2.5._
-  0x00006160 5a54564e 33633130 31344f70 65726174 ZTVN3c1014Operat
-  0x00006170 6f724b65 726e656c 45005f5a 4e4b3261 orKernelE._ZNK2a
-  0x00006180 74313054 656e736f 72426173 65386461 t10TensorBase8da
-  0x00006190 74615f70 7472496c 45455054 5f760050 ta_ptrIlEEPT_v.P
-  0x000061a0 79547570 6c655f53 65744974 656d005f yTuple_SetItem._
-  0x000061b0 5a313751 55414e54 5f47454d 4d5f4b65 Z17QUANT_GEMM_Ke
-  0x000061c0 726e656c 49313254 696c696e 67436f6e rnelI12TilingCon
-  0x000061d0 66696749 4c693445 4c693145 4c693845 figILi4ELi1ELi8E
-  0x000061e0 45664576 504b3575 696e7434 504b365f EfEvPK5uint4PK6_
-  0x000061f0 5f68616c 6653375f 5054305f 6d6d6d69 _halfS7_PT0_mmmi
-  0x00006200 00507954 68726561 645f7473 735f6765 .PyThread_tss_ge
-  0x00006210 74005079 4572725f 52657374 6f726500 t.PyErr_Restore.
-  0x00006220 5f5a3239 77656967 68745f70 72657061 _Z29weight_prepa
-  0x00006230 636b696e 675f6670 31365f74 6f5f6670 cking_fp16_to_fp
-  0x00006240 36507450 686d6d00 5f5a4e35 746f7263 6PtPhmm._ZN5torc
-  0x00006250 6835656d 70747945 4e336331 30384172 h5emptyEN3c108Ar
-  0x00006260 72617952 6566496c 45454e53 305f3133 rayRefIlEENS0_13
-  0x00006270 54656e73 6f724f70 74696f6e 73455374 TensorOptionsESt
-  0x00006280 386f7074 696f6e61 6c494e53 305f3132 8optionalINS0_12
-  0x00006290 4d656d6f 7279466f 726d6174 4545005f MemoryFormatEE._
-  0x000062a0 5a4e3574 6f726368 374c6962 72617279 ZN5torch7Library
-  0x000062b0 44314576 005f5a4e 33633130 34637564 D1Ev._ZN3c104cud
-  0x000062c0 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
-  0x000062d0 64496d70 6c443145 76005f5f 6378615f dImplD1Ev.__cxa_
-  0x000062e0 70757265 5f766972 7475616c 40435858 pure_virtual@CXX
-  0x000062f0 4142495f 312e3300 5f5f7074 68726561 ABI_1.3.__pthrea
-  0x00006300 645f6b65 795f6372 65617465 40474c49 d_key_create@GLI
-  0x00006310 42435f32 2e322e35 005f5a4e 53743135 BC_2.2.5._ZNSt15
-  0x00006320 5f5f6578 63657074 696f6e5f 70747231 __exception_ptr1
-  0x00006330 33657863 65707469 6f6e5f70 74723473 3exception_ptr4s
-  0x00006340 77617045 5253305f 40435858 4142495f wapERS0_@CXXABI_
-  0x00006350 312e332e 33005f5a 4e336331 30313153 1.3.3._ZN3c1011S
-  0x00006360 796d4e6f 6465496d 706c3130 77726170 ymNodeImpl10wrap
-  0x00006370 5f666c6f 61744564 005f5a4e 4b336331 _floatEd._ZNK3c1
-  0x00006380 30346375 64613469 6d706c31 33435544 04cuda4impl13CUD
-  0x00006390 41477561 7264496d 706c3672 65636f72 AGuardImpl6recor
-  0x000063a0 64455050 76524b4e 535f3653 74726561 dEPPvRKNS_6Strea
-  0x000063b0 6d45614e 535f3945 76656e74 466c6167 mEaNS_9EventFlag
-  0x000063c0 45005f5a 4e523574 6f726368 374c6962 E._ZNR5torch7Lib
-  0x000063d0 72617279 355f696d 706c4550 4b634f4e rary5_implEPKcON
-  0x000063e0 535f3131 43707046 756e6374 696f6e45 S_11CppFunctionE
-  0x000063f0 4e535f31 375f5265 67697374 65724f72 NS_17_RegisterOr
-  0x00006400 56657269 66794500 5f5a5374 706c4963 VerifyE._ZStplIc
-  0x00006410 53743131 63686172 5f747261 69747349 St11char_traitsI
-  0x00006420 63455361 49634545 53624954 5f54305f cESaIcEESbIT_T0_
-  0x00006430 54315f45 504b5333 5f524b53 365f005f T1_EPKS3_RKS6_._
-  0x00006440 5a4e5373 43314552 4b536149 63454047 ZNSsC1ERKSaIcE@G
-  0x00006450 4c494243 58585f33 2e34005f 5a4e3363 LIBCXX_3.4._ZN3c
-  0x00006460 31303463 75646139 47657444 65766963 104cuda9GetDevic
-  0x00006470 65455061 005f5a4e 33633130 31346765 eEPa._ZN3c1014ge
-  0x00006480 74547970 65507472 436f7079 494e3261 tTypePtrCopyIN2a
-  0x00006490 74365465 6e736f72 4545454e 535f3454 t6TensorEEENS_4T
-  0x000064a0 79706532 3453696e 676c6574 6f6e4f72 ype24SingletonOr
-  0x000064b0 53686172 65645479 70655074 72495333 SharedTypePtrIS3
-  0x000064c0 5f454576 005f5a4e 5373345f 52657031 _EEv._ZNSs4_Rep1
-  0x000064d0 305f4d5f 64657374 726f7945 524b5361 0_M_destroyERKSa
-  0x000064e0 49634540 474c4942 4358585f 332e3400 IcE@GLIBCXX_3.4.
-  0x000064f0 5f5a4e53 7431355f 5f657863 65707469 _ZNSt15__excepti
-  0x00006500 6f6e5f70 74723133 65786365 7074696f on_ptr13exceptio
-  0x00006510 6e5f7074 72443145 76404358 58414249 n_ptrD1Ev@CXXABI
-  0x00006520 5f312e33 2e33005f 5a4e3261 74345f6f _1.3.3._ZN2at4_o
-  0x00006530 70733132 696e6465 785f7365 6c656374 ps12index_select
-  0x00006540 3463616c 6c45524b 4e535f36 54656e73 4callERKNS_6Tens
-  0x00006550 6f72456c 53345f00 50795468 72656164 orElS4_.PyThread
-  0x00006560 5f747373 5f616c6c 6f63005f 5a544953 _tss_alloc._ZTIS
-  0x00006570 7431366e 65737465 645f6578 63657074 t16nested_except
-  0x00006580 696f6e40 43585841 42495f31 2e332e35 ion@CXXABI_1.3.5
-  0x00006590 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
-  0x000065a0 65496d70 6c326c65 45524b4e 535f3133 eImpl2leERKNS_13
-  0x000065b0 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
-  0x000065c0 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
-  0x000065d0 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x000065e0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x000065f0 53305f45 45454500 5f5a4e4b 33633130 S0_EEEE._ZNK3c10
-  0x00006600 34696d70 6c313656 69727475 616c4775 4impl16VirtualGu
-  0x00006610 61726449 6d706c31 34657863 68616e67 ardImpl14exchang
-  0x00006620 65446576 69636545 4e535f36 44657669 eDeviceENS_6Devi
-  0x00006630 63654500 5f5a4e4b 33633130 34696d70 ceE._ZNK3c104imp
-  0x00006640 6c313656 69727475 616c4775 61726449 l16VirtualGuardI
-  0x00006650 6d706c31 36676574 44656661 756c7453 mpl16getDefaultS
-  0x00006660 74726561 6d454e53 5f364465 76696365 treamENS_6Device
-  0x00006670 45005f5a 4e366361 66666532 38547970 E._ZN6caffe28Typ
-  0x00006680 654d6574 61323665 72726f72 5f756e73 eMeta26error_uns
-  0x00006690 7570706f 72746564 5f747970 656d6574 upported_typemet
-  0x000066a0 61455330 5f005f5a 4e336331 30313153 aES0_._ZN3c1011S
-  0x000066b0 796d4e6f 6465496d 706c3769 735f626f ymNodeImpl7is_bo
-  0x000066c0 6f6c4576 005f5a54 49537431 3372756e olEv._ZTISt13run
-  0x000066d0 74696d65 5f657272 6f724047 4c494243 time_error@GLIBC
-  0x000066e0 58585f33 2e34005f 5a4e3363 31303134 XX_3.4._ZN3c1014
-  0x000066f0 4f706572 61746f72 4b65726e 656c4431 OperatorKernelD1
-  0x00006700 45760063 75646147 65744572 726f7253 Ev.cudaGetErrorS
-  0x00006710 7472696e 67406c69 62637564 6172742e tring@libcudart.
-  0x00006720 736f2e31 32005f5a 4e537431 3372756e so.12._ZNSt13run
-  0x00006730 74696d65 5f657272 6f724331 45524b53 time_errorC1ERKS
-  0x00006740 7340474c 49424358 585f332e 34005f5a s@GLIBCXX_3.4._Z
-  0x00006750 4e326174 345f6f70 73366e61 72726f77 N2at4_ops6narrow
-  0x00006760 3463616c 6c45524b 4e535f36 54656e73 4callERKNS_6Tens
-  0x00006770 6f72456c 4e336331 30365379 6d496e74 orElN3c106SymInt
-  0x00006780 4553365f 005f5a4e 33633130 31315379 ES6_._ZN3c1011Sy
-  0x00006790 6d4e6f64 65496d70 6c326e65 45524b4e mNodeImpl2neERKN
-  0x000067a0 535f3133 696e7472 75736976 655f7074 S_13intrusive_pt
-  0x000067b0 72495330 5f4e535f 36646574 61696c33 rIS0_NS_6detail3
-  0x000067c0 34696e74 72757369 76655f74 61726765 4intrusive_targe
-  0x000067d0 745f6465 6661756c 745f6e75 6c6c5f74 t_default_null_t
-  0x000067e0 79706549 53305f45 45454500 5f5a4e35 ypeIS0_EEEE._ZN5
-  0x000067f0 746f7263 68386175 746f6772 61643133 torch8autograd13
-  0x00006800 6d616b65 5f766172 6961626c 65454e32 make_variableEN2
-  0x00006810 61743654 656e736f 72456262 005f5a4e at6TensorEbb._ZN
-  0x00006820 53743135 62617369 635f7374 72696e67 St15basic_string
-  0x00006830 62756649 63537431 31636861 725f7472 bufIcSt11char_tr
-  0x00006840 61697473 49634553 61496345 45443045 aitsIcESaIcEED0E
-  0x00006850 76005f5a 4e336331 30313556 61726961 v._ZN3c1015Varia
-  0x00006860 626c6556 65727369 6f6e3134 56657273 bleVersion14Vers
-  0x00006870 696f6e43 6f756e74 65724431 4576005f ionCounterD1Ev._
-  0x00006880 5a4e3363 31303130 56616c75 65457272 ZN3c1010ValueErr
-  0x00006890 6f724431 4576005f 5a4e3363 31303131 orD1Ev._ZN3c1011
-  0x000068a0 53796d4e 6f646549 6d706c31 31677561 SymNodeImpl11gua
-  0x000068b0 72645f66 6c6f6174 45504b63 6c005f5a rd_floatEPKcl._Z
-  0x000068c0 5374706c 49635374 31316368 61725f74 StplIcSt11char_t
-  0x000068d0 72616974 73496345 53614963 45455362 raitsIcESaIcEESb
-  0x000068e0 49545f54 305f5431 5f454f53 365f5337 IT_T0_T1_EOS6_S7
-  0x000068f0 5f005f5a 54534e33 63313031 3153796d _._ZTSN3c1011Sym
-  0x00006900 4e6f6465 496d706c 45005f5a 53743136 NodeImplE._ZSt16
-  0x00006910 5f5f6f73 74726561 6d5f696e 73657274 __ostream_insert
-  0x00006920 49635374 31316368 61725f74 72616974 IcSt11char_trait
-  0x00006930 73496345 45525374 31336261 7369635f sIcEERSt13basic_
-  0x00006940 6f737472 65616d49 545f5430 5f455336 ostreamIT_T0_ES6
-  0x00006950 5f504b53 335f6c40 474c4942 4358585f _PKS3_l@GLIBCXX_
-  0x00006960 332e342e 39005f49 544d5f72 65676973 3.4.9._ITM_regis
-  0x00006970 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
-  0x00006980 50794346 756e6374 696f6e5f 54797065 PyCFunction_Type
-  0x00006990 005f5a4e 33633130 34696d70 6c366465 ._ZN3c104impl6de
-  0x000069a0 7461696c 33315772 61704675 6e637469 tail31WrapFuncti
-  0x000069b0 6f6e496e 746f5275 6e74696d 6546756e onIntoRuntimeFun
-  0x000069c0 63746f72 5f495046 4e326174 3654656e ctor_IPFN2at6Ten
-  0x000069d0 736f7245 53345f53 345f5334 5f6c4553 sorES4_S4_S4_lES
-  0x000069e0 345f4e53 5f346775 74733874 7970656c 4_NS_4guts8typel
-  0x000069f0 69737438 74797065 6c697374 494a5334 ist8typelistIJS4
-  0x00006a00 5f53345f 53345f6c 45454545 44324576 _S4_S4_lEEEED2Ev
-  0x00006a10 005f5a4e 53734331 45524b53 736d6d40 ._ZNSsC1ERKSsmm@
-  0x00006a20 474c4942 4358585f 332e3400 50794749 GLIBCXX_3.4.PyGI
-  0x00006a30 4c537461 74655f47 65745468 69735468 LState_GetThisTh
-  0x00006a40 72656164 53746174 65005079 42797465 readState.PyByte
-  0x00006a50 735f4173 53747269 6e67416e 6453697a s_AsStringAndSiz
-  0x00006a60 65006d65 6d636d70 40474c49 42435f32 e.memcmp@GLIBC_2
-  0x00006a70 2e322e35 005f5a4e 33633130 3133696e .2.5._ZN3c1013in
-  0x00006a80 74727573 6976655f 70747249 4e535f31 trusive_ptrINS_1
-  0x00006a90 35566172 6961626c 65566572 73696f6e 5VariableVersion
-  0x00006aa0 31345665 7273696f 6e436f75 6e746572 14VersionCounter
-  0x00006ab0 454e535f 36646574 61696c33 34696e74 ENS_6detail34int
-  0x00006ac0 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x00006ad0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x00006ae0 53325f45 45453672 65736574 5f457600 S2_EEE6reset_Ev.
-  0x00006af0 5079556e 69636f64 655f4173 456e636f PyUnicode_AsEnco
-  0x00006b00 64656453 7472696e 67005f5a 4e4b5373 dedString._ZNKSs
-  0x00006b10 37636f6d 70617265 45504b63 40474c49 7compareEPKc@GLI
-  0x00006b20 42435858 5f332e34 005f5a4e 4b326174 BCXX_3.4._ZNK2at
-  0x00006b30 31305465 6e736f72 42617365 38646174 10TensorBase8dat
-  0x00006b40 615f7074 72494e33 63313034 48616c66 a_ptrIN3c104Half
-  0x00006b50 45454550 545f7600 5f5a4e33 63313031 EEEPT_v._ZN3c101
-  0x00006b60 3153796d 4e6f6465 496d706c 44324576 1SymNodeImplD2Ev
-  0x00006b70 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
-  0x00006b80 65496d70 6c386861 735f6869 6e744576 eImpl8has_hintEv
-  0x00006b90 00507954 75706c65 5f4e6577 005f5a31 .PyTuple_New._Z1
-  0x00006ba0 37515541 4e545f47 454d4d5f 4b65726e 7QUANT_GEMM_Kern
-  0x00006bb0 656c4931 3254696c 696e6743 6f6e6669 elI12TilingConfi
-  0x00006bc0 67494c69 34454c69 31454c69 32454536 gILi4ELi1ELi2EE6
-  0x00006bd0 5f5f6861 6c664576 504b3575 696e7434 __halfEvPK5uint4
-  0x00006be0 504b5332 5f53375f 5054305f 6d6d6d69 PKS2_S7_PT0_mmmi
-  0x00006bf0 005f5a4e 35746f72 63683664 65746169 ._ZN5torch6detai
-  0x00006c00 6c313654 6f726368 4c696272 61727949 l16TorchLibraryI
-  0x00006c10 6e697444 31457600 50794f62 6a656374 nitD1Ev.PyObject
-  0x00006c20 5f43616c 6c46756e 6374696f 6e4f626a _CallFunctionObj
-  0x00006c30 41726773 005f5a4e 33633130 34696d70 Args._ZN3c104imp
-  0x00006c40 6c323345 78636c75 64654469 73706174 l23ExcludeDispat
-  0x00006c50 63684b65 79477561 72644331 454e535f chKeyGuardC1ENS_
-  0x00006c60 31344469 73706174 63684b65 79536574 14DispatchKeySet
-  0x00006c70 45005f5a 4e4b3261 74313054 656e736f E._ZNK2at10Tenso
-  0x00006c80 72426173 65386461 74615f70 74724968 rBase8data_ptrIh
-  0x00006c90 45455054 5f76005f 5a4e4b53 74313962 EEPT_v._ZNKSt19b
-  0x00006ca0 61645f6f 7074696f 6e616c5f 61636365 ad_optional_acce
-  0x00006cb0 73733477 68617445 76005f5a 54495374 ss4whatEv._ZTISt
-  0x00006cc0 31365f53 705f636f 756e7465 645f6261 16_Sp_counted_ba
-  0x00006cd0 7365494c 4e395f5f 676e755f 63787831 seILN9__gnu_cxx1
-  0x00006ce0 325f4c6f 636b5f70 6f6c6963 79453245 2_Lock_policyE2E
-  0x00006cf0 45006375 64614576 656e7453 796e6368 E.cudaEventSynch
-  0x00006d00 726f6e69 7a65406c 69626375 64617274 ronize@libcudart
-  0x00006d10 2e736f2e 3132005f 5a4e3363 31303463 .so.12._ZN3c104c
-  0x00006d20 75646132 30676574 44656661 756c7443 uda20getDefaultC
-  0x00006d30 55444153 74726561 6d456100 5f5a3234 UDAStreamEa._Z24
-  0x00006d40 77656967 68745f6d 61747269 785f7072 weight_matrix_pr
-  0x00006d50 65706163 6b696e67 5069535f 6d6d005f epackingPiS_mm._
-  0x00006d60 5a4e4b33 63313031 3054656e 736f7249 ZNK3c1010TensorI
-  0x00006d70 6d706c36 64657669 63654576 005f5a4e mpl6deviceEv._ZN
-  0x00006d80 53743676 6563746f 72496253 61496245 St6vectorIbSaIbE
-  0x00006d90 4531335f 4d5f696e 73657274 5f617578 E13_M_insert_aux
-  0x00006da0 45537431 335f4269 745f6974 65726174 ESt13_Bit_iterat
-  0x00006db0 6f726200 5f5a4e33 6331306c 73455253 orb._ZN3c10lsERS
-  0x00006dc0 6f4e535f 31304465 76696365 54797065 oNS_10DeviceType
-  0x00006dd0 45005f5a 54545374 31396261 7369635f E._ZTTSt19basic_
-  0x00006de0 6f737472 696e6773 74726561 6d496353 ostringstreamIcS
-  0x00006df0 74313163 6861725f 74726169 74734963 t11char_traitsIc
-  0x00006e00 45536149 63454540 474c4942 4358585f ESaIcEE@GLIBCXX_
-  0x00006e10 332e3400 5f5a4e4b 33633130 34637564 3.4._ZNK3c104cud
-  0x00006e20 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
-  0x00006e30 64496d70 6c313465 78636861 6e676544 dImpl14exchangeD
-  0x00006e40 65766963 65454e53 5f364465 76696365 eviceENS_6Device
-  0x00006e50 45005f5a 4e336331 30323069 6e747275 E._ZN3c1020intru
-  0x00006e60 73697665 5f707472 5f746172 67657431 sive_ptr_target1
-  0x00006e70 3772656c 65617365 5f726573 6f757263 7release_resourc
-  0x00006e80 65734576 005f5a4e 53743130 5f486173 esEv._ZNSt10_Has
-  0x00006e90 68746162 6c654953 73537434 70616972 htableISsSt4pair
-  0x00006ea0 494b5373 50764553 61495333 5f454e53 IKSsPvESaIS3_ENS
-  0x00006eb0 74385f5f 64657461 696c3130 5f53656c t8__detail10_Sel
-  0x00006ec0 65637431 73744553 74386571 75616c5f ect1stESt8equal_
-  0x00006ed0 746f4953 73455374 34686173 68495373 toISsESt4hashISs
-  0x00006ee0 454e5335 5f31385f 4d6f645f 72616e67 ENS5_18_Mod_rang
-  0x00006ef0 655f6861 7368696e 67454e53 355f3230 e_hashingENS5_20
-  0x00006f00 5f446566 61756c74 5f72616e 6765645f _Default_ranged_
-  0x00006f10 68617368 454e5335 5f32305f 5072696d hashENS5_20_Prim
-  0x00006f20 655f7265 68617368 5f706f6c 69637945 e_rehash_policyE
-  0x00006f30 4e53355f 31375f48 61736874 61626c65 NS5_17_Hashtable
-  0x00006f40 5f747261 69747349 4c623145 4c623045 _traitsILb1ELb0E
-  0x00006f50 4c623145 45454539 5f4d5f72 65686173 Lb1EEEE9_M_rehas
-  0x00006f60 68456d52 4b6d0050 79457863 5f496d70 hEmRKm.PyExc_Imp
-  0x00006f70 6f727445 72726f72 005f5a4e 33633130 ortError._ZN3c10
-  0x00006f80 31315379 6d4e6f64 65496d70 6c326c74 11SymNodeImpl2lt
-  0x00006f90 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
-  0x00006fa0 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
-  0x00006fb0 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
-  0x00006fc0 61726765 745f6465 6661756c 745f6e75 arget_default_nu
-  0x00006fd0 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
-  0x00006fe0 5f5a4e4b 33633130 31315379 6d4e6f64 _ZNK3c1011SymNod
-  0x00006ff0 65496d70 6c313369 735f6e65 73746564 eImpl13is_nested
-  0x00007000 5f696e74 4576005f 5a4e5374 31396261 _intEv._ZNSt19ba
-  0x00007010 7369635f 6f737472 696e6773 74726561 sic_ostringstrea
-  0x00007020 6d496353 74313163 6861725f 74726169 mIcSt11char_trai
-  0x00007030 74734963 45536149 63454543 31457600 tsIcESaIcEEC1Ev.
-  0x00007040 5f5a5449 4e336331 3034696d 706c3664 _ZTIN3c104impl6d
-  0x00007050 65746169 6c333157 72617046 756e6374 etail31WrapFunct
-  0x00007060 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
-  0x00007070 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
-  0x00007080 6e736f72 4553345f 4553345f 4e535f34 nsorES4_ES4_NS_4
-  0x00007090 67757473 38747970 656c6973 74387479 guts8typelist8ty
-  0x000070a0 70656c69 7374494a 53345f45 45454545 pelistIJS4_EEEEE
-  0x000070b0 00507945 72725f4f 63637572 72656400 .PyErr_Occurred.
-  0x000070c0 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
-  0x000070d0 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000070e0 395f365f 6e6d735f 63755f31 62316437 9_6_nms_cu_1b1d7
-  0x000070f0 6430655f 32323030 31356e6d 735f6b65 d0e_220015nms_ke
-  0x00007100 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
-  0x00007110 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
+  0x00004c60 312e3300 5f5a4e37 746f7263 68616f34 1.3._ZN7torchao4
+  0x00004c70 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
+  0x00004c80 65393235 395f365f 6e6d735f 63755f31 e9259_6_nms_cu_1
+  0x00004c90 35623935 6539315f 32353836 31356e6d 5b95e91_258615nm
+  0x00004ca0 735f6b65 726e656c 5f696d70 6c494e33 s_kernel_implIN3
+  0x00004cb0 63313034 48616c66 45454576 6964504b c104HalfEEEvidPK
+  0x00004cc0 545f5079 00637564 61537472 65616d51 T_Py.cudaStreamQ
+  0x00004cd0 75657279 406c6962 63756461 72742e73 uery@libcudart.s
+  0x00004ce0 6f2e3132 005f5f63 75646152 65676973 o.12.__cudaRegis
+  0x00004cf0 74657246 61744269 6e617279 406c6962 terFatBinary@lib
+  0x00004d00 63756461 72742e73 6f2e3132 005f5a4e cudart.so.12._ZN
+  0x00004d10 33633130 31305465 6e736f72 54797065 3c1010TensorType
+  0x00004d20 33676574 4576005f 5a4e4b33 63313034 3getEv._ZNK3c104
+  0x00004d30 696d706c 31365669 72747561 6c477561 impl16VirtualGua
+  0x00004d40 7264496d 706c3562 6c6f636b 45507652 rdImpl5blockEPvR
+  0x00004d50 4b4e535f 36537472 65616d45 005f5a4e KNS_6StreamE._ZN
+  0x00004d60 33633130 3653796d 496e7443 31454e53 3c106SymIntC1ENS
+  0x00004d70 5f313369 6e747275 73697665 5f707472 _13intrusive_ptr
+  0x00004d80 494e535f 31315379 6d4e6f64 65496d70 INS_11SymNodeImp
+  0x00004d90 6c454e53 5f366465 7461696c 3334696e lENS_6detail34in
+  0x00004da0 74727573 6976655f 74617267 65745f64 trusive_target_d
+  0x00004db0 65666175 6c745f6e 756c6c5f 74797065 efault_null_type
+  0x00004dc0 4953325f 45454545 005f5a4e 33633130 IS2_EEEE._ZN3c10
+  0x00004dd0 34637564 61313445 78636861 6e676544 4cuda14ExchangeD
+  0x00004de0 65766963 65456100 5f5a4e33 63313034 eviceEa._ZN3c104
+  0x00004df0 63756461 32307365 74437572 72656e74 cuda20setCurrent
+  0x00004e00 43554441 53747265 616d454e 53305f31 CUDAStreamENS0_1
+  0x00004e10 30435544 41537472 65616d45 005f5a54 0CUDAStreamE._ZT
+  0x00004e20 494e3363 31303230 696e7472 75736976 IN3c1020intrusiv
+  0x00004e30 655f7074 725f7461 72676574 45005f5a e_ptr_targetE._Z
+  0x00004e40 4e4b3363 31303545 72726f72 32327768 NK3c105Error22wh
+  0x00004e50 61745f77 6974686f 75745f62 61636b74 at_without_backt
+  0x00004e60 72616365 4576005f 5a544946 4e326174 raceEv._ZTIFN2at
+  0x00004e70 3654656e 736f7245 524b5330 5f53325f 6TensorERKS0_S2_
+  0x00004e80 6445005f 5a4e5374 31337275 6e74696d dE._ZNSt13runtim
+  0x00004e90 655f6572 726f7244 32457640 474c4942 e_errorD2Ev@GLIB
+  0x00004ea0 4358585f 332e3400 5f5a5374 31316d61 CXX_3.4._ZSt11ma
+  0x00004eb0 6b655f75 6e697175 65494e35 746f7263 ke_uniqueIN5torc
+  0x00004ec0 68386175 746f6772 61643132 4175746f h8autograd12Auto
+  0x00004ed0 67726164 4d657461 454a504e 33633130 gradMetaEJPN3c10
+  0x00004ee0 31305465 6e736f72 496d706c 45526245 10TensorImplERbE
+  0x00004ef0 454e5374 395f4d61 6b65556e 69714954 ENSt9_MakeUniqIT
+  0x00004f00 5f453135 5f5f7369 6e676c65 5f6f626a _E15__single_obj
+  0x00004f10 65637445 44704f54 305f005f 5a54564e ectEDpOT0_._ZTVN
+  0x00004f20 31305f5f 63787861 62697631 32305f5f 10__cxxabiv120__
+  0x00004f30 66756e63 74696f6e 5f747970 655f696e function_type_in
+  0x00004f40 666f4540 43585841 42495f31 2e33005f foE@CXXABI_1.3._
+  0x00004f50 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
+  0x00004f60 6d706c37 73796d5f 6e6f7445 76005f5a mpl7sym_notEv._Z
+  0x00004f70 4e326174 345f6f70 7339746f 5f646576 N2at4_ops9to_dev
+  0x00004f80 69636534 63616c6c 45524b4e 535f3654 ice4callERKNS_6T
+  0x00004f90 656e736f 72454e33 63313036 44657669 ensorEN3c106Devi
+  0x00004fa0 6365454e 53355f31 30536361 6c617254 ceENS5_10ScalarT
+  0x00004fb0 79706545 62625374 386f7074 696f6e61 ypeEbbSt8optiona
+  0x00004fc0 6c494e53 355f3132 4d656d6f 7279466f lINS5_12MemoryFo
+  0x00004fd0 726d6174 4545005f 5a54534e 33633130 rmatEE._ZTSN3c10
+  0x00004fe0 31355661 72696162 6c655665 7273696f 15VariableVersio
+  0x00004ff0 6e313456 65727369 6f6e436f 756e7465 n14VersionCounte
+  0x00005000 72450050 79427974 65735f41 73537472 rE.PyBytes_AsStr
+  0x00005010 696e6700 5f5a4e53 7431335f 42766563 ing._ZNSt13_Bvec
+  0x00005020 746f725f 62617365 49536149 62454531 tor_baseISaIbEE1
+  0x00005030 335f4d5f 6465616c 6c6f6361 74654576 3_M_deallocateEv
+  0x00005040 005f5a4e 53733132 5f4d5f6c 65616b5f ._ZNSs12_M_leak_
+  0x00005050 68617264 45764047 4c494243 58585f33 hardEv@GLIBCXX_3
+  0x00005060 2e34005f 5a544946 4e326174 3654656e .4._ZTIFN2at6Ten
+  0x00005070 736f7245 53305f53 305f4500 5f5a4e33 sorES0_S0_E._ZN3
+  0x00005080 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
+  0x00005090 3773796d 5f697465 45524b4e 535f3133 7sym_iteERKNS_13
+  0x000050a0 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
+  0x000050b0 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
+  0x000050c0 72757369 76655f74 61726765 745f6465 rusive_target_de
+  0x000050d0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
+  0x000050e0 53305f45 45454553 375f005f 5a4e3363 S0_EEEES7_._ZN3c
+  0x000050f0 31303664 65746169 6c323374 6f726368 106detail23torch
+  0x00005100 496e7465 726e616c 41737365 72744661 InternalAssertFa
+  0x00005110 696c4550 4b635332 5f6a5332 5f53325f ilEPKcS2_jS2_S2_
+  0x00005120 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
+  0x00005130 65496d70 6c386973 5f666c6f 61744576 eImpl8is_floatEv
+  0x00005140 005f5a31 37515541 4e545f47 454d4d5f ._Z17QUANT_GEMM_
+  0x00005150 4b65726e 656c4931 3254696c 696e6743 KernelI12TilingC
+  0x00005160 6f6e6669 67494c69 34454c69 31454c69 onfigILi4ELi1ELi
+  0x00005170 31454536 5f5f6861 6c664576 504b3575 1EE6__halfEvPK5u
+  0x00005180 696e7434 504b5332 5f53375f 5054305f int4PKS2_S7_PT0_
+  0x00005190 6d6d6d69 005f5a4e 536f395f 4d5f696e mmmi._ZNSo9_M_in
+  0x000051a0 73657274 496d4545 52536f54 5f40474c sertImEERSoT_@GL
+  0x000051b0 49424358 585f332e 342e3900 5f5a5374 IBCXX_3.4.9._ZSt
+  0x000051c0 31315f48 6173685f 62797465 73504b76 11_Hash_bytesPKv
+  0x000051d0 6d6d4043 58584142 495f312e 332e3500 mm@CXXABI_1.3.5.
+  0x000051e0 5f5a4e4b 53733572 66696e64 45504b63 _ZNKSs5rfindEPKc
+  0x000051f0 6d6d4047 4c494243 58585f33 2e34005f mm@GLIBCXX_3.4._
+  0x00005200 5a4e4b53 73313766 696e645f 66697273 ZNKSs17find_firs
+  0x00005210 745f6e6f 745f6f66 45504b63 6d6d4047 t_not_ofEPKcmm@G
+  0x00005220 4c494243 58585f33 2e340050 79427974 LIBCXX_3.4.PyByt
+  0x00005230 65417272 61795f53 697a6500 5f5a4e32 eArray_Size._ZN2
+  0x00005240 61743869 6e646578 696e6731 3154656e at8indexing11Ten
+  0x00005250 736f7249 6e646578 44314576 005f5a64 sorIndexD1Ev._Zd
+  0x00005260 6c507640 474c4942 4358585f 332e3400 lPv@GLIBCXX_3.4.
+  0x00005270 5f5a4e4b 33633130 34637564 6134696d _ZNK3c104cuda4im
+  0x00005280 706c3133 43554441 47756172 64496d70 pl13CUDAGuardImp
+  0x00005290 6c323367 65745374 7265616d 46726f6d l23getStreamFrom
+  0x000052a0 476c6f62 616c506f 6f6c454e 535f3644 GlobalPoolENS_6D
+  0x000052b0 65766963 65456200 5f5a4e4b 33633130 eviceEb._ZNK3c10
+  0x000052c0 34696d70 6c313656 69727475 616c4775 4impl16VirtualGu
+  0x000052d0 61726449 6d706c31 32676574 4e657753 ardImpl12getNewS
+  0x000052e0 74726561 6d454e53 5f364465 76696365 treamENS_6Device
+  0x000052f0 4569005f 5a4e5373 43314550 4b636d52 Ei._ZNSsC1EPKcmR
+  0x00005300 4b536149 63454047 4c494243 58585f33 KSaIcE@GLIBCXX_3
+  0x00005310 2e34005f 5a4e3363 31303131 53796d4e .4._ZN3c1011SymN
+  0x00005320 6f646549 6d706c31 326d6179 62655f61 odeImpl12maybe_a
+  0x00005330 735f696e 74457600 5f5a4e33 63313031 s_intEv._ZN3c101
+  0x00005340 344f7065 7261746f 724b6572 6e656c44 4OperatorKernelD
+  0x00005350 30457600 50794361 7073756c 655f4765 0Ev.PyCapsule_Ge
+  0x00005360 74436f6e 74657874 005f5a4e 4b326174 tContext._ZNK2at
+  0x00005370 31305465 6e736f72 42617365 32315f5f 10TensorBase21__
+  0x00005380 64697370 61746368 5f636f6e 74696775 dispatch_contigu
+  0x00005390 6f757345 4e336331 3031324d 656d6f72 ousEN3c1012Memor
+  0x000053a0 79466f72 6d617445 005f5a4e 33633130 yFormatE._ZN3c10
+  0x000053b0 31315379 6d4e6f64 65496d70 6c35626f 11SymNodeImpl5bo
+  0x000053c0 6f6c5f45 76005f5a 4e4b3363 31303469 ol_Ev._ZNK3c104i
+  0x000053d0 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
+  0x000053e0 64496d70 6c313773 796e6368 726f6e69 dImpl17synchroni
+  0x000053f0 7a655374 7265616d 45524b4e 535f3653 zeStreamERKNS_6S
+  0x00005400 74726561 6d45005f 5a4e3261 74345f6f treamE._ZN2at4_o
+  0x00005410 70733139 656d7074 795f6d65 6d6f7279 ps19empty_memory
+  0x00005420 5f666f72 6d617434 63616c6c 454e3363 _format4callEN3c
+  0x00005430 31303841 72726179 52656649 4e53325f 108ArrayRefINS2_
+  0x00005440 3653796d 496e7445 45455374 386f7074 6SymIntEEESt8opt
+  0x00005450 696f6e61 6c494e53 325f3130 5363616c ionalINS2_10Scal
+  0x00005460 61725479 70654545 53365f49 4e53325f arTypeEES6_INS2_
+  0x00005470 364c6179 6f757445 4553365f 494e5332 6LayoutEES6_INS2
+  0x00005480 5f364465 76696365 45455336 5f496245 _6DeviceEES6_IbE
+  0x00005490 53365f49 4e53325f 31324d65 6d6f7279 S6_INS2_12Memory
+  0x000054a0 466f726d 61744545 005f5a4e 33633130 FormatEE._ZN3c10
+  0x000054b0 31315379 6d4e6f64 65496d70 6c35636c 11SymNodeImpl5cl
+  0x000054c0 6f6e6545 76005f5a 54494e33 63313031 oneEv._ZTIN3c101
+  0x000054d0 344f7065 7261746f 724b6572 6e656c45 4OperatorKernelE
+  0x000054e0 005f5a4e 53733661 7070656e 6445504b ._ZNSs6appendEPK
+  0x000054f0 636d4047 4c494243 58585f33 2e34005f cm@GLIBCXX_3.4._
+  0x00005500 5a4e3363 31303230 696e7472 75736976 ZN3c1020intrusiv
+  0x00005510 655f7074 725f7461 72676574 44304576 e_ptr_targetD0Ev
+  0x00005520 005f5a4e 53733473 77617045 52537340 ._ZNSs4swapERSs@
+  0x00005530 474c4942 4358585f 332e3400 5f5a5456 GLIBCXX_3.4._ZTV
+  0x00005540 4e336331 30313556 61726961 626c6556 N3c1015VariableV
+  0x00005550 65727369 6f6e3134 56657273 696f6e43 ersion14VersionC
+  0x00005560 6f756e74 65724500 5f507954 7970655f ounterE._PyType_
+  0x00005570 4c6f6f6b 75700050 79546872 65616453 Lookup.PyThreadS
+  0x00005580 74617465 5f436c65 61720050 79457272 tate_Clear.PyErr
+  0x00005590 5f436c65 6172005f 5a4e5374 36766563 _Clear._ZNSt6vec
+  0x000055a0 746f7249 62536149 62454531 345f4d5f torIbSaIbEE14_M_
+  0x000055b0 66696c6c 5f696e73 65727445 53743133 fill_insertESt13
+  0x000055c0 5f426974 5f697465 7261746f 726d6200 _Bit_iteratormb.
+  0x000055d0 5f5f6378 615f7468 726f7740 43585841 __cxa_throw@CXXA
+  0x000055e0 42495f31 2e330063 75646153 74726561 BI_1.3.cudaStrea
+  0x000055f0 6d53796e 6368726f 6e697a65 406c6962 mSynchronize@lib
+  0x00005600 63756461 72742e73 6f2e3132 005f5a54 cudart.so.12._ZT
+  0x00005610 53464e32 61743654 656e736f 7245524b SFN2at6TensorERK
+  0x00005620 53305f53 325f6445 00507943 61707375 S0_S2_dE.PyCapsu
+  0x00005630 6c655f4e 65770050 794d656d 5f43616c le_New.PyMem_Cal
+  0x00005640 6c6f6300 5f5a4e33 63313034 696d706c loc._ZN3c104impl
+  0x00005650 36646574 61696c33 31577261 7046756e 6detail31WrapFun
+  0x00005660 6374696f 6e496e74 6f52756e 74696d65 ctionIntoRuntime
+  0x00005670 46756e63 746f725f 4950464e 32617436 Functor_IPFN2at6
+  0x00005680 54656e73 6f724553 345f5334 5f455334 TensorES4_S4_ES4
+  0x00005690 5f4e535f 34677574 73387479 70656c69 _NS_4guts8typeli
+  0x000056a0 73743874 7970656c 69737449 4a53345f st8typelistIJS4_
+  0x000056b0 53345f45 45454544 31457600 5f5a4e33 S4_EEEED1Ev._ZN3
+  0x000056c0 63313036 64657461 696c3132 5f737472 c106detail12_str
+  0x000056d0 5f777261 70706572 494a504b 63524b6c _wrapperIJPKcRKl
+  0x000056e0 45453463 616c6c45 524b5333 5f53355f EE4callERKS3_S5_
+  0x000056f0 005f5a4e 32617434 5f6f7073 3131736f ._ZN2at4_ops11so
+  0x00005700 72745f73 7461626c 65346361 6c6c4552 rt_stable4callER
+  0x00005710 4b4e535f 3654656e 736f7245 5374386f KNS_6TensorESt8o
+  0x00005720 7074696f 6e616c49 62456c62 005f5a53 ptionalIbElb._ZS
+  0x00005730 7432305f 5f746872 6f775f6c 656e6774 t20__throw_lengt
+  0x00005740 685f6572 726f7250 4b634047 4c494243 h_errorPKc@GLIBC
+  0x00005750 58585f33 2e34005f 5a4e3574 6f726368 XX_3.4._ZN5torch
+  0x00005760 374c6962 72617279 4331454e 53305f34 7LibraryC1ENS0_4
+  0x00005770 4b696e64 45537353 74386f70 74696f6e KindESsSt8option
+  0x00005780 616c494e 33633130 31314469 73706174 alIN3c1011Dispat
+  0x00005790 63684b65 79454550 4b636a00 5f556e77 chKeyEEPKcj._Unw
+  0x000057a0 696e645f 52657375 6d654047 43435f33 ind_Resume@GCC_3
+  0x000057b0 2e30005f 5a4e4b33 63313034 63756461 .0._ZNK3c104cuda
+  0x000057c0 34696d70 6c313343 55444147 75617264 4impl13CUDAGuard
+  0x000057d0 496d706c 31317175 65727953 74726561 Impl11queryStrea
+  0x000057e0 6d45524b 4e535f36 53747265 616d4500 mERKNS_6StreamE.
+  0x000057f0 50794279 7465735f 53697a65 005f5a54 PyBytes_Size._ZT
+  0x00005800 534e3363 31303469 6d706c36 64657461 SN3c104impl6deta
+  0x00005810 696c3331 57726170 46756e63 74696f6e il31WrapFunction
+  0x00005820 496e746f 52756e74 696d6546 756e6374 IntoRuntimeFunct
+  0x00005830 6f725f49 50464e32 61743654 656e736f or_IPFN2at6Tenso
+  0x00005840 72455334 5f53345f 4553345f 4e535f34 rES4_S4_ES4_NS_4
+  0x00005850 67757473 38747970 656c6973 74387479 guts8typelist8ty
+  0x00005860 70656c69 7374494a 53345f53 345f4545 pelistIJS4_S4_EE
+  0x00005870 45454500 5f5a4e33 63313031 3153796d EEE._ZN3c1011Sym
+  0x00005880 4e6f6465 496d706c 31366e65 73746564 NodeImpl16nested
+  0x00005890 5f696e74 5f636f65 66664576 005f5a4e _int_coeffEv._ZN
+  0x000058a0 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
+  0x000058b0 33435544 41477561 7264496d 706c3136 3CUDAGuardImpl16
+  0x000058c0 73796e63 68726f6e 697a6545 76656e74 synchronizeEvent
+  0x000058d0 45507600 5f5a4e33 63313034 63756461 EPv._ZN3c104cuda
+  0x000058e0 31326465 76696365 5f636f75 6e744576 12device_countEv
+  0x000058f0 005f5a4e 4b336331 30346375 64613469 ._ZNK3c104cuda4i
+  0x00005900 6d706c31 33435544 41477561 7264496d mpl13CUDAGuardIm
+  0x00005910 706c3967 65744465 76696365 4576005f pl9getDeviceEv._
+  0x00005920 5a323042 6974496e 7465726c 65617669 Z20BitInterleavi
+  0x00005930 6e675f32 62697450 68005f5a 4e37746f ng_2bitPh._ZN7to
+  0x00005940 72636861 6f323577 65696768 745f6d61 rchao25weight_ma
+  0x00005950 74726978 5f646571 75616e74 5f637075 trix_dequant_cpu
+  0x00005960 454e3261 74365465 6e736f72 4553315f EN2at6TensorES1_
+  0x00005970 0076736e 7072696e 74664047 4c494243 .vsnprintf@GLIBC
+  0x00005980 5f322e32 2e35005f 5a4e3363 31303469 _2.2.5._ZN3c104i
+  0x00005990 6d706c32 38777261 705f6b65 726e656c mpl28wrap_kernel
+  0x000059a0 5f66756e 63746f72 5f756e62 6f786564 _functor_unboxed
+  0x000059b0 5f494e53 305f3664 65746169 6c333157 _INS0_6detail31W
+  0x000059c0 72617046 756e6374 696f6e49 6e746f52 rapFunctionIntoR
+  0x000059d0 756e7469 6d654675 6e63746f 725f4950 untimeFunctor_IP
+  0x000059e0 464e3261 74365465 6e736f72 4553355f FN2at6TensorES5_
+  0x000059f0 4553355f 4e535f34 67757473 38747970 ES5_NS_4guts8typ
+  0x00005a00 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x00005a10 53355f45 45454545 53365f45 3463616c S5_EEEEES6_E4cal
+  0x00005a20 6c45504e 535f3134 4f706572 61746f72 lEPNS_14Operator
+  0x00005a30 4b65726e 656c454e 535f3134 44697370 KernelENS_14Disp
+  0x00005a40 61746368 4b657953 65744553 355f005f atchKeySetES5_._
+  0x00005a50 5a4e3363 31303135 56617269 61626c65 ZN3c1015Variable
+  0x00005a60 56657273 696f6e31 34566572 73696f6e Version14Version
+  0x00005a70 436f756e 74657244 30457600 5f5a4e33 CounterD0Ev._ZN3
+  0x00005a80 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
+  0x00005a90 3773796d 5f6d6178 45524b4e 535f3133 7sym_maxERKNS_13
+  0x00005aa0 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
+  0x00005ab0 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
+  0x00005ac0 72757369 76655f74 61726765 745f6465 rusive_target_de
+  0x00005ad0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
+  0x00005ae0 53305f45 45454500 5f5a5449 464e3261 S0_EEEE._ZTIFN2a
+  0x00005af0 74365465 6e736f72 4553305f 53305f53 t6TensorES0_S0_S
+  0x00005b00 305f6c45 00507945 78635f54 79706545 0_lE.PyExc_TypeE
+  0x00005b10 72726f72 005f5a4e 33633130 31315379 rror._ZN3c1011Sy
+  0x00005b20 6d4e6f64 65496d70 6c35666c 6f6f7245 mNodeImpl5floorE
+  0x00005b30 76005f5a 54494e33 63313034 63756461 v._ZTIN3c104cuda
+  0x00005b40 34696d70 6c313343 55444147 75617264 4impl13CUDAGuard
+  0x00005b50 496d706c 45005f5a 4e4b3363 31303469 ImplE._ZNK3c104i
+  0x00005b60 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
+  0x00005b70 64496d70 6c313875 6e636865 636b6564 dImpl18unchecked
+  0x00005b80 53657444 65766963 65454e53 5f364465 SetDeviceENS_6De
+  0x00005b90 76696365 45005f5a 4e4b3363 31303463 viceE._ZNK3c104c
+  0x00005ba0 75646134 696d706c 31334355 44414775 uda4impl13CUDAGu
+  0x00005bb0 61726449 6d706c39 73657444 65766963 ardImpl9setDevic
+  0x00005bc0 65454e53 5f364465 76696365 45005f5a eENS_6DeviceE._Z
+  0x00005bd0 54564e33 63313031 3153796d 4e6f6465 TVN3c1011SymNode
+  0x00005be0 496d706c 45005f5a 54494e33 63313031 ImplE._ZTIN3c101
+  0x00005bf0 3056616c 75654572 726f7245 005f5a54 0ValueErrorE._ZT
+  0x00005c00 564e3363 31303469 6d706c36 64657461 VN3c104impl6deta
+  0x00005c10 696c3331 57726170 46756e63 74696f6e il31WrapFunction
+  0x00005c20 496e746f 52756e74 696d6546 756e6374 IntoRuntimeFunct
+  0x00005c30 6f725f49 50464e32 61743654 656e736f or_IPFN2at6Tenso
+  0x00005c40 72455334 5f455334 5f4e535f 34677574 rES4_ES4_NS_4gut
+  0x00005c50 73387479 70656c69 73743874 7970656c s8typelist8typel
+  0x00005c60 69737449 4a53345f 45454545 45005079 istIJS4_EEEEE.Py
+  0x00005c70 54797065 5f526561 6479005f 5a544953 Type_Ready._ZTIS
+  0x00005c80 74313962 61645f6f 7074696f 6e616c5f t19bad_optional_
+  0x00005c90 61636365 7373005f 5a54534e 33633130 access._ZTSN3c10
+  0x00005ca0 34696d70 6c366465 7461696c 33315772 4impl6detail31Wr
+  0x00005cb0 61704675 6e637469 6f6e496e 746f5275 apFunctionIntoRu
+  0x00005cc0 6e74696d 6546756e 63746f72 5f495046 ntimeFunctor_IPF
+  0x00005cd0 4e326174 3654656e 736f7245 53345f45 N2at6TensorES4_E
+  0x00005ce0 53345f4e 535f3467 75747338 74797065 S4_NS_4guts8type
+  0x00005cf0 6c697374 38747970 656c6973 74494a53 list8typelistIJS
+  0x00005d00 345f4545 45454500 5f5a4e33 63313031 4_EEEEE._ZN3c101
+  0x00005d10 3153796d 4e6f6465 496d706c 32676545 1SymNodeImpl2geE
+  0x00005d20 524b4e53 5f313369 6e747275 73697665 RKNS_13intrusive
+  0x00005d30 5f707472 4953305f 4e535f36 64657461 _ptrIS0_NS_6deta
+  0x00005d40 696c3334 696e7472 75736976 655f7461 il34intrusive_ta
+  0x00005d50 72676574 5f646566 61756c74 5f6e756c rget_default_nul
+  0x00005d60 6c5f7479 70654953 305f4545 4545005f l_typeIS0_EEEE._
+  0x00005d70 5a4e3363 31303545 72726f72 4332454e ZN3c105ErrorC2EN
+  0x00005d80 535f3134 536f7572 63654c6f 63617469 S_14SourceLocati
+  0x00005d90 6f6e4553 73005f5a 54494e33 63313031 onESs._ZTIN3c101
+  0x00005da0 3153796d 4e6f6465 496d706c 45005f5a 1SymNodeImplE._Z
+  0x00005db0 53743234 5f5f7468 726f775f 6f75745f St24__throw_out_
+  0x00005dc0 6f665f72 616e6765 5f666d74 504b637a of_range_fmtPKcz
+  0x00005dd0 005f5a31 37515541 4e545f47 454d4d5f ._Z17QUANT_GEMM_
+  0x00005de0 4b65726e 656c4931 3254696c 696e6743 KernelI12TilingC
+  0x00005df0 6f6e6669 67494c69 34454c69 31454c69 onfigILi4ELi1ELi
+  0x00005e00 31454566 4576504b 3575696e 7434504b 1EEfEvPK5uint4PK
+  0x00005e10 365f5f68 616c6653 375f5054 305f6d6d 6__halfS7_PT0_mm
+  0x00005e20 6d69005f 5a4e3363 31303469 6d706c36 mi._ZN3c104impl6
+  0x00005e30 64657461 696c3331 57726170 46756e63 detail31WrapFunc
+  0x00005e40 74696f6e 496e746f 52756e74 696d6546 tionIntoRuntimeF
+  0x00005e50 756e6374 6f725f49 50464e32 61743654 unctor_IPFN2at6T
+  0x00005e60 656e736f 72455334 5f53345f 53345f6c ensorES4_S4_S4_l
+  0x00005e70 4553345f 4e535f34 67757473 38747970 ES4_NS_4guts8typ
+  0x00005e80 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x00005e90 53345f53 345f5334 5f6c4545 45454430 S4_S4_S4_lEEEED0
+  0x00005ea0 4576005f 5a4e3363 31303131 53796d4e Ev._ZN3c1011SymN
+  0x00005eb0 6f646549 6d706c31 3369735f 636f6e74 odeImpl13is_cont
+  0x00005ec0 6967756f 7573454e 535f3841 72726179 iguousENS_8Array
+  0x00005ed0 52656649 4e535f31 33696e74 72757369 RefINS_13intrusi
+  0x00005ee0 76655f70 74724953 305f4e53 5f366465 ve_ptrIS0_NS_6de
+  0x00005ef0 7461696c 3334696e 74727573 6976655f tail34intrusive_
+  0x00005f00 74617267 65745f64 65666175 6c745f6e target_default_n
+  0x00005f10 756c6c5f 74797065 4953305f 45454545 ull_typeIS0_EEEE
+  0x00005f20 45455337 5f005f5a 4e336331 30313153 EES7_._ZN3c1011S
+  0x00005f30 796d4e6f 6465496d 706c4430 4576005f ymNodeImplD0Ev._
+  0x00005f40 5a4e5373 36617373 69676e45 524b5373 ZNSs6assignERKSs
+  0x00005f50 40474c49 42435858 5f332e34 005f5a4e @GLIBCXX_3.4._ZN
+  0x00005f60 53733661 73736967 6e45504b 636d4047 Ss6assignEPKcm@G
+  0x00005f70 4c494243 58585f33 2e34005f 5a4e3363 LIBCXX_3.4._ZN3c
+  0x00005f80 31303131 53796d4e 6f646549 6d706c36 1011SymNodeImpl6
+  0x00005f90 73796d5f 6f724552 4b4e535f 3133696e sym_orERKNS_13in
+  0x00005fa0 74727573 6976655f 70747249 53305f4e trusive_ptrIS0_N
+  0x00005fb0 535f3664 65746169 6c333469 6e747275 S_6detail34intru
+  0x00005fc0 73697665 5f746172 6765745f 64656661 sive_target_defa
+  0x00005fd0 756c745f 6e756c6c 5f747970 65495330 ult_null_typeIS0
+  0x00005fe0 5f454545 45005f5a 4e336331 30313153 _EEEE._ZN3c1011S
+  0x00005ff0 796d4e6f 6465496d 706c3370 6f774552 ymNodeImpl3powER
+  0x00006000 4b4e535f 3133696e 74727573 6976655f KNS_13intrusive_
+  0x00006010 70747249 53305f4e 535f3664 65746169 ptrIS0_NS_6detai
+  0x00006020 6c333469 6e747275 73697665 5f746172 l34intrusive_tar
+  0x00006030 6765745f 64656661 756c745f 6e756c6c get_default_null
+  0x00006040 5f747970 65495330 5f454545 45005f5a _typeIS0_EEEE._Z
+  0x00006050 4e336331 30366465 7461696c 3233746f N3c106detail23to
+  0x00006060 72636849 6e746572 6e616c41 73736572 rchInternalAsser
+  0x00006070 74466169 6c45504b 6353325f 6a53325f tFailEPKcS2_jS2_
+  0x00006080 524b5373 00507949 6e69745f 5f43005f RKSs.PyInit__C._
+  0x00006090 5a4e5373 36617070 656e6445 524b5373 ZNSs6appendERKSs
+  0x000060a0 40474c49 42435858 5f332e34 005f5a54 @GLIBCXX_3.4._ZT
+  0x000060b0 53464e32 61743654 656e736f 72455330 SFN2at6TensorES0
+  0x000060c0 5f53305f 45005079 5475706c 655f4765 _S0_E.PyTuple_Ge
+  0x000060d0 74497465 6d005f5a 4e537431 355f5f65 tItem._ZNSt15__e
+  0x000060e0 78636570 74696f6e 5f707472 6e654552 xception_ptrneER
+  0x000060f0 4b4e535f 31336578 63657074 696f6e5f KNS_13exception_
+  0x00006100 70747245 53325f40 43585841 42495f31 ptrES2_@CXXABI_1
+  0x00006110 2e332e33 005f5a4e 37746f72 6368616f .3.3._ZN7torchao
+  0x00006120 32387765 69676874 5f6d6174 7269785f 28weight_matrix_
+  0x00006130 70726570 61636b69 6e675f63 7075454e prepacking_cpuEN
+  0x00006140 32617436 54656e73 6f724500 5f50794f 2at6TensorE._PyO
+  0x00006150 626a6563 745f4765 74446963 74507472 bject_GetDictPtr
+  0x00006160 005f5a4e 4b326174 3654656e 736f7235 ._ZNK2at6Tensor5
+  0x00006170 696e6465 78455374 3136696e 69746961 indexESt16initia
+  0x00006180 6c697a65 725f6c69 7374494e 535f3869 lizer_listINS_8i
+  0x00006190 6e646578 696e6731 3154656e 736f7249 ndexing11TensorI
+  0x000061a0 6e646578 4545005f 5f637861 5f617465 ndexEE.__cxa_ate
+  0x000061b0 78697440 474c4942 435f322e 322e3500 xit@GLIBC_2.2.5.
+  0x000061c0 5f5a5456 4e336331 3031344f 70657261 _ZTVN3c1014Opera
+  0x000061d0 746f724b 65726e65 6c45005f 5a4e4b32 torKernelE._ZNK2
+  0x000061e0 61743130 54656e73 6f724261 73653864 at10TensorBase8d
+  0x000061f0 6174615f 70747249 6c454550 545f7600 ata_ptrIlEEPT_v.
+  0x00006200 50795475 706c655f 53657449 74656d00 PyTuple_SetItem.
+  0x00006210 5f5a3137 5155414e 545f4745 4d4d5f4b _Z17QUANT_GEMM_K
+  0x00006220 65726e65 6c493132 54696c69 6e67436f ernelI12TilingCo
+  0x00006230 6e666967 494c6934 454c6931 454c6938 nfigILi4ELi1ELi8
+  0x00006240 45456645 76504b35 75696e74 34504b36 EEfEvPK5uint4PK6
+  0x00006250 5f5f6861 6c665337 5f505430 5f6d6d6d __halfS7_PT0_mmm
+  0x00006260 69005079 54687265 61645f74 73735f67 i.PyThread_tss_g
+  0x00006270 65740050 79457272 5f526573 746f7265 et.PyErr_Restore
+  0x00006280 005f5a32 39776569 6768745f 70726570 ._Z29weight_prep
+  0x00006290 61636b69 6e675f66 7031365f 746f5f66 acking_fp16_to_f
+  0x000062a0 70365074 50686d6d 005f5a4e 35746f72 p6PtPhmm._ZN5tor
+  0x000062b0 63683565 6d707479 454e3363 31303841 ch5emptyEN3c108A
+  0x000062c0 72726179 52656649 6c45454e 53305f31 rrayRefIlEENS0_1
+  0x000062d0 3354656e 736f724f 7074696f 6e734553 3TensorOptionsES
+  0x000062e0 74386f70 74696f6e 616c494e 53305f31 t8optionalINS0_1
+  0x000062f0 324d656d 6f727946 6f726d61 74454500 2MemoryFormatEE.
+  0x00006300 5f5a4e35 746f7263 68374c69 62726172 _ZN5torch7Librar
+  0x00006310 79443145 76005f5a 4e336331 30346375 yD1Ev._ZN3c104cu
+  0x00006320 64613469 6d706c31 33435544 41477561 da4impl13CUDAGua
+  0x00006330 7264496d 706c4431 4576005f 5f637861 rdImplD1Ev.__cxa
+  0x00006340 5f707572 655f7669 72747561 6c404358 _pure_virtual@CX
+  0x00006350 58414249 5f312e33 005f5f70 74687265 XABI_1.3.__pthre
+  0x00006360 61645f6b 65795f63 72656174 6540474c ad_key_create@GL
+  0x00006370 4942435f 322e322e 35005f5a 4e537431 IBC_2.2.5._ZNSt1
+  0x00006380 355f5f65 78636570 74696f6e 5f707472 5__exception_ptr
+  0x00006390 31336578 63657074 696f6e5f 70747234 13exception_ptr4
+  0x000063a0 73776170 45525330 5f404358 58414249 swapERS0_@CXXABI
+  0x000063b0 5f312e33 2e33005f 5a4e3363 31303131 _1.3.3._ZN3c1011
+  0x000063c0 53796d4e 6f646549 6d706c31 30777261 SymNodeImpl10wra
+  0x000063d0 705f666c 6f617445 64005f5a 4e4b3363 p_floatEd._ZNK3c
+  0x000063e0 31303463 75646134 696d706c 31334355 104cuda4impl13CU
+  0x000063f0 44414775 61726449 6d706c36 7265636f DAGuardImpl6reco
+  0x00006400 72644550 5076524b 4e535f36 53747265 rdEPPvRKNS_6Stre
+  0x00006410 616d4561 4e535f39 4576656e 74466c61 amEaNS_9EventFla
+  0x00006420 6745005f 5a4e5235 746f7263 68374c69 gE._ZNR5torch7Li
+  0x00006430 62726172 79355f69 6d706c45 504b634f brary5_implEPKcO
+  0x00006440 4e535f31 31437070 46756e63 74696f6e NS_11CppFunction
+  0x00006450 454e535f 31375f52 65676973 7465724f ENS_17_RegisterO
+  0x00006460 72566572 69667945 005f5a53 74706c49 rVerifyE._ZStplI
+  0x00006470 63537431 31636861 725f7472 61697473 cSt11char_traits
+  0x00006480 49634553 61496345 45536249 545f5430 IcESaIcEESbIT_T0
+  0x00006490 5f54315f 45504b53 335f524b 53365f00 _T1_EPKS3_RKS6_.
+  0x000064a0 5f5a4e53 73433145 524b5361 49634540 _ZNSsC1ERKSaIcE@
+  0x000064b0 474c4942 4358585f 332e3400 5f5a4e33 GLIBCXX_3.4._ZN3
+  0x000064c0 63313034 63756461 39476574 44657669 c104cuda9GetDevi
+  0x000064d0 63654550 61005f5a 4e336331 30313467 ceEPa._ZN3c1014g
+  0x000064e0 65745479 70655074 72436f70 79494e32 etTypePtrCopyIN2
+  0x000064f0 61743654 656e736f 72454545 4e535f34 at6TensorEEENS_4
+  0x00006500 54797065 32345369 6e676c65 746f6e4f Type24SingletonO
+  0x00006510 72536861 72656454 79706550 74724953 rSharedTypePtrIS
+  0x00006520 335f4545 76005f5a 4e537334 5f526570 3_EEv._ZNSs4_Rep
+  0x00006530 31305f4d 5f646573 74726f79 45524b53 10_M_destroyERKS
+  0x00006540 61496345 40474c49 42435858 5f332e34 aIcE@GLIBCXX_3.4
+  0x00006550 005f5a4e 53743135 5f5f6578 63657074 ._ZNSt15__except
+  0x00006560 696f6e5f 70747231 33657863 65707469 ion_ptr13excepti
+  0x00006570 6f6e5f70 74724431 45764043 58584142 on_ptrD1Ev@CXXAB
+  0x00006580 495f312e 332e3300 5f5a4e32 6174345f I_1.3.3._ZN2at4_
+  0x00006590 6f707331 32696e64 65785f73 656c6563 ops12index_selec
+  0x000065a0 74346361 6c6c4552 4b4e535f 3654656e t4callERKNS_6Ten
+  0x000065b0 736f7245 6c53345f 00507954 68726561 sorElS4_.PyThrea
+  0x000065c0 645f7473 735f616c 6c6f6300 5f5a5449 d_tss_alloc._ZTI
+  0x000065d0 53743136 6e657374 65645f65 78636570 St16nested_excep
+  0x000065e0 74696f6e 40435858 4142495f 312e332e tion@CXXABI_1.3.
+  0x000065f0 35005f5a 4e336331 30313153 796d4e6f 5._ZN3c1011SymNo
+  0x00006600 6465496d 706c326c 6545524b 4e535f31 deImpl2leERKNS_1
+  0x00006610 33696e74 72757369 76655f70 74724953 3intrusive_ptrIS
+  0x00006620 305f4e53 5f366465 7461696c 3334696e 0_NS_6detail34in
+  0x00006630 74727573 6976655f 74617267 65745f64 trusive_target_d
+  0x00006640 65666175 6c745f6e 756c6c5f 74797065 efault_null_type
+  0x00006650 4953305f 45454545 005f5a4e 4b336331 IS0_EEEE._ZNK3c1
+  0x00006660 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
+  0x00006670 75617264 496d706c 31346578 6368616e uardImpl14exchan
+  0x00006680 67654465 76696365 454e535f 36446576 geDeviceENS_6Dev
+  0x00006690 69636545 005f5a4e 4b336331 3034696d iceE._ZNK3c104im
+  0x000066a0 706c3136 56697274 75616c47 75617264 pl16VirtualGuard
+  0x000066b0 496d706c 31366765 74446566 61756c74 Impl16getDefault
+  0x000066c0 53747265 616d454e 535f3644 65766963 StreamENS_6Devic
+  0x000066d0 6545005f 5a4e3663 61666665 32385479 eE._ZN6caffe28Ty
+  0x000066e0 70654d65 74613236 6572726f 725f756e peMeta26error_un
+  0x000066f0 73757070 6f727465 645f7479 70656d65 supported_typeme
+  0x00006700 74614553 305f005f 5a4e3363 31303131 taES0_._ZN3c1011
+  0x00006710 53796d4e 6f646549 6d706c37 69735f62 SymNodeImpl7is_b
+  0x00006720 6f6f6c45 76005f5a 54495374 31337275 oolEv._ZTISt13ru
+  0x00006730 6e74696d 655f6572 726f7240 474c4942 ntime_error@GLIB
+  0x00006740 4358585f 332e3400 5f5a4e33 63313031 CXX_3.4._ZN3c101
+  0x00006750 344f7065 7261746f 724b6572 6e656c44 4OperatorKernelD
+  0x00006760 31457600 63756461 47657445 72726f72 1Ev.cudaGetError
+  0x00006770 53747269 6e67406c 69626375 64617274 String@libcudart
+  0x00006780 2e736f2e 3132005f 5a4e5374 31337275 .so.12._ZNSt13ru
+  0x00006790 6e74696d 655f6572 726f7243 3145524b ntime_errorC1ERK
+  0x000067a0 53734047 4c494243 58585f33 2e34005f Ss@GLIBCXX_3.4._
+  0x000067b0 5a4e3261 74345f6f 7073366e 6172726f ZN2at4_ops6narro
+  0x000067c0 77346361 6c6c4552 4b4e535f 3654656e w4callERKNS_6Ten
+  0x000067d0 736f7245 6c4e3363 31303653 796d496e sorElN3c106SymIn
+  0x000067e0 74455336 5f005f5a 4e336331 30313153 tES6_._ZN3c1011S
+  0x000067f0 796d4e6f 6465496d 706c326e 6545524b ymNodeImpl2neERK
+  0x00006800 4e535f31 33696e74 72757369 76655f70 NS_13intrusive_p
+  0x00006810 74724953 305f4e53 5f366465 7461696c trIS0_NS_6detail
+  0x00006820 3334696e 74727573 6976655f 74617267 34intrusive_targ
+  0x00006830 65745f64 65666175 6c745f6e 756c6c5f et_default_null_
+  0x00006840 74797065 4953305f 45454545 005f5a4e typeIS0_EEEE._ZN
+  0x00006850 35746f72 63683861 75746f67 72616431 5torch8autograd1
+  0x00006860 336d616b 655f7661 72696162 6c65454e 3make_variableEN
+  0x00006870 32617436 54656e73 6f724562 62005f5a 2at6TensorEbb._Z
+  0x00006880 4e537431 35626173 69635f73 7472696e NSt15basic_strin
+  0x00006890 67627566 49635374 31316368 61725f74 gbufIcSt11char_t
+  0x000068a0 72616974 73496345 53614963 45454430 raitsIcESaIcEED0
+  0x000068b0 4576005f 5a4e3363 31303135 56617269 Ev._ZN3c1015Vari
+  0x000068c0 61626c65 56657273 696f6e31 34566572 ableVersion14Ver
+  0x000068d0 73696f6e 436f756e 74657244 31457600 sionCounterD1Ev.
+  0x000068e0 5f5a4e33 63313031 3056616c 75654572 _ZN3c1010ValueEr
+  0x000068f0 726f7244 31457600 5f5a4e33 63313031 rorD1Ev._ZN3c101
+  0x00006900 3153796d 4e6f6465 496d706c 31316775 1SymNodeImpl11gu
+  0x00006910 6172645f 666c6f61 7445504b 636c005f ard_floatEPKcl._
+  0x00006920 5a537470 6c496353 74313163 6861725f ZStplIcSt11char_
+  0x00006930 74726169 74734963 45536149 63454553 traitsIcESaIcEES
+  0x00006940 6249545f 54305f54 315f454f 53365f53 bIT_T0_T1_EOS6_S
+  0x00006950 375f005f 5a54534e 33633130 31315379 7_._ZTSN3c1011Sy
+  0x00006960 6d4e6f64 65496d70 6c45005f 5a537431 mNodeImplE._ZSt1
+  0x00006970 365f5f6f 73747265 616d5f69 6e736572 6__ostream_inser
+  0x00006980 74496353 74313163 6861725f 74726169 tIcSt11char_trai
+  0x00006990 74734963 45455253 74313362 61736963 tsIcEERSt13basic
+  0x000069a0 5f6f7374 7265616d 49545f54 305f4553 _ostreamIT_T0_ES
+  0x000069b0 365f504b 53335f6c 40474c49 42435858 6_PKS3_l@GLIBCXX
+  0x000069c0 5f332e34 2e39005f 49544d5f 72656769 _3.4.9._ITM_regi
+  0x000069d0 73746572 544d436c 6f6e6554 61626c65 sterTMCloneTable
+  0x000069e0 00507943 46756e63 74696f6e 5f547970 .PyCFunction_Typ
+  0x000069f0 65005f5a 4e336331 3034696d 706c3664 e._ZN3c104impl6d
+  0x00006a00 65746169 6c333157 72617046 756e6374 etail31WrapFunct
+  0x00006a10 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
+  0x00006a20 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
+  0x00006a30 6e736f72 4553345f 53345f53 345f6c45 nsorES4_S4_S4_lE
+  0x00006a40 53345f4e 535f3467 75747338 74797065 S4_NS_4guts8type
+  0x00006a50 6c697374 38747970 656c6973 74494a53 list8typelistIJS
+  0x00006a60 345f5334 5f53345f 6c454545 45443245 4_S4_S4_lEEEED2E
+  0x00006a70 76005f5a 4e537343 3145524b 53736d6d v._ZNSsC1ERKSsmm
+  0x00006a80 40474c49 42435858 5f332e34 00507947 @GLIBCXX_3.4.PyG
+  0x00006a90 494c5374 6174655f 47657454 68697354 ILState_GetThisT
+  0x00006aa0 68726561 64537461 74650050 79427974 hreadState.PyByt
+  0x00006ab0 65735f41 73537472 696e6741 6e645369 es_AsStringAndSi
+  0x00006ac0 7a65006d 656d636d 7040474c 4942435f ze.memcmp@GLIBC_
+  0x00006ad0 322e322e 35005f5a 4e336331 30313369 2.2.5._ZN3c1013i
+  0x00006ae0 6e747275 73697665 5f707472 494e535f ntrusive_ptrINS_
+  0x00006af0 31355661 72696162 6c655665 7273696f 15VariableVersio
+  0x00006b00 6e313456 65727369 6f6e436f 756e7465 n14VersionCounte
+  0x00006b10 72454e53 5f366465 7461696c 3334696e rENS_6detail34in
+  0x00006b20 74727573 6976655f 74617267 65745f64 trusive_target_d
+  0x00006b30 65666175 6c745f6e 756c6c5f 74797065 efault_null_type
+  0x00006b40 4953325f 45454536 72657365 745f4576 IS2_EEE6reset_Ev
+  0x00006b50 00507955 6e69636f 64655f41 73456e63 .PyUnicode_AsEnc
+  0x00006b60 6f646564 53747269 6e67005f 5a4e4b53 odedString._ZNKS
+  0x00006b70 7337636f 6d706172 6545504b 6340474c s7compareEPKc@GL
+  0x00006b80 49424358 585f332e 34005f5a 4e4b3261 IBCXX_3.4._ZNK2a
+  0x00006b90 74313054 656e736f 72426173 65386461 t10TensorBase8da
+  0x00006ba0 74615f70 7472494e 33633130 3448616c ta_ptrIN3c104Hal
+  0x00006bb0 66454545 50545f76 005f5a4e 33633130 fEEEPT_v._ZN3c10
+  0x00006bc0 31315379 6d4e6f64 65496d70 6c443245 11SymNodeImplD2E
+  0x00006bd0 76005f5a 4e336331 30313153 796d4e6f v._ZN3c1011SymNo
+  0x00006be0 6465496d 706c3868 61735f68 696e7445 deImpl8has_hintE
+  0x00006bf0 76005079 5475706c 655f4e65 77005f5a v.PyTuple_New._Z
+  0x00006c00 31375155 414e545f 47454d4d 5f4b6572 17QUANT_GEMM_Ker
+  0x00006c10 6e656c49 31325469 6c696e67 436f6e66 nelI12TilingConf
+  0x00006c20 6967494c 6934454c 6931454c 69324545 igILi4ELi1ELi2EE
+  0x00006c30 365f5f68 616c6645 76504b35 75696e74 6__halfEvPK5uint
+  0x00006c40 34504b53 325f5337 5f505430 5f6d6d6d 4PKS2_S7_PT0_mmm
+  0x00006c50 69005f5a 4e35746f 72636836 64657461 i._ZN5torch6deta
+  0x00006c60 696c3136 546f7263 684c6962 72617279 il16TorchLibrary
+  0x00006c70 496e6974 44314576 0050794f 626a6563 InitD1Ev.PyObjec
+  0x00006c80 745f4361 6c6c4675 6e637469 6f6e4f62 t_CallFunctionOb
+  0x00006c90 6a417267 73005f5a 4e336331 3034696d jArgs._ZN3c104im
+  0x00006ca0 706c3233 4578636c 75646544 69737061 pl23ExcludeDispa
+  0x00006cb0 7463684b 65794775 61726443 31454e53 tchKeyGuardC1ENS
+  0x00006cc0 5f313444 69737061 7463684b 65795365 _14DispatchKeySe
+  0x00006cd0 7445005f 5a4e4b32 61743130 54656e73 tE._ZNK2at10Tens
+  0x00006ce0 6f724261 73653864 6174615f 70747249 orBase8data_ptrI
+  0x00006cf0 68454550 545f7600 5f5a4e4b 53743139 hEEPT_v._ZNKSt19
+  0x00006d00 6261645f 6f707469 6f6e616c 5f616363 bad_optional_acc
+  0x00006d10 65737334 77686174 4576005f 5a544953 ess4whatEv._ZTIS
+  0x00006d20 7431365f 53705f63 6f756e74 65645f62 t16_Sp_counted_b
+  0x00006d30 61736549 4c4e395f 5f676e75 5f637878 aseILN9__gnu_cxx
+  0x00006d40 31325f4c 6f636b5f 706f6c69 63794532 12_Lock_policyE2
+  0x00006d50 45450063 75646145 76656e74 53796e63 EE.cudaEventSync
+  0x00006d60 68726f6e 697a6540 6c696263 75646172 hronize@libcudar
+  0x00006d70 742e736f 2e313200 5f5a4e33 63313034 t.so.12._ZN3c104
+  0x00006d80 63756461 32306765 74446566 61756c74 cuda20getDefault
+  0x00006d90 43554441 53747265 616d4561 005f5a32 CUDAStreamEa._Z2
+  0x00006da0 34776569 6768745f 6d617472 69785f70 4weight_matrix_p
+  0x00006db0 72657061 636b696e 67506953 5f6d6d00 repackingPiS_mm.
+  0x00006dc0 5f5a4e4b 33633130 31305465 6e736f72 _ZNK3c1010Tensor
+  0x00006dd0 496d706c 36646576 69636545 76005f5a Impl6deviceEv._Z
+  0x00006de0 4e537436 76656374 6f724962 53614962 NSt6vectorIbSaIb
+  0x00006df0 45453133 5f4d5f69 6e736572 745f6175 EE13_M_insert_au
+  0x00006e00 78455374 31335f42 69745f69 74657261 xESt13_Bit_itera
+  0x00006e10 746f7262 005f5a4e 33633130 6c734552 torb._ZN3c10lsER
+  0x00006e20 536f4e53 5f313044 65766963 65547970 SoNS_10DeviceTyp
+  0x00006e30 6545005f 5a545453 74313962 61736963 eE._ZTTSt19basic
+  0x00006e40 5f6f7374 72696e67 73747265 616d4963 _ostringstreamIc
+  0x00006e50 53743131 63686172 5f747261 69747349 St11char_traitsI
+  0x00006e60 63455361 49634545 40474c49 42435858 cESaIcEE@GLIBCXX
+  0x00006e70 5f332e34 005f5a4e 4b336331 30346375 _3.4._ZNK3c104cu
+  0x00006e80 64613469 6d706c31 33435544 41477561 da4impl13CUDAGua
+  0x00006e90 7264496d 706c3134 65786368 616e6765 rdImpl14exchange
+  0x00006ea0 44657669 6365454e 535f3644 65766963 DeviceENS_6Devic
+  0x00006eb0 6545005f 5a4e3363 31303230 696e7472 eE._ZN3c1020intr
+  0x00006ec0 75736976 655f7074 725f7461 72676574 usive_ptr_target
+  0x00006ed0 31377265 6c656173 655f7265 736f7572 17release_resour
+  0x00006ee0 63657345 76005f5a 4e537431 305f4861 cesEv._ZNSt10_Ha
+  0x00006ef0 73687461 626c6549 53735374 34706169 shtableISsSt4pai
+  0x00006f00 72494b53 73507645 53614953 335f454e rIKSsPvESaIS3_EN
+  0x00006f10 5374385f 5f646574 61696c31 305f5365 St8__detail10_Se
+  0x00006f20 6c656374 31737445 53743865 7175616c lect1stESt8equal
+  0x00006f30 5f746f49 53734553 74346861 73684953 _toISsESt4hashIS
+  0x00006f40 73454e53 355f3138 5f4d6f64 5f72616e sENS5_18_Mod_ran
+  0x00006f50 67655f68 61736869 6e67454e 53355f32 ge_hashingENS5_2
+  0x00006f60 305f4465 6661756c 745f7261 6e676564 0_Default_ranged
+  0x00006f70 5f686173 68454e53 355f3230 5f507269 _hashENS5_20_Pri
+  0x00006f80 6d655f72 65686173 685f706f 6c696379 me_rehash_policy
+  0x00006f90 454e5335 5f31375f 48617368 7461626c ENS5_17_Hashtabl
+  0x00006fa0 655f7472 61697473 494c6231 454c6230 e_traitsILb1ELb0
+  0x00006fb0 454c6231 45454545 395f4d5f 72656861 ELb1EEEE9_M_reha
+  0x00006fc0 7368456d 524b6d00 50794578 635f496d shEmRKm.PyExc_Im
+  0x00006fd0 706f7274 4572726f 72005f5a 4e336331 portError._ZN3c1
+  0x00006fe0 30313153 796d4e6f 6465496d 706c326c 011SymNodeImpl2l
+  0x00006ff0 7445524b 4e535f31 33696e74 72757369 tERKNS_13intrusi
+  0x00007000 76655f70 74724953 305f4e53 5f366465 ve_ptrIS0_NS_6de
+  0x00007010 7461696c 3334696e 74727573 6976655f tail34intrusive_
+  0x00007020 74617267 65745f64 65666175 6c745f6e target_default_n
+  0x00007030 756c6c5f 74797065 4953305f 45454545 ull_typeIS0_EEEE
+  0x00007040 005f5a4e 4b336331 30313153 796d4e6f ._ZNK3c1011SymNo
+  0x00007050 6465496d 706c3133 69735f6e 65737465 deImpl13is_neste
+  0x00007060 645f696e 74457600 5f5a4e53 74313962 d_intEv._ZNSt19b
+  0x00007070 61736963 5f6f7374 72696e67 73747265 asic_ostringstre
+  0x00007080 616d4963 53743131 63686172 5f747261 amIcSt11char_tra
+  0x00007090 69747349 63455361 49634545 43314576 itsIcESaIcEEC1Ev
+  0x000070a0 005f5a54 494e3363 31303469 6d706c36 ._ZTIN3c104impl6
+  0x000070b0 64657461 696c3331 57726170 46756e63 detail31WrapFunc
+  0x000070c0 74696f6e 496e746f 52756e74 696d6546 tionIntoRuntimeF
+  0x000070d0 756e6374 6f725f49 50464e32 61743654 unctor_IPFN2at6T
+  0x000070e0 656e736f 72455334 5f455334 5f4e535f ensorES4_ES4_NS_
+  0x000070f0 34677574 73387479 70656c69 73743874 4guts8typelist8t
+  0x00007100 7970656c 69737449 4a53345f 45454545 ypelistIJS4_EEEE
+  0x00007110 45005079 4572725f 4f636375 72726564 E.PyErr_Occurred
   0x00007120 00507954 68726561 64537461 74655f44 .PyThreadState_D
   0x00007130 656c6574 65437572 72656e74 005f5a4e eleteCurrent._ZN
   0x00007140 33633130 3133696e 74727573 6976655f 3c1013intrusive_
   0x00007150 70747249 4e535f31 3153796d 4e6f6465 ptrINS_11SymNode
   0x00007160 496d706c 454e535f 36646574 61696c33 ImplENS_6detail3
   0x00007170 34696e74 72757369 76655f74 61726765 4intrusive_targe
   0x00007180 745f6465 6661756c 745f6e75 6c6c5f74 t_default_null_t
@@ -2230,251 +2230,251 @@
   0x00008b30 74657246 61744269 6e617279 456e6440 terFatBinaryEnd@
   0x00008b40 6c696263 75646172 742e736f 2e313200 libcudart.so.12.
   0x00008b50 5079496e 7374616e 63654d65 74686f64 PyInstanceMethod
   0x00008b60 5f4e6577 005f5a4e 33633130 31315379 _New._ZN3c1011Sy
   0x00008b70 6d4e6f64 65496d70 6c313169 735f636f mNodeImpl11is_co
   0x00008b80 6e737461 6e744576 005f5f67 78785f70 nstantEv.__gxx_p
   0x00008b90 6572736f 6e616c69 74795f76 30404358 ersonality_v0@CX
-  0x00008ba0 58414249 5f312e33 005f5a4e 4b336331 XABI_1.3._ZNK3c1
-  0x00008bb0 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
-  0x00008bc0 75617264 496d706c 34747970 65457600 uardImpl4typeEv.
-  0x00008bd0 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x00008be0 496d706c 38777261 705f696e 74456c00 Impl8wrap_intEl.
-  0x00008bf0 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x00008c00 496d706c 44314576 005f5a4e 33633130 ImplD1Ev._ZN3c10
-  0x00008c10 34696d70 6c33316d 616b655f 626f7865 4impl31make_boxe
-  0x00008c20 645f6672 6f6d5f75 6e626f78 65645f66 d_from_unboxed_f
-  0x00008c30 756e6374 6f72494e 53305f36 64657461 unctorINS0_6deta
-  0x00008c40 696c3331 57726170 46756e63 74696f6e il31WrapFunction
-  0x00008c50 496e746f 52756e74 696d6546 756e6374 IntoRuntimeFunct
-  0x00008c60 6f725f49 50464e32 61743654 656e736f or_IPFN2at6Tenso
-  0x00008c70 72455335 5f53355f 4553355f 4e535f34 rES5_S5_ES5_NS_4
-  0x00008c80 67757473 38747970 656c6973 74387479 guts8typelist8ty
-  0x00008c90 70656c69 7374494a 53355f53 355f4545 pelistIJS5_S5_EE
-  0x00008ca0 4545454c 62304545 3463616c 6c45504e EEELb0EE4callEPN
-  0x00008cb0 535f3134 4f706572 61746f72 4b65726e S_14OperatorKern
-  0x00008cc0 656c4552 4b4e535f 31344f70 65726174 elERKNS_14Operat
-  0x00008cd0 6f724861 6e646c65 454e535f 31344469 orHandleENS_14Di
-  0x00008ce0 73706174 63684b65 79536574 45505374 spatchKeySetEPSt
-  0x00008cf0 36766563 746f7249 4e535f36 4956616c 6vectorINS_6IVal
-  0x00008d00 75654553 6149534c 5f454500 5f5a4e4b ueESaISL_EE._ZNK
-  0x00008d10 33633130 34637564 6134696d 706c3133 3c104cuda4impl13
-  0x00008d20 43554441 47756172 64496d70 6c313267 CUDAGuardImpl12g
-  0x00008d30 65744e65 77537472 65616d45 4e535f36 etNewStreamENS_6
-  0x00008d40 44657669 63654569 00507944 6963745f DeviceEi.PyDict_
-  0x00008d50 4e657700 5f5a4e33 63313031 35566172 New._ZN3c1015Var
-  0x00008d60 6961626c 65566572 73696f6e 31345665 iableVersion14Ve
-  0x00008d70 7273696f 6e436f75 6e746572 44324576 rsionCounterD2Ev
-  0x00008d80 00507943 61707375 6c655f53 6574506f .PyCapsule_SetPo
-  0x00008d90 696e7465 72005f5a 4e537438 696f735f inter._ZNSt8ios_
-  0x00008da0 62617365 34496e69 74443145 7640474c base4InitD1Ev@GL
-  0x00008db0 49424358 585f332e 34005f5a 4e336331 IBCXX_3.4._ZN3c1
-  0x00008dc0 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
-  0x00008dd0 75617264 496d706c 44314576 005f5a4e uardImplD1Ev._ZN
-  0x00008de0 33633130 36495661 6c756537 64657374 3c106IValue7dest
-  0x00008df0 726f7945 76005f5a 4e336331 30313153 royEv._ZN3c1011S
-  0x00008e00 796d4e6f 6465496d 706c3373 75624552 ymNodeImpl3subER
-  0x00008e10 4b4e535f 3133696e 74727573 6976655f KNS_13intrusive_
-  0x00008e20 70747249 53305f4e 535f3664 65746169 ptrIS0_NS_6detai
-  0x00008e30 6c333469 6e747275 73697665 5f746172 l34intrusive_tar
-  0x00008e40 6765745f 64656661 756c745f 6e756c6c get_default_null
-  0x00008e50 5f747970 65495330 5f454545 45005079 _typeIS0_EEEE.Py
-  0x00008e60 47494c53 74617465 5f52656c 65617365 GILState_Release
-  0x00008e70 005f5a4e 33633130 31344469 73706174 ._ZN3c1014Dispat
-  0x00008e80 63684b65 79536574 4331454e 535f3131 chKeySetC1ENS_11
-  0x00008e90 44697370 61746368 4b657945 00637564 DispatchKeyE.cud
-  0x00008ea0 61457665 6e74456c 61707365 6454696d aEventElapsedTim
-  0x00008eb0 65406c69 62637564 6172742e 736f2e31 e@libcudart.so.1
-  0x00008ec0 32005f5a 4e537370 4c45504b 6340474c 2._ZNSspLEPKc@GL
-  0x00008ed0 49424358 585f332e 34005f5a 4e336331 IBCXX_3.4._ZN3c1
-  0x00008ee0 30313153 796d4e6f 6465496d 706c3463 011SymNodeImpl4c
-  0x00008ef0 65696c45 76005f5a 54564e33 63313034 eilEv._ZTVN3c104
-  0x00008f00 696d706c 36646574 61696c33 31577261 impl6detail31Wra
-  0x00008f10 7046756e 6374696f 6e496e74 6f52756e pFunctionIntoRun
-  0x00008f20 74696d65 46756e63 746f725f 4950464e timeFunctor_IPFN
-  0x00008f30 32617436 54656e73 6f724553 345f5334 2at6TensorES4_S4
-  0x00008f40 5f455334 5f4e535f 34677574 73387479 _ES4_NS_4guts8ty
-  0x00008f50 70656c69 73743874 7970656c 69737449 pelist8typelistI
-  0x00008f60 4a53345f 53345f45 45454545 005f5079 JS4_S4_EEEEE._Py
-  0x00008f70 5f4e6f74 496d706c 656d656e 74656453 _NotImplementedS
-  0x00008f80 74727563 74005f5a 4e537438 696f735f truct._ZNSt8ios_
-  0x00008f90 62617365 44324576 40474c49 42435858 baseD2Ev@GLIBCXX
-  0x00008fa0 5f332e34 005f5a4e 4b336331 3034696d _3.4._ZNK3c104im
-  0x00008fb0 706c3136 56697274 75616c47 75617264 pl16VirtualGuard
-  0x00008fc0 496d706c 36726563 6f726445 50507652 Impl6recordEPPvR
-  0x00008fd0 4b4e535f 36537472 65616d45 614e535f KNS_6StreamEaNS_
-  0x00008fe0 39457665 6e74466c 61674500 5f5a4e33 9EventFlagE._ZN3
-  0x00008ff0 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
-  0x00009000 31316578 70656374 5f747275 6545504b 11expect_trueEPK
-  0x00009010 636c005f 5a4e5373 36696e73 65727445 cl._ZNSs6insertE
-  0x00009020 6d504b63 6d40474c 49424358 585f332e mPKcm@GLIBCXX_3.
-  0x00009030 34005f5a 33314578 74726163 745f325f 4._Z31Extract_2_
-  0x00009040 42697473 5f46726f 6d5f345f 50616464 Bits_From_4_Padd
-  0x00009050 65644650 36686868 68005f5a 32354465 edFP6hhhh._Z25De
-  0x00009060 5175616e 744d6174 7269785f 4650365f QuantMatrix_FP6_
-  0x00009070 546f5f46 50313650 365f5f68 616c6650 To_FP16P6__halfP
-  0x00009080 686d6d53 305f005f 5a4e3363 31303131 hmmS0_._ZN3c1011
-  0x00009090 53796d4e 6f646549 6d706c31 31657870 SymNodeImpl11exp
-  0x000090a0 6563745f 73697a65 45504b63 6c005f5a ect_sizeEPKcl._Z
-  0x000090b0 4e4b3261 74313054 656e736f 72426173 NK2at10TensorBas
-  0x000090c0 65386461 74615f70 74724966 45455054 e8data_ptrIfEEPT
-  0x000090d0 5f76005f 5a4e3363 31303469 6d706c36 _v._ZN3c104impl6
-  0x000090e0 64657461 696c3331 57726170 46756e63 detail31WrapFunc
-  0x000090f0 74696f6e 496e746f 52756e74 696d6546 tionIntoRuntimeF
-  0x00009100 756e6374 6f725f49 50464e32 61743654 unctor_IPFN2at6T
-  0x00009110 656e736f 72455334 5f53345f 4553345f ensorES4_S4_ES4_
-  0x00009120 4e535f34 67757473 38747970 656c6973 NS_4guts8typelis
-  0x00009130 74387479 70656c69 7374494a 53345f53 t8typelistIJS4_S
-  0x00009140 345f4545 45454432 4576005f 5a4e3261 4_EEEED2Ev._ZN2a
-  0x00009150 74345f6f 70733130 656d7074 795f6c69 t4_ops10empty_li
-  0x00009160 6b653463 616c6c45 524b4e53 5f365465 ke4callERKNS_6Te
-  0x00009170 6e736f72 45537438 6f707469 6f6e616c nsorESt8optional
-  0x00009180 494e3363 31303130 5363616c 61725479 IN3c1010ScalarTy
-  0x00009190 70654545 53355f49 4e53365f 364c6179 peEES5_INS6_6Lay
-  0x000091a0 6f757445 4553355f 494e5336 5f364465 outEES5_INS6_6De
-  0x000091b0 76696365 45455335 5f496245 53355f49 viceEES5_IbES5_I
-  0x000091c0 4e53365f 31324d65 6d6f7279 466f726d NS6_12MemoryForm
-  0x000091d0 61744545 005f5a4e 5373345f 52657039 atEE._ZNSs4_Rep9
-  0x000091e0 5f535f63 72656174 65456d6d 524b5361 _S_createEmmRKSa
-  0x000091f0 49634540 474c4942 4358585f 332e3400 IcE@GLIBCXX_3.4.
-  0x00009200 50794f62 6a656374 5f536574 4974656d PyObject_SetItem
-  0x00009210 005f5a4e 4b336331 30346375 64613469 ._ZNK3c104cuda4i
-  0x00009220 6d706c31 33435544 41477561 7264496d mpl13CUDAGuardIm
-  0x00009230 706c3231 7265636f 72644461 74615074 pl21recordDataPt
-  0x00009240 724f6e53 74726561 6d45524b 4e535f37 rOnStreamERKNS_7
-  0x00009250 44617461 50747245 524b4e53 5f365374 DataPtrERKNS_6St
-  0x00009260 7265616d 45005f5a 54494e33 63313034 reamE._ZTIN3c104
-  0x00009270 696d706c 36646574 61696c33 31577261 impl6detail31Wra
-  0x00009280 7046756e 6374696f 6e496e74 6f52756e pFunctionIntoRun
-  0x00009290 74696d65 46756e63 746f725f 4950464e timeFunctor_IPFN
-  0x000092a0 32617436 54656e73 6f724552 4b53345f 2at6TensorERKS4_
-  0x000092b0 53365f64 4553345f 4e535f34 67757473 S6_dES4_NS_4guts
-  0x000092c0 38747970 656c6973 74387479 70656c69 8typelist8typeli
-  0x000092d0 7374494a 53365f53 365f6445 45454545 stIJS6_S6_dEEEEE
-  0x000092e0 00507945 78635f53 79737465 6d457272 .PyExc_SystemErr
-  0x000092f0 6f72005f 5a4e3574 6f726368 374c6962 or._ZN5torch7Lib
-  0x00009300 72617279 44324576 005f5a4e 33633130 raryD2Ev._ZN3c10
-  0x00009310 36646574 61696c33 30696e66 65724675 6detail30inferFu
-  0x00009320 6e637469 6f6e5363 68656d61 46726f6d nctionSchemaFrom
-  0x00009330 46756e63 746f7249 50464e32 61743654 FunctorIPFN2at6T
-  0x00009340 656e736f 72455333 5f53335f 53335f6c ensorES3_S3_S3_l
-  0x00009350 45454553 74313075 6e697175 655f7074 EEESt10unique_pt
-  0x00009360 72494e53 5f313446 756e6374 696f6e53 rINS_14FunctionS
-  0x00009370 6368656d 61455374 31346465 6661756c chemaESt14defaul
-  0x00009380 745f6465 6c657465 4953375f 45457600 t_deleteIS7_EEv.
-  0x00009390 5f5a4e53 74366c6f 63616c65 43314576 _ZNSt6localeC1Ev
-  0x000093a0 40474c49 42435858 5f332e34 005f5a4e @GLIBCXX_3.4._ZN
-  0x000093b0 53743676 6563746f 72496853 61496845 St6vectorIhSaIhE
-  0x000093c0 4531375f 4d5f7265 616c6c6f 635f696e E17_M_realloc_in
-  0x000093d0 73657274 494a524b 68454545 764e395f sertIJRKhEEEvN9_
-  0x000093e0 5f676e75 5f637878 31375f5f 6e6f726d _gnu_cxx17__norm
-  0x000093f0 616c5f69 74657261 746f7249 50685331 al_iteratorIPhS1
-  0x00009400 5f454544 704f545f 005f5a4e 53743676 _EEDpOT_._ZNSt6v
-  0x00009410 6563746f 72494e33 63313038 41726775 ectorIN3c108Argu
-  0x00009420 6d656e74 45536149 53315f45 45443145 mentESaIS1_EED1E
-  0x00009430 76005f5a 4e336331 306e6545 524b4e53 v._ZN3c10neERKNS
-  0x00009440 5f365379 6d496e74 4569005f 5a4e3363 _6SymIntEi._ZN3c
-  0x00009450 31303133 696e7472 75736976 655f7074 1013intrusive_pt
-  0x00009460 72494e53 5f313556 61726961 626c6556 rINS_15VariableV
-  0x00009470 65727369 6f6e3134 56657273 696f6e43 ersion14VersionC
-  0x00009480 6f756e74 6572454e 535f3664 65746169 ounterENS_6detai
-  0x00009490 6c333469 6e747275 73697665 5f746172 l34intrusive_tar
-  0x000094a0 6765745f 64656661 756c745f 6e756c6c get_default_null
-  0x000094b0 5f747970 65495332 5f454545 43314550 _typeIS2_EEEC1EP
-  0x000094c0 53325f00 5f5a4e33 63313031 3153796d S2_._ZN3c1011Sym
-  0x000094d0 4e6f6465 496d706c 336e6567 45760050 NodeImpl3negEv.P
-  0x000094e0 79436170 73756c65 5f547970 65005f5f yCapsule_Type.__
-  0x000094f0 6378615f 656e645f 63617463 68404358 cxa_end_catch@CX
-  0x00009500 58414249 5f312e33 005f5a4e 33633130 XABI_1.3._ZN3c10
-  0x00009510 31386765 7446616b 65547970 65507472 18getFakeTypePtr
-  0x00009520 436f7079 49644545 4e535f34 54797065 CopyIdEENS_4Type
-  0x00009530 32345369 6e676c65 746f6e4f 72536861 24SingletonOrSha
-  0x00009540 72656454 79706550 74724953 315f4545 redTypePtrIS1_EE
-  0x00009550 76005f5a 33314578 74726163 745f345f v._Z31Extract_4_
-  0x00009560 42697473 5f46726f 6d5f325f 50616464 Bits_From_2_Padd
-  0x00009570 65644650 36686800 5f5a4e53 74313962 edFP6hh._ZNSt19b
-  0x00009580 61645f6f 7074696f 6e616c5f 61636365 ad_optional_acce
-  0x00009590 73734432 45760073 7472636d 7040474c ssD2Ev.strcmp@GL
-  0x000095a0 4942435f 322e322e 35005f5a 4e336331 IBC_2.2.5._ZN3c1
-  0x000095b0 30346375 64613953 65744465 76696365 04cuda9SetDevice
-  0x000095c0 4561005f 5f637861 5f726574 68726f77 Ea.__cxa_rethrow
-  0x000095d0 40435858 4142495f 312e3300 5f5a4e33 @CXXABI_1.3._ZN3
-  0x000095e0 63313032 30696e74 72757369 76655f70 c1020intrusive_p
-  0x000095f0 74725f74 61726765 74443245 76005f5a tr_targetD2Ev._Z
-  0x00009600 32354173 7369676e 5f33325f 4650365f 25Assign_32_FP6_
-  0x00009610 546f5f34 5f546872 65616450 53743676 To_4_ThreadPSt6v
-  0x00009620 6563746f 72496853 61496845 4553325f ectorIhSaIhEES2_
-  0x00009630 50685333 5f53335f 53335f00 5f5a4e53 PhS3_S3_S3_._ZNS
-  0x00009640 74367665 63746f72 49506353 61495330 t6vectorIPcSaIS0
-  0x00009650 5f454531 375f4d5f 7265616c 6c6f635f _EE17_M_realloc_
-  0x00009660 696e7365 7274494a 524b5330 5f454545 insertIJRKS0_EEE
-  0x00009670 764e395f 5f676e75 5f637878 31375f5f vN9__gnu_cxx17__
-  0x00009680 6e6f726d 616c5f69 74657261 746f7249 normal_iteratorI
-  0x00009690 5053305f 53325f45 4544704f 545f005f PS0_S2_EEDpOT_._
-  0x000096a0 5a4e5374 31337275 6e74696d 655f6572 ZNSt13runtime_er
-  0x000096b0 726f7244 31457640 474c4942 4358585f rorD1Ev@GLIBCXX_
-  0x000096c0 332e3400 5f5a4e4b 53733466 696e6445 3.4._ZNKSs4findE
-  0x000096d0 504b636d 6d40474c 49424358 585f332e PKcmm@GLIBCXX_3.
-  0x000096e0 34005f5a 4e336331 3034696d 706c3334 4._ZN3c104impl34
-  0x000096f0 63616c6c 5f66756e 63746f72 5f776974 call_functor_wit
-  0x00009700 685f6172 67735f66 726f6d5f 73746163 h_args_from_stac
-  0x00009710 6b5f494e 53305f36 64657461 696c3331 k_INS0_6detail31
-  0x00009720 57726170 46756e63 74696f6e 496e746f WrapFunctionInto
-  0x00009730 52756e74 696d6546 756e6374 6f725f49 RuntimeFunctor_I
-  0x00009740 50464e32 61743654 656e736f 72455335 PFN2at6TensorES5
-  0x00009750 5f53355f 53355f6c 4553355f 4e535f34 _S5_S5_lES5_NS_4
-  0x00009760 67757473 38747970 656c6973 74387479 guts8typelist8ty
-  0x00009770 70656c69 7374494a 53355f53 355f5335 pelistIJS5_S5_S5
-  0x00009780 5f6c4545 4545454c 6230454a 4c6d3045 _lEEEEELb0EJLm0E
-  0x00009790 4c6d3145 4c6d3245 4c6d3345 454a5335 Lm1ELm2ELm3EEJS5
-  0x000097a0 5f53355f 53355f6c 4545454e 53743564 _S5_S5_lEEENSt5d
-  0x000097b0 65636179 494e5338 5f323169 6e666572 ecayINS8_21infer
-  0x000097c0 5f66756e 6374696f 6e5f7472 61697473 _function_traits
-  0x000097d0 49545f45 34747970 65313172 65747572 IT_E4type11retur
-  0x000097e0 6e5f7479 70654545 34747970 6545504e n_typeEE4typeEPN
-  0x000097f0 535f3134 4f706572 61746f72 4b65726e S_14OperatorKern
-  0x00009800 656c454e 535f3134 44697370 61746368 elENS_14Dispatch
-  0x00009810 4b657953 65744550 53743676 6563746f KeySetEPSt6vecto
-  0x00009820 72494e53 5f364956 616c7565 45536149 rINS_6IValueESaI
-  0x00009830 53505f45 45537431 36696e74 65676572 SP_EESt16integer
-  0x00009840 5f736571 75656e63 65496d4a 58737054 _sequenceImJXspT
-  0x00009850 315f4545 45504e53 415f494a 44705432 1_EEEPNSA_IJDpT2
-  0x00009860 5f454545 005f5f63 75646152 65676973 _EEE.__cudaRegis
-  0x00009870 74657246 756e6374 696f6e40 6c696263 terFunction@libc
-  0x00009880 75646172 742e736f 2e313200 5f5a4e53 udart.so.12._ZNS
-  0x00009890 74367665 63746f72 494e3363 31303941 t6vectorIN3c109A
-  0x000098a0 6c696173 496e666f 45536149 53315f45 liasInfoESaIS1_E
-  0x000098b0 45443145 76005f5a 54534e33 63313034 ED1Ev._ZTSN3c104
-  0x000098c0 63756461 34696d70 6c313343 55444147 cuda4impl13CUDAG
-  0x000098d0 75617264 496d706c 45005f5a 4e336331 uardImplE._ZN3c1
-  0x000098e0 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
-  0x000098f0 75617264 496d706c 44324576 005f5a4e uardImplD2Ev._ZN
-  0x00009900 33633130 36646574 61696c33 30696e66 3c106detail30inf
-  0x00009910 65724675 6e637469 6f6e5363 68656d61 erFunctionSchema
-  0x00009920 46726f6d 46756e63 746f7249 50464e32 FromFunctorIPFN2
-  0x00009930 61743654 656e736f 72455333 5f454545 at6TensorES3_EEE
-  0x00009940 53743130 756e6971 75655f70 7472494e St10unique_ptrIN
-  0x00009950 535f3134 46756e63 74696f6e 53636865 S_14FunctionSche
-  0x00009960 6d614553 74313464 65666175 6c745f64 maESt14default_d
-  0x00009970 656c6574 65495337 5f454576 005f5a4e eleteIS7_EEv._ZN
-  0x00009980 33633130 37496e74 54797065 33676574 3c107IntType3get
-  0x00009990 4576005f 5a4e3363 31303131 53796d4e Ev._ZN3c1011SymN
-  0x000099a0 6f646549 6d706c32 65714552 4b4e535f odeImpl2eqERKNS_
-  0x000099b0 3133696e 74727573 6976655f 70747249 13intrusive_ptrI
-  0x000099c0 53305f4e 535f3664 65746169 6c333469 S0_NS_6detail34i
-  0x000099d0 6e747275 73697665 5f746172 6765745f ntrusive_target_
-  0x000099e0 64656661 756c745f 6e756c6c 5f747970 default_null_typ
-  0x000099f0 65495330 5f454545 45005079 4672616d eIS0_EEEE.PyFram
-  0x00009a00 655f4765 74426163 6b005f5a 4e37746f e_GetBack._ZN7to
-  0x00009a10 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
-  0x00009a20 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x00009a30 735f6375 5f316231 64376430 655f3232 s_cu_1b1d7d0e_22
-  0x00009a40 30303130 6e6d735f 6b65726e 656c4552 0010nms_kernelER
-  0x00009a50 4b4e3261 74365465 6e736f72 4553345f KN2at6TensorES4_
-  0x00009a60 64005f5f 63756461 506f7043 616c6c43 d.__cudaPopCallC
+  0x00008ba0 58414249 5f312e33 005f5a4e 37746f72 XABI_1.3._ZN7tor
+  0x00008bb0 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
+  0x00008bc0 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
+  0x00008bd0 5f63755f 31356239 35653931 5f323538 _cu_15b95e91_258
+  0x00008be0 3631306e 6d735f6b 65726e65 6c45524b 610nms_kernelERK
+  0x00008bf0 4e326174 3654656e 736f7245 53345f64 N2at6TensorES4_d
+  0x00008c00 005f5a4e 4b336331 3034696d 706c3136 ._ZNK3c104impl16
+  0x00008c10 56697274 75616c47 75617264 496d706c VirtualGuardImpl
+  0x00008c20 34747970 65457600 5f5a4e33 63313031 4typeEv._ZN3c101
+  0x00008c30 3153796d 4e6f6465 496d706c 38777261 1SymNodeImpl8wra
+  0x00008c40 705f696e 74456c00 5f5a4e33 63313031 p_intEl._ZN3c101
+  0x00008c50 3153796d 4e6f6465 496d706c 44314576 1SymNodeImplD1Ev
+  0x00008c60 005f5a4e 33633130 34696d70 6c33316d ._ZN3c104impl31m
+  0x00008c70 616b655f 626f7865 645f6672 6f6d5f75 ake_boxed_from_u
+  0x00008c80 6e626f78 65645f66 756e6374 6f72494e nboxed_functorIN
+  0x00008c90 53305f36 64657461 696c3331 57726170 S0_6detail31Wrap
+  0x00008ca0 46756e63 74696f6e 496e746f 52756e74 FunctionIntoRunt
+  0x00008cb0 696d6546 756e6374 6f725f49 50464e32 imeFunctor_IPFN2
+  0x00008cc0 61743654 656e736f 72455335 5f53355f at6TensorES5_S5_
+  0x00008cd0 4553355f 4e535f34 67757473 38747970 ES5_NS_4guts8typ
+  0x00008ce0 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x00008cf0 53355f53 355f4545 4545454c 62304545 S5_S5_EEEEELb0EE
+  0x00008d00 3463616c 6c45504e 535f3134 4f706572 4callEPNS_14Oper
+  0x00008d10 61746f72 4b65726e 656c4552 4b4e535f atorKernelERKNS_
+  0x00008d20 31344f70 65726174 6f724861 6e646c65 14OperatorHandle
+  0x00008d30 454e535f 31344469 73706174 63684b65 ENS_14DispatchKe
+  0x00008d40 79536574 45505374 36766563 746f7249 ySetEPSt6vectorI
+  0x00008d50 4e535f36 4956616c 75654553 6149534c NS_6IValueESaISL
+  0x00008d60 5f454500 5f5a4e4b 33633130 34637564 _EE._ZNK3c104cud
+  0x00008d70 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
+  0x00008d80 64496d70 6c313267 65744e65 77537472 dImpl12getNewStr
+  0x00008d90 65616d45 4e535f36 44657669 63654569 eamENS_6DeviceEi
+  0x00008da0 00507944 6963745f 4e657700 5f5a4e33 .PyDict_New._ZN3
+  0x00008db0 63313031 35566172 6961626c 65566572 c1015VariableVer
+  0x00008dc0 73696f6e 31345665 7273696f 6e436f75 sion14VersionCou
+  0x00008dd0 6e746572 44324576 00507943 61707375 nterD2Ev.PyCapsu
+  0x00008de0 6c655f53 6574506f 696e7465 72005f5a le_SetPointer._Z
+  0x00008df0 4e537438 696f735f 62617365 34496e69 NSt8ios_base4Ini
+  0x00008e00 74443145 7640474c 49424358 585f332e tD1Ev@GLIBCXX_3.
+  0x00008e10 34005f5a 4e336331 3034696d 706c3136 4._ZN3c104impl16
+  0x00008e20 56697274 75616c47 75617264 496d706c VirtualGuardImpl
+  0x00008e30 44314576 005f5a4e 33633130 36495661 D1Ev._ZN3c106IVa
+  0x00008e40 6c756537 64657374 726f7945 76005f5a lue7destroyEv._Z
+  0x00008e50 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
+  0x00008e60 706c3373 75624552 4b4e535f 3133696e pl3subERKNS_13in
+  0x00008e70 74727573 6976655f 70747249 53305f4e trusive_ptrIS0_N
+  0x00008e80 535f3664 65746169 6c333469 6e747275 S_6detail34intru
+  0x00008e90 73697665 5f746172 6765745f 64656661 sive_target_defa
+  0x00008ea0 756c745f 6e756c6c 5f747970 65495330 ult_null_typeIS0
+  0x00008eb0 5f454545 45005079 47494c53 74617465 _EEEE.PyGILState
+  0x00008ec0 5f52656c 65617365 005f5a4e 33633130 _Release._ZN3c10
+  0x00008ed0 31344469 73706174 63684b65 79536574 14DispatchKeySet
+  0x00008ee0 4331454e 535f3131 44697370 61746368 C1ENS_11Dispatch
+  0x00008ef0 4b657945 00637564 61457665 6e74456c KeyE.cudaEventEl
+  0x00008f00 61707365 6454696d 65406c69 62637564 apsedTime@libcud
+  0x00008f10 6172742e 736f2e31 32005f5a 4e537370 art.so.12._ZNSsp
+  0x00008f20 4c45504b 6340474c 49424358 585f332e LEPKc@GLIBCXX_3.
+  0x00008f30 34005f5a 4e336331 30313153 796d4e6f 4._ZN3c1011SymNo
+  0x00008f40 6465496d 706c3463 65696c45 76005f5a deImpl4ceilEv._Z
+  0x00008f50 54564e33 63313034 696d706c 36646574 TVN3c104impl6det
+  0x00008f60 61696c33 31577261 7046756e 6374696f ail31WrapFunctio
+  0x00008f70 6e496e74 6f52756e 74696d65 46756e63 nIntoRuntimeFunc
+  0x00008f80 746f725f 4950464e 32617436 54656e73 tor_IPFN2at6Tens
+  0x00008f90 6f724553 345f5334 5f455334 5f4e535f orES4_S4_ES4_NS_
+  0x00008fa0 34677574 73387479 70656c69 73743874 4guts8typelist8t
+  0x00008fb0 7970656c 69737449 4a53345f 53345f45 ypelistIJS4_S4_E
+  0x00008fc0 45454545 005f5079 5f4e6f74 496d706c EEEE._Py_NotImpl
+  0x00008fd0 656d656e 74656453 74727563 74005f5a ementedStruct._Z
+  0x00008fe0 4e537438 696f735f 62617365 44324576 NSt8ios_baseD2Ev
+  0x00008ff0 40474c49 42435858 5f332e34 005f5a4e @GLIBCXX_3.4._ZN
+  0x00009000 4b336331 3034696d 706c3136 56697274 K3c104impl16Virt
+  0x00009010 75616c47 75617264 496d706c 36726563 ualGuardImpl6rec
+  0x00009020 6f726445 50507652 4b4e535f 36537472 ordEPPvRKNS_6Str
+  0x00009030 65616d45 614e535f 39457665 6e74466c eamEaNS_9EventFl
+  0x00009040 61674500 5f5a4e33 63313031 3153796d agE._ZN3c1011Sym
+  0x00009050 4e6f6465 496d706c 31316578 70656374 NodeImpl11expect
+  0x00009060 5f747275 6545504b 636c005f 5a4e5373 _trueEPKcl._ZNSs
+  0x00009070 36696e73 65727445 6d504b63 6d40474c 6insertEmPKcm@GL
+  0x00009080 49424358 585f332e 34005f5a 33314578 IBCXX_3.4._Z31Ex
+  0x00009090 74726163 745f325f 42697473 5f46726f tract_2_Bits_Fro
+  0x000090a0 6d5f345f 50616464 65644650 36686868 m_4_PaddedFP6hhh
+  0x000090b0 68005f5a 32354465 5175616e 744d6174 h._Z25DeQuantMat
+  0x000090c0 7269785f 4650365f 546f5f46 50313650 rix_FP6_To_FP16P
+  0x000090d0 365f5f68 616c6650 686d6d53 305f005f 6__halfPhmmS0_._
+  0x000090e0 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
+  0x000090f0 6d706c31 31657870 6563745f 73697a65 mpl11expect_size
+  0x00009100 45504b63 6c005f5a 4e4b3261 74313054 EPKcl._ZNK2at10T
+  0x00009110 656e736f 72426173 65386461 74615f70 ensorBase8data_p
+  0x00009120 74724966 45455054 5f76005f 5a4e3363 trIfEEPT_v._ZN3c
+  0x00009130 31303469 6d706c36 64657461 696c3331 104impl6detail31
+  0x00009140 57726170 46756e63 74696f6e 496e746f WrapFunctionInto
+  0x00009150 52756e74 696d6546 756e6374 6f725f49 RuntimeFunctor_I
+  0x00009160 50464e32 61743654 656e736f 72455334 PFN2at6TensorES4
+  0x00009170 5f53345f 4553345f 4e535f34 67757473 _S4_ES4_NS_4guts
+  0x00009180 38747970 656c6973 74387479 70656c69 8typelist8typeli
+  0x00009190 7374494a 53345f53 345f4545 45454432 stIJS4_S4_EEEED2
+  0x000091a0 4576005f 5a4e3261 74345f6f 70733130 Ev._ZN2at4_ops10
+  0x000091b0 656d7074 795f6c69 6b653463 616c6c45 empty_like4callE
+  0x000091c0 524b4e53 5f365465 6e736f72 45537438 RKNS_6TensorESt8
+  0x000091d0 6f707469 6f6e616c 494e3363 31303130 optionalIN3c1010
+  0x000091e0 5363616c 61725479 70654545 53355f49 ScalarTypeEES5_I
+  0x000091f0 4e53365f 364c6179 6f757445 4553355f NS6_6LayoutEES5_
+  0x00009200 494e5336 5f364465 76696365 45455335 INS6_6DeviceEES5
+  0x00009210 5f496245 53355f49 4e53365f 31324d65 _IbES5_INS6_12Me
+  0x00009220 6d6f7279 466f726d 61744545 005f5a4e moryFormatEE._ZN
+  0x00009230 5373345f 52657039 5f535f63 72656174 Ss4_Rep9_S_creat
+  0x00009240 65456d6d 524b5361 49634540 474c4942 eEmmRKSaIcE@GLIB
+  0x00009250 4358585f 332e3400 50794f62 6a656374 CXX_3.4.PyObject
+  0x00009260 5f536574 4974656d 005f5a4e 4b336331 _SetItem._ZNK3c1
+  0x00009270 30346375 64613469 6d706c31 33435544 04cuda4impl13CUD
+  0x00009280 41477561 7264496d 706c3231 7265636f AGuardImpl21reco
+  0x00009290 72644461 74615074 724f6e53 74726561 rdDataPtrOnStrea
+  0x000092a0 6d45524b 4e535f37 44617461 50747245 mERKNS_7DataPtrE
+  0x000092b0 524b4e53 5f365374 7265616d 45005f5a RKNS_6StreamE._Z
+  0x000092c0 54494e33 63313034 696d706c 36646574 TIN3c104impl6det
+  0x000092d0 61696c33 31577261 7046756e 6374696f ail31WrapFunctio
+  0x000092e0 6e496e74 6f52756e 74696d65 46756e63 nIntoRuntimeFunc
+  0x000092f0 746f725f 4950464e 32617436 54656e73 tor_IPFN2at6Tens
+  0x00009300 6f724552 4b53345f 53365f64 4553345f orERKS4_S6_dES4_
+  0x00009310 4e535f34 67757473 38747970 656c6973 NS_4guts8typelis
+  0x00009320 74387479 70656c69 7374494a 53365f53 t8typelistIJS6_S
+  0x00009330 365f6445 45454545 00507945 78635f53 6_dEEEEE.PyExc_S
+  0x00009340 79737465 6d457272 6f72005f 5a4e3574 ystemError._ZN5t
+  0x00009350 6f726368 374c6962 72617279 44324576 orch7LibraryD2Ev
+  0x00009360 005f5a4e 33633130 36646574 61696c33 ._ZN3c106detail3
+  0x00009370 30696e66 65724675 6e637469 6f6e5363 0inferFunctionSc
+  0x00009380 68656d61 46726f6d 46756e63 746f7249 hemaFromFunctorI
+  0x00009390 50464e32 61743654 656e736f 72455333 PFN2at6TensorES3
+  0x000093a0 5f53335f 53335f6c 45454553 74313075 _S3_S3_lEEESt10u
+  0x000093b0 6e697175 655f7074 72494e53 5f313446 nique_ptrINS_14F
+  0x000093c0 756e6374 696f6e53 6368656d 61455374 unctionSchemaESt
+  0x000093d0 31346465 6661756c 745f6465 6c657465 14default_delete
+  0x000093e0 4953375f 45457600 5f5a4e53 74366c6f IS7_EEv._ZNSt6lo
+  0x000093f0 63616c65 43314576 40474c49 42435858 caleC1Ev@GLIBCXX
+  0x00009400 5f332e34 005f5a4e 53743676 6563746f _3.4._ZNSt6vecto
+  0x00009410 72496853 61496845 4531375f 4d5f7265 rIhSaIhEE17_M_re
+  0x00009420 616c6c6f 635f696e 73657274 494a524b alloc_insertIJRK
+  0x00009430 68454545 764e395f 5f676e75 5f637878 hEEEvN9__gnu_cxx
+  0x00009440 31375f5f 6e6f726d 616c5f69 74657261 17__normal_itera
+  0x00009450 746f7249 50685331 5f454544 704f545f torIPhS1_EEDpOT_
+  0x00009460 005f5a4e 53743676 6563746f 72494e33 ._ZNSt6vectorIN3
+  0x00009470 63313038 41726775 6d656e74 45536149 c108ArgumentESaI
+  0x00009480 53315f45 45443145 76005f5a 4e336331 S1_EED1Ev._ZN3c1
+  0x00009490 306e6545 524b4e53 5f365379 6d496e74 0neERKNS_6SymInt
+  0x000094a0 4569005f 5a4e3363 31303133 696e7472 Ei._ZN3c1013intr
+  0x000094b0 75736976 655f7074 72494e53 5f313556 usive_ptrINS_15V
+  0x000094c0 61726961 626c6556 65727369 6f6e3134 ariableVersion14
+  0x000094d0 56657273 696f6e43 6f756e74 6572454e VersionCounterEN
+  0x000094e0 535f3664 65746169 6c333469 6e747275 S_6detail34intru
+  0x000094f0 73697665 5f746172 6765745f 64656661 sive_target_defa
+  0x00009500 756c745f 6e756c6c 5f747970 65495332 ult_null_typeIS2
+  0x00009510 5f454545 43314550 53325f00 5f5a4e33 _EEEC1EPS2_._ZN3
+  0x00009520 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
+  0x00009530 336e6567 45760050 79436170 73756c65 3negEv.PyCapsule
+  0x00009540 5f547970 65005f5f 6378615f 656e645f _Type.__cxa_end_
+  0x00009550 63617463 68404358 58414249 5f312e33 catch@CXXABI_1.3
+  0x00009560 005f5a4e 33633130 31386765 7446616b ._ZN3c1018getFak
+  0x00009570 65547970 65507472 436f7079 49644545 eTypePtrCopyIdEE
+  0x00009580 4e535f34 54797065 32345369 6e676c65 NS_4Type24Single
+  0x00009590 746f6e4f 72536861 72656454 79706550 tonOrSharedTypeP
+  0x000095a0 74724953 315f4545 76005f5a 33314578 trIS1_EEv._Z31Ex
+  0x000095b0 74726163 745f345f 42697473 5f46726f tract_4_Bits_Fro
+  0x000095c0 6d5f325f 50616464 65644650 36686800 m_2_PaddedFP6hh.
+  0x000095d0 5f5a4e53 74313962 61645f6f 7074696f _ZNSt19bad_optio
+  0x000095e0 6e616c5f 61636365 73734432 45760073 nal_accessD2Ev.s
+  0x000095f0 7472636d 7040474c 4942435f 322e322e trcmp@GLIBC_2.2.
+  0x00009600 35005f5a 4e336331 30346375 64613953 5._ZN3c104cuda9S
+  0x00009610 65744465 76696365 4561005f 5f637861 etDeviceEa.__cxa
+  0x00009620 5f726574 68726f77 40435858 4142495f _rethrow@CXXABI_
+  0x00009630 312e3300 5f5a4e33 63313032 30696e74 1.3._ZN3c1020int
+  0x00009640 72757369 76655f70 74725f74 61726765 rusive_ptr_targe
+  0x00009650 74443245 76005f5a 32354173 7369676e tD2Ev._Z25Assign
+  0x00009660 5f33325f 4650365f 546f5f34 5f546872 _32_FP6_To_4_Thr
+  0x00009670 65616450 53743676 6563746f 72496853 eadPSt6vectorIhS
+  0x00009680 61496845 4553325f 50685333 5f53335f aIhEES2_PhS3_S3_
+  0x00009690 53335f00 5f5a4e53 74367665 63746f72 S3_._ZNSt6vector
+  0x000096a0 49506353 61495330 5f454531 375f4d5f IPcSaIS0_EE17_M_
+  0x000096b0 7265616c 6c6f635f 696e7365 7274494a realloc_insertIJ
+  0x000096c0 524b5330 5f454545 764e395f 5f676e75 RKS0_EEEvN9__gnu
+  0x000096d0 5f637878 31375f5f 6e6f726d 616c5f69 _cxx17__normal_i
+  0x000096e0 74657261 746f7249 5053305f 53325f45 teratorIPS0_S2_E
+  0x000096f0 4544704f 545f005f 5a4e5374 31337275 EDpOT_._ZNSt13ru
+  0x00009700 6e74696d 655f6572 726f7244 31457640 ntime_errorD1Ev@
+  0x00009710 474c4942 4358585f 332e3400 5f5a4e4b GLIBCXX_3.4._ZNK
+  0x00009720 53733466 696e6445 504b636d 6d40474c Ss4findEPKcmm@GL
+  0x00009730 49424358 585f332e 34005f5a 4e336331 IBCXX_3.4._ZN3c1
+  0x00009740 3034696d 706c3334 63616c6c 5f66756e 04impl34call_fun
+  0x00009750 63746f72 5f776974 685f6172 67735f66 ctor_with_args_f
+  0x00009760 726f6d5f 73746163 6b5f494e 53305f36 rom_stack_INS0_6
+  0x00009770 64657461 696c3331 57726170 46756e63 detail31WrapFunc
+  0x00009780 74696f6e 496e746f 52756e74 696d6546 tionIntoRuntimeF
+  0x00009790 756e6374 6f725f49 50464e32 61743654 unctor_IPFN2at6T
+  0x000097a0 656e736f 72455335 5f53355f 53355f6c ensorES5_S5_S5_l
+  0x000097b0 4553355f 4e535f34 67757473 38747970 ES5_NS_4guts8typ
+  0x000097c0 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x000097d0 53355f53 355f5335 5f6c4545 4545454c S5_S5_S5_lEEEEEL
+  0x000097e0 6230454a 4c6d3045 4c6d3145 4c6d3245 b0EJLm0ELm1ELm2E
+  0x000097f0 4c6d3345 454a5335 5f53355f 53355f6c Lm3EEJS5_S5_S5_l
+  0x00009800 4545454e 53743564 65636179 494e5338 EEENSt5decayINS8
+  0x00009810 5f323169 6e666572 5f66756e 6374696f _21infer_functio
+  0x00009820 6e5f7472 61697473 49545f45 34747970 n_traitsIT_E4typ
+  0x00009830 65313172 65747572 6e5f7479 70654545 e11return_typeEE
+  0x00009840 34747970 6545504e 535f3134 4f706572 4typeEPNS_14Oper
+  0x00009850 61746f72 4b65726e 656c454e 535f3134 atorKernelENS_14
+  0x00009860 44697370 61746368 4b657953 65744550 DispatchKeySetEP
+  0x00009870 53743676 6563746f 72494e53 5f364956 St6vectorINS_6IV
+  0x00009880 616c7565 45536149 53505f45 45537431 alueESaISP_EESt1
+  0x00009890 36696e74 65676572 5f736571 75656e63 6integer_sequenc
+  0x000098a0 65496d4a 58737054 315f4545 45504e53 eImJXspT1_EEEPNS
+  0x000098b0 415f494a 44705432 5f454545 005f5f63 A_IJDpT2_EEE.__c
+  0x000098c0 75646152 65676973 74657246 756e6374 udaRegisterFunct
+  0x000098d0 696f6e40 6c696263 75646172 742e736f ion@libcudart.so
+  0x000098e0 2e313200 5f5a4e53 74367665 63746f72 .12._ZNSt6vector
+  0x000098f0 494e3363 31303941 6c696173 496e666f IN3c109AliasInfo
+  0x00009900 45536149 53315f45 45443145 76005f5a ESaIS1_EED1Ev._Z
+  0x00009910 54534e33 63313034 63756461 34696d70 TSN3c104cuda4imp
+  0x00009920 6c313343 55444147 75617264 496d706c l13CUDAGuardImpl
+  0x00009930 45005f5a 4e336331 3034696d 706c3136 E._ZN3c104impl16
+  0x00009940 56697274 75616c47 75617264 496d706c VirtualGuardImpl
+  0x00009950 44324576 005f5a4e 33633130 36646574 D2Ev._ZN3c106det
+  0x00009960 61696c33 30696e66 65724675 6e637469 ail30inferFuncti
+  0x00009970 6f6e5363 68656d61 46726f6d 46756e63 onSchemaFromFunc
+  0x00009980 746f7249 50464e32 61743654 656e736f torIPFN2at6Tenso
+  0x00009990 72455333 5f454545 53743130 756e6971 rES3_EEESt10uniq
+  0x000099a0 75655f70 7472494e 535f3134 46756e63 ue_ptrINS_14Func
+  0x000099b0 74696f6e 53636865 6d614553 74313464 tionSchemaESt14d
+  0x000099c0 65666175 6c745f64 656c6574 65495337 efault_deleteIS7
+  0x000099d0 5f454576 005f5a4e 33633130 37496e74 _EEv._ZN3c107Int
+  0x000099e0 54797065 33676574 4576005f 5a4e3363 Type3getEv._ZN3c
+  0x000099f0 31303131 53796d4e 6f646549 6d706c32 1011SymNodeImpl2
+  0x00009a00 65714552 4b4e535f 3133696e 74727573 eqERKNS_13intrus
+  0x00009a10 6976655f 70747249 53305f4e 535f3664 ive_ptrIS0_NS_6d
+  0x00009a20 65746169 6c333469 6e747275 73697665 etail34intrusive
+  0x00009a30 5f746172 6765745f 64656661 756c745f _target_default_
+  0x00009a40 6e756c6c 5f747970 65495330 5f454545 null_typeIS0_EEE
+  0x00009a50 45005079 4672616d 655f4765 74426163 E.PyFrame_GetBac
+  0x00009a60 6b005f5f 63756461 506f7043 616c6c43 k.__cudaPopCallC
   0x00009a70 6f6e6669 67757261 74696f6e 406c6962 onfiguration@lib
   0x00009a80 63756461 72742e73 6f2e3132 00507945 cudart.so.12.PyE
   0x00009a90 78635f49 6e646578 4572726f 72005f5a xc_IndexError._Z
   0x00009aa0 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
   0x00009ab0 706c3361 64644552 4b4e535f 3133696e pl3addERKNS_13in
   0x00009ac0 74727573 6976655f 70747249 53305f4e trusive_ptrIS0_N
   0x00009ad0 535f3664 65746169 6c333469 6e747275 S_6detail34intru
@@ -2661,76 +2661,76 @@
   0x0000a620 65746169 6c333469 6e747275 73697665 etail34intrusive
   0x0000a630 5f746172 6765745f 64656661 756c745f _target_default_
   0x0000a640 6e756c6c 5f747970 65495331 5f454545 null_typeIS1_EEE
   0x0000a650 43324550 53315f00 5f5a4e33 63313031 C2EPS1_._ZN3c101
   0x0000a660 3153796d 4e6f6465 496d706c 3973796d 1SymNodeImpl9sym
   0x0000a670 5f666c6f 61744576 0050794f 626a6563 _floatEv.PyObjec
   0x0000a680 745f5374 72005f5a 4e336331 3039466c t_Str._ZN3c109Fl
-  0x0000a690 6f617454 79706533 67657445 76005f5a oatType3getEv._Z
-  0x0000a6a0 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
-  0x0000a6b0 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x0000a6c0 365f6e6d 735f6375 5f316231 64376430 6_nms_cu_1b1d7d0
-  0x0000a6d0 655f3232 30303135 6e6d735f 6b65726e e_220015nms_kern
-  0x0000a6e0 656c5f69 6d706c49 66454576 6964504b el_implIfEEvidPK
-  0x0000a6f0 545f5079 00507944 6963745f 47657449 T_Py.PyDict_GetI
-  0x0000a700 74656d57 69746845 72726f72 005f5a4e temWithError._ZN
-  0x0000a710 33633130 34696d70 6c366465 7461696c 3c104impl6detail
-  0x0000a720 33315772 61704675 6e637469 6f6e496e 31WrapFunctionIn
-  0x0000a730 746f5275 6e74696d 6546756e 63746f72 toRuntimeFunctor
-  0x0000a740 5f495046 4e326174 3654656e 736f7245 _IPFN2at6TensorE
-  0x0000a750 53345f53 345f5334 5f6c4553 345f4e53 S4_S4_S4_lES4_NS
-  0x0000a760 5f346775 74733874 7970656c 69737438 _4guts8typelist8
-  0x0000a770 74797065 6c697374 494a5334 5f53345f typelistIJS4_S4_
-  0x0000a780 53345f6c 45454545 44314576 00507945 S4_lEEEED1Ev.PyE
-  0x0000a790 72725f46 6f726d61 74005f5a 4e336331 rr_Format._ZN3c1
-  0x0000a7a0 30366465 7461696c 31325f73 74725f77 06detail12_str_w
-  0x0000a7b0 72617070 6572494a 504b6352 4b537345 rapperIJPKcRKSsE
-  0x0000a7c0 45346361 6c6c4552 4b53335f 53355f00 E4callERKS3_S5_.
-  0x0000a7d0 5f5a4e53 7431305f 48617368 7461626c _ZNSt10_Hashtabl
-  0x0000a7e0 65495037 5f6f626a 65637453 315f5361 eIP7_objectS1_Sa
-  0x0000a7f0 4953315f 454e5374 385f5f64 65746169 IS1_ENSt8__detai
-  0x0000a800 6c395f49 64656e74 69747945 53743865 l9_IdentityESt8e
-  0x0000a810 7175616c 5f746f49 53315f45 53743468 qual_toIS1_ESt4h
-  0x0000a820 61736849 53315f45 4e53335f 31385f4d ashIS1_ENS3_18_M
-  0x0000a830 6f645f72 616e6765 5f686173 68696e67 od_range_hashing
-  0x0000a840 454e5333 5f32305f 44656661 756c745f ENS3_20_Default_
-  0x0000a850 72616e67 65645f68 61736845 4e53335f ranged_hashENS3_
-  0x0000a860 32305f50 72696d65 5f726568 6173685f 20_Prime_rehash_
-  0x0000a870 706f6c69 6379454e 53335f31 375f4861 policyENS3_17_Ha
-  0x0000a880 73687461 626c655f 74726169 7473494c shtable_traitsIL
-  0x0000a890 6230454c 6231454c 62314545 45454432 b0ELb1ELb1EEEED2
-  0x0000a8a0 4576005f 5a54534e 33633130 3230696e Ev._ZTSN3c1020in
-  0x0000a8b0 74727573 6976655f 7074725f 74617267 trusive_ptr_targ
-  0x0000a8c0 65744500 5f5a4e33 63313034 696d706c etE._ZN3c104impl
-  0x0000a8d0 32334578 636c7564 65446973 70617463 23ExcludeDispatc
-  0x0000a8e0 684b6579 47756172 64443145 76005f5a hKeyGuardD1Ev._Z
-  0x0000a8f0 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
-  0x0000a900 706c3967 75617264 5f696e74 45504b63 pl9guard_intEPKc
-  0x0000a910 6c005f5a 4e4b3363 31303653 796d496e l._ZNK3c106SymIn
-  0x0000a920 74396775 6172645f 696e7445 504b636c t9guard_intEPKcl
-  0x0000a930 005f5a4e 4b336331 30346375 64613469 ._ZNK3c104cuda4i
-  0x0000a940 6d706c31 33435544 41477561 7264496d mpl13CUDAGuardIm
-  0x0000a950 706c3138 756e6368 65636b65 64536574 pl18uncheckedSet
-  0x0000a960 44657669 6365454e 535f3644 65766963 DeviceENS_6Devic
-  0x0000a970 6545005f 5a4e3363 31303133 696e7472 eE._ZN3c1013intr
-  0x0000a980 75736976 655f7074 72494e53 5f31344f usive_ptrINS_14O
-  0x0000a990 70657261 746f724b 65726e65 6c454e53 peratorKernelENS
-  0x0000a9a0 5f366465 7461696c 3334696e 74727573 _6detail34intrus
-  0x0000a9b0 6976655f 74617267 65745f64 65666175 ive_target_defau
-  0x0000a9c0 6c745f6e 756c6c5f 74797065 4953315f lt_null_typeIS1_
-  0x0000a9d0 45454536 72657365 745f4576 005f5a54 EEE6reset_Ev._ZT
-  0x0000a9e0 494e3363 31303545 72726f72 45005f5a IN3c105ErrorE._Z
-  0x0000a9f0 53743974 65726d69 6e617465 7640474c St9terminatev@GL
-  0x0000aa00 49424358 585f332e 34005079 556e6963 IBCXX_3.4.PyUnic
-  0x0000aa10 6f64655f 41735554 4638416e 6453697a ode_AsUTF8AndSiz
-  0x0000aa20 65005079 5475706c 655f5369 7a65005f e.PyTuple_Size._
-  0x0000aa30 5a4e4b33 63313031 3054656e 736f7249 ZNK3c1010TensorI
-  0x0000aa40 6d706c31 3173697a 655f6375 73746f6d mpl11size_custom
-  0x0000aa50 456c005f 5a4e3363 31303134 4f706572 El._ZN3c1014Oper
-  0x0000aa60 61746f72 4b65726e 656c4432 4576005f atorKernelD2Ev._
+  0x0000a690 6f617454 79706533 67657445 76005079 oatType3getEv.Py
+  0x0000a6a0 44696374 5f476574 4974656d 57697468 Dict_GetItemWith
+  0x0000a6b0 4572726f 72005f5a 4e336331 3034696d Error._ZN3c104im
+  0x0000a6c0 706c3664 65746169 6c333157 72617046 pl6detail31WrapF
+  0x0000a6d0 756e6374 696f6e49 6e746f52 756e7469 unctionIntoRunti
+  0x0000a6e0 6d654675 6e63746f 725f4950 464e3261 meFunctor_IPFN2a
+  0x0000a6f0 74365465 6e736f72 4553345f 53345f53 t6TensorES4_S4_S
+  0x0000a700 345f6c45 53345f4e 535f3467 75747338 4_lES4_NS_4guts8
+  0x0000a710 74797065 6c697374 38747970 656c6973 typelist8typelis
+  0x0000a720 74494a53 345f5334 5f53345f 6c454545 tIJS4_S4_S4_lEEE
+  0x0000a730 45443145 76005079 4572725f 466f726d ED1Ev.PyErr_Form
+  0x0000a740 6174005f 5a4e3363 31303664 65746169 at._ZN3c106detai
+  0x0000a750 6c31325f 7374725f 77726170 70657249 l12_str_wrapperI
+  0x0000a760 4a504b63 524b5373 45453463 616c6c45 JPKcRKSsEE4callE
+  0x0000a770 524b5333 5f53355f 005f5a4e 53743130 RKS3_S5_._ZNSt10
+  0x0000a780 5f486173 68746162 6c654950 375f6f62 _HashtableIP7_ob
+  0x0000a790 6a656374 53315f53 61495331 5f454e53 jectS1_SaIS1_ENS
+  0x0000a7a0 74385f5f 64657461 696c395f 4964656e t8__detail9_Iden
+  0x0000a7b0 74697479 45537438 65717561 6c5f746f tityESt8equal_to
+  0x0000a7c0 4953315f 45537434 68617368 4953315f IS1_ESt4hashIS1_
+  0x0000a7d0 454e5333 5f31385f 4d6f645f 72616e67 ENS3_18_Mod_rang
+  0x0000a7e0 655f6861 7368696e 67454e53 335f3230 e_hashingENS3_20
+  0x0000a7f0 5f446566 61756c74 5f72616e 6765645f _Default_ranged_
+  0x0000a800 68617368 454e5333 5f32305f 5072696d hashENS3_20_Prim
+  0x0000a810 655f7265 68617368 5f706f6c 69637945 e_rehash_policyE
+  0x0000a820 4e53335f 31375f48 61736874 61626c65 NS3_17_Hashtable
+  0x0000a830 5f747261 69747349 4c623045 4c623145 _traitsILb0ELb1E
+  0x0000a840 4c623145 45454544 32457600 5f5a5453 Lb1EEEED2Ev._ZTS
+  0x0000a850 4e336331 30323069 6e747275 73697665 N3c1020intrusive
+  0x0000a860 5f707472 5f746172 67657445 005f5a4e _ptr_targetE._ZN
+  0x0000a870 33633130 34696d70 6c323345 78636c75 3c104impl23Exclu
+  0x0000a880 64654469 73706174 63684b65 79477561 deDispatchKeyGua
+  0x0000a890 72644431 4576005f 5a4e3363 31303131 rdD1Ev._ZN3c1011
+  0x0000a8a0 53796d4e 6f646549 6d706c39 67756172 SymNodeImpl9guar
+  0x0000a8b0 645f696e 7445504b 636c005f 5a4e4b33 d_intEPKcl._ZNK3
+  0x0000a8c0 63313036 53796d49 6e743967 75617264 c106SymInt9guard
+  0x0000a8d0 5f696e74 45504b63 6c005f5a 4e4b3363 _intEPKcl._ZNK3c
+  0x0000a8e0 31303463 75646134 696d706c 31334355 104cuda4impl13CU
+  0x0000a8f0 44414775 61726449 6d706c31 38756e63 DAGuardImpl18unc
+  0x0000a900 6865636b 65645365 74446576 69636545 heckedSetDeviceE
+  0x0000a910 4e535f36 44657669 63654500 5f5a4e33 NS_6DeviceE._ZN3
+  0x0000a920 63313031 33696e74 72757369 76655f70 c1013intrusive_p
+  0x0000a930 7472494e 535f3134 4f706572 61746f72 trINS_14Operator
+  0x0000a940 4b65726e 656c454e 535f3664 65746169 KernelENS_6detai
+  0x0000a950 6c333469 6e747275 73697665 5f746172 l34intrusive_tar
+  0x0000a960 6765745f 64656661 756c745f 6e756c6c get_default_null
+  0x0000a970 5f747970 65495331 5f454545 36726573 _typeIS1_EEE6res
+  0x0000a980 65745f45 76005f5a 54494e33 63313035 et_Ev._ZTIN3c105
+  0x0000a990 4572726f 7245005f 5a537439 7465726d ErrorE._ZSt9term
+  0x0000a9a0 696e6174 65764047 4c494243 58585f33 inatev@GLIBCXX_3
+  0x0000a9b0 2e340050 79556e69 636f6465 5f417355 .4.PyUnicode_AsU
+  0x0000a9c0 54463841 6e645369 7a650050 79547570 TF8AndSize.PyTup
+  0x0000a9d0 6c655f53 697a6500 5f5a4e4b 33633130 le_Size._ZNK3c10
+  0x0000a9e0 31305465 6e736f72 496d706c 31317369 10TensorImpl11si
+  0x0000a9f0 7a655f63 7573746f 6d456c00 5f5a4e33 ze_customEl._ZN3
+  0x0000aa00 63313031 344f7065 7261746f 724b6572 c1014OperatorKer
+  0x0000aa10 6e656c44 32457600 5f5a4e37 746f7263 nelD2Ev._ZN7torc
+  0x0000aa20 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
+  0x0000aa30 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
+  0x0000aa40 63755f31 35623935 6539315f 32353836 cu_15b95e91_2586
+  0x0000aa50 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
+  0x0000aa60 6c496645 45766964 504b545f 5079005f lIfEEvidPKT_Py._
   0x0000aa70 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
   0x0000aa80 6d706c32 3769735f 6368616e 6e656c73 mpl27is_channels
   0x0000aa90 5f6c6173 745f7374 72696465 735f3264 _last_strides_2d
   0x0000aaa0 454e535f 38417272 61795265 66494e53 ENS_8ArrayRefINS
   0x0000aab0 5f313369 6e747275 73697665 5f707472 _13intrusive_ptr
   0x0000aac0 4953305f 4e535f36 64657461 696c3334 IS0_NS_6detail34
   0x0000aad0 696e7472 75736976 655f7461 72676574 intrusive_target
```

## torchao/quantization/utils.py

```diff
@@ -95,14 +95,15 @@
     s = 0
     for p in model.parameters():
         s += p.nelement() * p.element_size()
     for b in model.buffers():
         s += b.nelement() * b.element_size()
     return s
 
+# TODO: quantization namespace is not the right place ot have this
 if version.parse(torch.__version__) >= version.parse("2.4.0.dev"):
     TORCH_VERSION_AFTER_2_4 = True
 else:
     TORCH_VERSION_AFTER_2_4 = False
 
 if version.parse(torch.__version__) >= version.parse("2.3.0.dev"):
     TORCH_VERSION_AFTER_2_3 = True
```

## Comparing `torchao_nightly-2024.5.23.dist-info/LICENSE` & `torchao_nightly-2024.5.24.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchao_nightly-2024.5.23.dist-info/METADATA` & `torchao_nightly-2024.5.24.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.5.23
+Version: 2024.5.24
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

## Comparing `torchao_nightly-2024.5.23.dist-info/RECORD` & `torchao_nightly-2024.5.24.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-torchao/_C.cpython-39-x86_64-linux-gnu.so,sha256=ueBWaVYbJjUX5A9FutOE7ayDqPtPOOj6MVnfDOGN8xI,810656
+torchao/_C.cpython-39-x86_64-linux-gnu.so,sha256=yxOWwKy9ZMCFnp8lZpWC6MXYhB0Zq2NEN5LhWHkXZRY,810656
 torchao/__init__.py,sha256=cV6Ke6Rr9WsMlnQGs6znd-25GrJewfDgfpHUtbvvGEs,426
 torchao/ops.py,sha256=xFX9XhUPDhdvc4u2wbfX-s4Li4mjAShnPMTRvX0R6ek,4792
 torchao/utils.py,sha256=d_pvMlkW6uyLO3RmMKJns2KL3s9Q2m6G0CEB6N5vZcg,860
 torchao/csrc/init.cpp,sha256=yH3sqHPiMO4t2b7lqJb4GU3zJtQtt_OrjvNm1qRSELs,74
 torchao/csrc/nms.cpp,sha256=xXR6X-w9AkhKwFuZhge3dp-cX5YI80FcUVigbzExWa4,251
 torchao/csrc/cuda/nms.cu,sha256=IhBuR-PhH1WFBtbGDSG7k5OE2lZAgKXQLtJkaNHKoUo,5554
 torchao/csrc/cuda/fp6_llm/fp6_linear.cu,sha256=qOzQyFNT2v3Z1HjtSt7LXEf0bn6hqFZ3t36Li01cTF0,9437
@@ -23,14 +23,16 @@
 torchao/prototype/dora/dora_layer.py,sha256=DGqY7Mg1PhD0uusFCEPeej5cPUD6CWJhOrjZDFJ9Ry4,6639
 torchao/prototype/dora/dora_profile.py,sha256=kXNQHvrTvCJl6LdLkbj6g_CAGvW1AESLA4g8o_65-U8,3972
 torchao/prototype/dora/kernels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchao/prototype/dora/kernels/common.py,sha256=J4ORrgK7MacmNg5FeU33IaZQg_y2COqOHaasBJA80Us,4846
 torchao/prototype/dora/kernels/custom_autotune.py,sha256=nljGHm7qWfIw2YxyZBwbSM-vCZ6LOFrWUcmACHindlg,15366
 torchao/prototype/dora/kernels/matmul.py,sha256=0no8T0EVd58ZSRTSDZ51dK9Z6glAjsTMSY5d0jUcHGM,7641
 torchao/prototype/dora/kernels/smallk.py,sha256=IuhcN69-uAugUEgTA8wRvC37UigbzRYsjt9N71aWHPk,16439
+torchao/prototype/fp8/__init__.py,sha256=607WEYAgShynAd-NZ2xynkflq0ecGrJKKXmtTFAv8tY,38
+torchao/prototype/fp8/splitk_gemm.py,sha256=m-EFKASgkiGa7haiJeqLc3YBYInQh3WmjAkAGurFy5w,3811
 torchao/prototype/galore/__init__.py,sha256=00BA4jwW7F8rXSVoJCt8auAsS4pNGzFiGWUjluAZXvE,23
 torchao/prototype/galore/utils.py,sha256=PXegtGgAaEWqi817Urqjg_U4cSW1Gbd2qDl8MpLwy_Y,3195
 torchao/prototype/galore/kernels/__init__.py,sha256=_LREFj3Nh1JpjJzCcRhlKluj6omfSh82qm0bgs1vm-s,210
 torchao/prototype/galore/kernels/adam_downproj_fused.py,sha256=mB_x78mS02bj434RduvO0vuR9W7PRjTbqiauonN-xrQ,10675
 torchao/prototype/galore/kernels/adam_step.py,sha256=Cxi-r4919zGMTgBz_h27HE0k0Sfq7GHwvBtZGBAf9V0,4722
 torchao/prototype/galore/kernels/custom_autotune.py,sha256=EOMMNb0j4gbKJjNId6A81wXdom-2sVBCNfDxkhYawSg,15180
 torchao/prototype/galore/kernels/matmul.py,sha256=BURVYayxXd1f7MVxuku1JNxDUQ29VH7NFdBq42a2Hkc,11641
@@ -46,15 +48,15 @@
 torchao/quantization/autoquant.py,sha256=lQibDS6P2WiiktyuuaWj6zx-G5676rfi9Y7sYhuOyTg,19369
 torchao/quantization/dynamic_quant.py,sha256=jSoTSeTk-Av5mvrDvqykbS0BPyhJAIGWEyQtTOXbzIA,2747
 torchao/quantization/quant_api.py,sha256=bQtu4oJsYIkry7B145KzbjriXDRhMcEt_V2yWx0-AJs,7110
 torchao/quantization/quant_primitives.py,sha256=ep1wH_kM7fy6EGjvuTW1xRNmH0XS-hUNTGjYQzHJh0U,32825
 torchao/quantization/smoothquant.py,sha256=zU_1Sywf9HwIO-Px2_5nAi6HOtWLkA_VwLLA2eS4ubo,9159
 torchao/quantization/subclass.py,sha256=OoDdW45aB13uAvn0lq4jsf3y62UuULP2I-6DA7F81vY,42347
 torchao/quantization/unified.py,sha256=OMKqbwoNo6P7ubyUL2wPsms5Rs6z6oNGqZm46eT6GGs,754
-torchao/quantization/utils.py,sha256=_641uYpzWbw2tdkhjdQGrXUryMpPxT4VIXEIieNJ6hA,3169
+torchao/quantization/utils.py,sha256=8SBDFb-H9-zHU4l3wjjN6AiNQkzBbr-xJKMW7UMkT8A,3236
 torchao/quantization/weight_only.py,sha256=gR0BLzFHeNel1Bwr2iiwz4qcZCkgkWVSNAZ9IoF_Pyo,2742
 torchao/quantization/prototype/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchao/quantization/prototype/qat.py,sha256=JI9vCsvXyUrkrf9AjDyj9RrgEhHG2ILchIlKmFGL_FI,12816
 torchao/sparsity/__init__.py,sha256=Ffo6dQSZ9G-7tjgwH5bDU1hSOA4rFaimsJfIOvO-RQU,508
 torchao/sparsity/sparse_api.py,sha256=HOLRPjPPuOIQFdWZ7DYBH0TFIgqGFAGgFw7qGPB8N4k,1077
 torchao/sparsity/utils.py,sha256=tiXs9WB65R1AElMJem4dJgPV-g-0TmTKGVcFnR__7yo,1708
 torchao/sparsity/wanda.py,sha256=LIeslH8Qj_ng9Cw0ROql8hkVFM0JwnTfdzzHvMPu2FQ,4156
@@ -73,12 +75,12 @@
 torchao/sparsity/prototype/scheduler/cubic_scheduler.py,sha256=fXirWwTeIixjh4Vpvzt-4fgjyPb7awM_ixQjQhTC-2c,3873
 torchao/sparsity/prototype/scheduler/lambda_scheduler.py,sha256=fRoa4OTZuuhxwwd9VLtUti5s6e7RHfwfDyy3UB3QjbU,2018
 torchao/sparsity/prototype/sparsifier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchao/sparsity/prototype/sparsifier/base_sparsifier.py,sha256=JVlL80Zwjv13u802EzD3yThnnkH4L2hM8hbI6cXqplg,13762
 torchao/sparsity/prototype/sparsifier/nearly_diagonal_sparsifier.py,sha256=tAI5EFoh6JZfolesoyfDuCzSxkjqhhtISXVvWjdMEw8,2189
 torchao/sparsity/prototype/sparsifier/utils.py,sha256=tFKke04D87JFiXX0AAgvWzAAfoj0TxC03HqgZzDG0N0,4786
 torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py,sha256=xPLtL3wyQuBShVcL1yqpJeCRPiyO9EKop4O6KMxzX9I,8853
-torchao_nightly-2024.5.23.dist-info/LICENSE,sha256=ZK-8briIL4OZEMv4DgmmN3My6-Lhe3rFAaPDzKH693s,1453
-torchao_nightly-2024.5.23.dist-info/METADATA,sha256=NRbuF8Lbac24dFz1qlR7yF90F_HsEwtDTo3ZyddUkcE,7128
-torchao_nightly-2024.5.23.dist-info/WHEEL,sha256=FNUt4eBsrBVn_Yc5KG3aXtKE40X3uNZrbGLNCbVxyFw,148
-torchao_nightly-2024.5.23.dist-info/top_level.txt,sha256=gGr5oEJ1W-T-QL0cRUf7RhX8HXPkJVi8DDnRwMMDZyY,8
-torchao_nightly-2024.5.23.dist-info/RECORD,,
+torchao_nightly-2024.5.24.dist-info/LICENSE,sha256=ZK-8briIL4OZEMv4DgmmN3My6-Lhe3rFAaPDzKH693s,1453
+torchao_nightly-2024.5.24.dist-info/METADATA,sha256=1xCYUdGHtKa10FTQ6qsfIPxRvbNnmMfeWRId2W9sE2k,7128
+torchao_nightly-2024.5.24.dist-info/WHEEL,sha256=FNUt4eBsrBVn_Yc5KG3aXtKE40X3uNZrbGLNCbVxyFw,148
+torchao_nightly-2024.5.24.dist-info/top_level.txt,sha256=gGr5oEJ1W-T-QL0cRUf7RhX8HXPkJVi8DDnRwMMDZyY,8
+torchao_nightly-2024.5.24.dist-info/RECORD,,
```

