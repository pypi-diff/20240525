# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.5.24-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.5.25-cp38-cp38-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,60 +1,62 @@
-Zip file size: 3172857 bytes, number of entries: 58
--rw-r--r--  2.0 unx     1342 b- defN 24-May-24 12:59 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-May-24 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-May-24 12:59 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10953208 b- defN 24-May-24 12:59 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-May-24 12:59 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-May-24 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-May-24 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-May-24 12:59 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4020 b- defN 24-May-24 12:59 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-May-24 12:59 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    31526 b- defN 24-May-24 12:59 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5859 b- defN 24-May-24 12:59 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-May-24 12:59 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-May-24 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26853 b- defN 24-May-24 12:59 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-May-24 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     4035 b- defN 24-May-24 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    67230 b- defN 24-May-24 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx   101933 b- defN 24-May-24 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40873 b- defN 24-May-24 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-May-24 12:59 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      419 b- defN 24-May-24 12:59 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-May-24 12:59 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-May-24 12:59 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-May-24 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-May-24 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-May-24 12:59 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4180 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4180 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2147 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3144 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3144 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2420 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2420 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4512 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4512 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3964 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3964 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3762 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3762 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-May-24 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx      231 b- defN 24-May-24 12:59 fbgemm_gpu/tbe/__init__.py
--rw-r--r--  2.0 unx      308 b- defN 24-May-24 12:59 fbgemm_gpu/tbe/cache/__init__.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-24 12:59 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
--rw-r--r--  2.0 unx     2602 b- defN 24-May-24 12:59 fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-May-24 12:59 fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-24 12:59 fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6301 b- defN 24-May-24 12:59 fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/RECORD
-58 files, 11387226 bytes uncompressed, 3162325 bytes compressed:  72.2%
+Zip file size: 3176431 bytes, number of entries: 60
+-rw-r--r--  2.0 unx     1342 b- defN 24-May-25 12:57 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-May-25 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-May-25 12:57 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10953208 b- defN 24-May-25 12:57 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-May-25 12:57 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-May-25 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-May-25 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-May-25 12:57 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-25 12:57 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-May-25 12:57 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    32627 b- defN 24-May-25 12:57 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5859 b- defN 24-May-25 12:57 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-May-25 12:57 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-May-25 12:57 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26853 b- defN 24-May-25 12:57 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-May-25 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     4035 b- defN 24-May-25 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    67230 b- defN 24-May-25 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx   101933 b- defN 24-May-25 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    44844 b- defN 24-May-25 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-May-25 12:57 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      419 b- defN 24-May-25 12:57 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-May-25 12:57 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-May-25 12:57 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-May-25 12:57 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-May-25 12:57 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-25 12:57 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx     1964 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4181 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4181 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2153 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     2194 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args_ssd.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3145 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3145 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2421 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2421 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4513 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4513 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3902 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_ssd.py
+-rw-r--r--  2.0 unx     3965 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3965 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3763 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3763 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-May-25 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx      231 b- defN 24-May-25 12:57 fbgemm_gpu/tbe/__init__.py
+-rw-r--r--  2.0 unx      308 b- defN 24-May-25 12:57 fbgemm_gpu/tbe/cache/__init__.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-25 12:57 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
+-rw-r--r--  2.0 unx     2602 b- defN 24-May-25 12:57 fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-May-25 12:57 fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-25 12:57 fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6564 b- defN 24-May-25 12:57 fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/RECORD
+60 files, 11399181 bytes uncompressed, 3165449 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -93,14 +93,17 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
 Comment: 
 
+Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args_ssd.py
+Comment: 
+
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
@@ -129,14 +132,17 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
 Comment: 
 
+Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_ssd.py
+Comment: 
+
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
@@ -156,20 +162,20 @@
 
 Filename: fbgemm_gpu/tbe/cache/__init__.py
 Comment: 
 
 Filename: fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -16151,53 +16151,53 @@
 SymFloat
 GenericList
 PyObject
 Uninitialized
 Quantizer
 Generator
 InvalidTag(
-extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
+extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/forward/embedding_forward_split_cpu.cpp
 Expected !indice_weights.defined() || indice_weights.scalar_type() != at::kHalf to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_codegen_forward_cpu_meta
 split_embedding_codegen_forward_cpu(Tensor weights, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, Tensor hash_size_cumsum, Tensor indices, Tensor offsets, int pooling_mode, Tensor indice_weights, int output_dtype) -> Tensor
 Expected weights.is_contiguous() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_forward_cpu_kernel
 split_embedding_grad_indice_weights_cpu_outer
 split_embedding_grad_indice_weights_cpu
 split_embedding_codegen_grad_indice_weights_cpu(Tensor grad_output, Tensor weights, Tensor weights_offsets, Tensor D_offsets, Tensor indices, Tensor offsets, Tensor feature_requires_grad) -> Tensor
 tensor does not have a device
 device_default
 There is an error in the layout calculation logic.
-is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
+is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
 Operators taking TensorOptions cannot take a TensorOptions with options.requires_grad set as true. This isn't implemented yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
 check_tensor_options_and_extract_memory_format
 Cannot set memory_format both in TensorOptions and explicit argument; please delete the redundant setter.
 basic_string::_S_construct null not valid
 basic_string::append
 IntArrayRef contains an int that cannot be represented as a SymInt: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymIntArrayRef.h
 fromIntArrayRefSlow
  dims but tensor has 
 TensorAccessor expected 
 accessor
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/TensorBase.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/TensorBase.h
  is out of bounds: 
 , range 
 report_embedding_error
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/include/fbgemm_gpu/cpu_utils.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
 expected int
 vector::_M_realloc_insert
 Expected SymInt or int but got 
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h
 toSymInt
 St19bad_optional_access
 N3c1020intrusive_ptr_targetE
 N3c1014OperatorKernelE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_S5_S5_S5_EXadL_Z47split_embedding_codegen_grad_indice_weights_cpuS5_S5_S5_S5_S5_S5_S5_EEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_S5_S5_EEEEE
 FN2at6TensorES0_S0_S0_S0_S0_S0_S0_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_NS_6SymIntES5_S5_S5_lS5_lEXadL_Z35split_embedding_codegen_forward_cpuS5_S5_S5_S6_S5_S5_S5_lS5_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S6_S5_S5_S5_lS5_lEEEEE
@@ -16226,136 +16226,136 @@
 __obj_flatten__
 Expected GenericDict but got 
 toGenericDict
 Unknown Exception Type
  devices
 getDeviceGuardImpl
 PyTorch is not linked with support for 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
 Event device type 
  does not match blocking stream's device type 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineEvent.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineEvent.h
 Expected !name.empty() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h
 Invalid name for qualified name: '
-!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
-!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
+!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
+!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/util/ArrayRef.h
 QualifiedName
 basic_string::substr
 ArrayRef: invalid slice, N = 
 ; size = 
 Expected a 0-dim Tensor, but got Tensor with dimensions: 
-tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
+tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
  in its first dimension, but got Tensor with size 
-tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
+tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
 TensorDataContainer is already a Tensor type, `fill_tensor` should not be called
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
 Invalid TensorDataContainer type
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
 fill_tensor
 Expected a Tensor with size 
  in its first dimension
 can not do torch::tensor(complex, dtype=non-complex) because complex can not be casted to real number without loss of information
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
 convert_to_tensor
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/inference/embedding_forward_quantized_host_cpu.cpp
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function shouldn't be called for CPU; it is only for GPU.
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1966, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1966, please report a bug to PyTorch. 
 vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
 __getstate__ should take exactly one argument: self. Got: 
 self argument of __getstate__ must be the custom class type. Got 
 __getstate__ should return exactly one value for serialization. Got: 
 __getstate__'s return type should be a subtype of input argument of __setstate__. Got 
-isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2355, please report a bug to PyTorch. 
+isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2355, please report a bug to PyTorch. 
 //deeplearning/fbgemm/fbgemm_gpu:sparse_ops_py
 int_nbit_split_embedding_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment = None, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1) -> Tensor
 int_nbit_split_embedding_codegen_lookup_function
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights=None, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment=-1, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1, Tensor? cache_hash_size_cumsum=None, int? total_cache_hash_size=-1, Tensor? cache_index_table_map=None, Tensor? lxu_cache_state=None, Tensor? lxu_state=None) -> Tensor
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function
 pruned_hashmap_insert(Tensor indices, Tensor dense_indices, Tensor offsets, Tensor(a!) hash_table, Tensor hash_table_offsets) -> ()
 pruned_hashmap_lookup(Tensor indices, Tensor offsets, Tensor hash_table, Tensor hash_table_offsets) -> Tensor
 pruned_array_lookup(Tensor indices, Tensor offsets, Tensor index_remappings, Tensor index_remappings_offsets) -> Tensor
-isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2082, please report a bug to PyTorch. 
-self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
+isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2082, please report a bug to PyTorch. 
+self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h
 Only Tensors of floating point and complex dtype can require gradients
 AutogradMeta
 set_requires_grad
 Expected T > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected B > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected maps_.size() == T to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 , got one on device 
 getDevicesOfStorages
 Expected all data ptrs to be on a device of type 
 vector::reserve
 Expected map.size() == (table_offsets_acc[t + 1] - table_offsets_acc[t]) to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 serialize
 table_offsets
 vector::_M_fill_insert
-schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h
+schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h
 BuiltinOpFunction
 defineMethod
 Default values must be specified for none or all arguments
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/custom_class.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/custom_class.h
 TensorImpl with nullptr is not supported
 init_tensor
 vector::_M_default_append
 cannot create std::deque larger than max_size()
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodIZNS2_10def_pickleINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL20PrunedMapCPURegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodIZNS2_10def_pickleINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL21AtomicCounterRegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodIZNS2_10def_pickleINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL19TensorQueueRegistryMUlNS5_4DictISsN2at6TensorEEEE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSH_E_EEPNS_3jit8FunctionESsSK_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISZ_EEE_
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 Expected Object but got 
 toObject
-isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
+isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
 Argument passed to at() was not in the map.
 Streams have a mix of device types: stream 0 is on 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
  while stream 
  is on device 
 getDeviceTypeOfStreams
 , trying to set error: 
 setErrorInternal
 Error already set on this Future: 
 Future is already marked completed
-!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1215, please report a bug to PyTorch. 
+!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1215, please report a bug to PyTorch. 
  which are not among the expected device(s) 
 The result contained tensors residing on device(s) 
 Attempting to mark a completed Future as complete again. Note that a Future can only be marked completed once.
  does not match recording stream's device type 
 ensureIsSubsetOfDevices
 markCompleted
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
  could not be converted to any of the known types.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type.h
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 Tried to cast IValue to custom class but it did not contain a custom class!
-isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
+isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
 toCustomClass
 toCapsule
 Expected TensorList but got 
 toTensorList
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2038, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2038, please report a bug to PyTorch. 
 Tried to cast a Dict<
 > to a Dict<
 >. Key types mismatch.
 toTypedDict
 >. Value types mismatch.
-*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h
-*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
+*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h
+*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
 N3c1010ValueErrorE
 N3c1011StorageImplE
 N3c1015VariableVersion14VersionCounterE
 N3c104impl24DeviceGuardImplInterfaceE
 N3c106detail8ListImplE
 N5torch17CustomClassHolderE
 N3c106detail8DictImplE
@@ -16403,37 +16403,37 @@
 pooling_mode
 function 
 apply_with_saved
 missing before())
 vector<bool>::_M_insert_aux
 Please open a feature request on GitHub if you need this.
 jvp is not implemented for the c++ API of custom Function yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h
 compiled_args not implemented for non-traceable node: 
 dense_embedding_codegen_lookup_function(Tensor dev_weights, Tensor weights_offsets, Tensor D_offsets, int total_D, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, int output_dtype=0) -> Tensor
 dense_embedding_codegen_lookup_function
 Cannot update a node's topological_nr after it already has a parent. If we allow this, we can no longer guarantee that a parent's topo_nr is always greater than those of all its children
-!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h
+!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/backward/embedding_backward_dense_host_cpu.cpp
 Check failed: grad_outputs.size() == 1 (
  returned an incorrect number of gradients (expected 
  returned a gradient different that is defined at position 
 , but the corresponding forward input was not a Variable
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
-it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
-arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
-it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
-sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
+it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
+arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
+it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
+sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
 next_sym_size
 PFvPN5torch8autograd4NodeEE
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRN2at6TensorES8_S8_RlS9_S8_S9_S8_S8_S9_RSt8optionalIS7_ESC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSE_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSF_EUlRKSt6vectorIS7_SaIS7_EESP_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRN2at6TensorES8_S8_RlS9_S8_S9_S8_S8_S9_RSt8optionalIS7_ESC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSE_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSF_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_llS5_lS5_S5_lSt8optionalIS5_ES7_lEXadL_ZN12_GLOBAL__N_145split_embedding_codegen_lookup_dense_functionES5_S5_S5_llS5_lS5_S5_lS7_S7_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_llS5_lS5_S5_lS7_S7_lEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
@@ -16476,37 +16476,37 @@
 sum_reduce_to_one
 merge_pooled_embeddings
 t must be a CPU tensor; it is currently on device 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/merge_pooled_embedding_ops/merge_pooled_embedding_ops_cpu.cpp
 Expected input_tensors.size() > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 input_0 must be a CPU tensor; it is currently on device 
 input_tensors[i] must be a CPU tensor; it is currently on device 
-isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":931, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2034, please report a bug to PyTorch. 
+isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":931, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2034, please report a bug to PyTorch. 
 toDevice
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EElNS_6DeviceElEXadL_ZN10fbgemm_gpu27merge_pooled_embeddings_cpuES8_lS9_lEEEES5_NS_4guts8typelist8typelistIJS8_lS9_lEEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EElN3c106DeviceElE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EENS_6DeviceEEXadL_ZN10fbgemm_gpu21sum_reduce_to_one_cpuES8_S9_EEEES5_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EEN3c106DeviceEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES8_NS_6DeviceEEXadL_ZN10fbgemm_gpu21all_to_one_device_cpuES8_S9_EEEES8_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FSt6vectorIN2at6TensorESaIS1_EES3_N3c106DeviceEE
 merge_pooled_embeddings(Tensor[] pooled_embeddings, SymInt uncat_dim_size, Device target_device, SymInt cat_dim=all_to_one_device(Tensor[] input_tensors, Device target_device) sum_reduce_to_onfbgemm::permute_pooled_embs
 expected bool
 fbgemm::permute_duplicate_pooled_embs
 offset_dim_list needs to have long/int64 type
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_function.cpp
 permute_list needs to have long/int64 type
 Expected ptr_->is_bool() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymBool.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":676, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymBool.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":676, please report a bug to PyTorch. 
 permute_pooled_embs does not support allow_duplicates in backward!
 Tried to access the schema for 
  which doesn't have a schema registered yet
-schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
+schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
 FN2at6TensorERKS0_S2_S2_S2_S2_E
 inv_offset_dim_linv_permute_listallow_duplicatespermute_pooled_embs_cpu_impl
 permute_pooled_embs_auto_grad
 permute_duplicate_pooled_embs
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_ops_cpu.cpp
 permute_duplicate_pooled_embs_auto_grad
 N5torch8autograd7CppNodeIN10fbgemm_gpu25PermutePooledEmbsFunctionEEE
@@ -16565,27 +16565,27 @@
 num_output_rows
 slice_length
 fbgemm::jagged_slice_forward
 lengths is currently on 
 start should be <= len
 jagged_dense_dense_elementwise_add_jagged_output
 batched_dense_vec_jagged_2d_mul
-isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2066, please report a bug to PyTorch. 
+isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2066, please report a bug to PyTorch. 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/jagged_tensor_ops/jagged_tensor_ops_autograd.cpp
 Expected grad_outputs.size() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_L >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_to_padded_dense_backward
 fbgemm::jagged_to_padded_dense_forward
 Expected values.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_L > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_lengths.size() == x_offsets.size() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected SymIntList or IntList but got 
-isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1978, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
+isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1978, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymInt.h
 Expected dense_values_grad.sym_sizes() == dense_shape to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_dense_dense_elementwise_add_jagged_output_forward
 fbgemm::jagged_dense_elementwise_mul_backward
 fbgemm::jagged_dense_elementwise_mul_forward
 fbgemm::batched_dense_vec_jagged_2d_mul_backward
 fbgemm::batched_dense_vec_jagged_2d_mul_forward
 fbgemm::dense_to_jagged_forward
@@ -16605,15 +16605,15 @@
 fbgemm::jagged_index_select_2d_forward_v2
 output_lengths is currently on 
 grad must be on the same device as output_lengths! grad is currently on 
 Tensor 'values' must have 1 dimension(s). Found 
 values must be on the same device as lengths! values is currently on 
 start should be always be positive
 type with contained types did not overload createWithContained: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type_base.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type_base.h
 createWithContained
 ; Length = 
 ArrayRef: invalid index Index = 
  with None type
 Can not create 
 : SymIntArrayRef expected to contain only concrete integers
 asIntArrayRefSlow
@@ -16659,24 +16659,24 @@
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115DenseToJaggedOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_136JaggedDenseElementwiseAddJaggedOutOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115JaggedSoftmaxOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_117JaggedJaggedBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_116JaggedDenseBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_121JaggedIndexSelect2dOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_113JaggedSliceOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
 Tried to cast a List<
 > to a List<
 >. Types mismatch.
 toTypedList
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/List_inl.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/List_inl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
 Expected ptr_->is_float() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymFloat.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
 expected double
 toDouble
 St23enable_shared_from_thisIN3c1010SharedTypeEE
 N3c1010SharedTypeE
 N3c1017SingleElementTypeILNS_8TypeKindE6ENS_8ListTypeEEE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefINS8_6SymIntEEEdE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefIlEEdE
@@ -16873,15 +16873,15 @@
 jagged_jagged_elementwise_dense_output_kernel_
 Expected !NO_INNER_DENSE || output.size(-1) == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 unsupported number of jagged dim 
 jagged_2d_to_dense_forward_cpu
 jagged_2d_to_dense_backward_kernel
 fbgemm::jagged_index_select_2d_forward
 fbgemm::jagged_index_add_2d_forward
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1962, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1962, please report a bug to PyTorch. 
 FN2at6TensorERKS0_S2_S2_S2_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_RKSt6vectorIS5_SaIS5_EES7_EXadL_ZN10fbgemm_gpu28jagged_dense_elementwise_addES7_SC_S7_EEEES5_NS_4guts8typelist8typelistIJS7_SC_S7_EEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_1d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 FSt6vectorIN2at6TensorESaIS1_EES1_S1_RKS_IlSaIlEES7_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_2d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_lEXadL_ZN10fbgemm_gpu34jagged_index_select_2d_forward_cpuES7_S7_S7_S7_lEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_llEXadL_ZN10fbgemm_gpu31jagged_index_add_2d_forward_cpuES7_S7_S7_S7_llEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_llEEEEE
@@ -17460,15 +17460,15 @@
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_bEXadL_Z43batch_index_select_dim0_tensor_cpu_autogradS7_S7_S7_S7_S7_bEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_bEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_bE
 St19_Sp_counted_deleterIPN5torch8autograd7CppNodeI25BatchIndexSelectDim0CPUOpEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 St19_Sp_counted_deleterIPN5torch8autograd7CppNodeI31BatchIndexSelectDim0TensorCPUOpEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 Unsupported SparseType: 
 pruned_array_lookup_cpu
 Expected placement != PlacementType::DEVICE to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
 int8 output are only supported for int8 weights
 Expected offsets_nobag.numel() == index_size + 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets_nobag_ptr[index_size] - offsets_nobag_ptr[0] == index_size to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 int_nbit_split_embedding_codegen_forward_unweighted_cpu
 Expected B >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_D > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Enabling both CUDA and HIP in ATen is not supported, as HIP masquerades to be CUDA (e.g., when you say CUDA, on a HIP build of ATen, this actually means HIP.  Rebuild PyTorch with one or the other disabled.
@@ -17481,30 +17481,30 @@
 int_nbit_split_embedding_nobag_codegen_forward_
 "intn_split_embedding_nobag_codegen_forward_kernel"
 pruned_hashmap_lookup_unweighted_cpu
 hash_table must be a CPU tensor; it is currently on device 
 hash_table_offsets must be a CPU tensor; it is currently on device 
 pruned_hashmap_insert_unweighted_cpu
 dense_indices must be a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
 pruned_hashmap_lookup_weighted_cpu
 pruned_hashmap_insert_weighted_cpu
 int_nbit_split_embedding_codegen_forward_weighted_cpu
 indice_weights must be empty or a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
 Check failed: host_weights.dim() == 1 (
 split_embedding_backward_exact_cpu
 split_embedding_backward_codegen_dense_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, float unused = 0) -> Tensor
 split_embedding_backward_codegen_dense_cpu
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_dEXadL_Z42split_embedding_backward_codegen_dense_cpuS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEEE
 FN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_dE
 split_embedding_codegen_grad_indice_weights_pt2_wrapper
 split_embedding_codegen_forward_weighted_pt2_wrapper
 split_embedding_codegen_forward_unweighted_pt2_wrapper
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
 fbgemm::split_embedding_codegen_grad_indice_weights_cpu
 fbgemm::split_embedding_codegen_forward_cpu
 FN2at6TensorES0_S0_S0_lS0_S0_S0_lS0_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_NS_6SymIntES7_S7_S7_S7_EXadL_Z59split_embedding_codegen_grad_indice_weights_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_N3c106SymIntES2_S2_S2_S2_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_NS_6SymIntES8_S7_S7_S7_lS7_S7_S7_blEXadL_Z56split_embedding_codegen_forward_weighted_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_N3c106SymIntES4_S2_S2_S2_lS2_S2_S2_blE
@@ -17512,150 +17512,150 @@
 gradient_clipping
 max_gradient
 stochastic_rounding
 output_dtype
 learning_rate
 split_embedding_codegen_lookup_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddlEXadL_ZN12_GLOBAL__N_151split_embedding_codegen_lookup_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z71split_embedding_backward_codegen_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_ddlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z73split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 weight_decay
 weight_decay_mode
 max_norm
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_rowwise_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddldlEXadL_ZN12_GLOBAL__N_159split_embedding_codegen_lookup_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddldlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z79split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_dddldlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z81split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 split_embedding_codegen_lookup_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_sgd_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
 fbgemm::split_embedding_backward_codegen_sgd_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_147split_embedding_codegen_lookup_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bdlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bdlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbdlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_sgd_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_sgd_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z67split_embedding_backward_codegen_sgd_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbdlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z69split_embedding_backward_codegen_sgd_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 split_embedding_codegen_lookup_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
 split_embedding_codegen_lookup_adam_function_cpu
 split_embedding_codegen_lookup_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_dddddllE
 split_embedding_codegen_lookup_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
 split_embedding_codegen_lookup_lamb_function_cpu
 split_embedding_codegen_lookup_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_lars_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
 split_embedding_codegen_lookup_lars_sgd_function_cpu
 split_embedding_codegen_lookup_lars_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float learning_rate = 0, float eta = 0, float momentum = 0, float weight_decay = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddddlEXadL_ZN12_GLOBAL__N_152split_embedding_codegen_lookup_lars_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddddlE
 split_embedding_codegen_lookup_none_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_none_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_none_cpu.cpp
 split_embedding_codegen_lookup_none_function_cpu
 split_embedding_codegen_lookup_none_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, int total_hash_size = 0, int total_unique_indices = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdblllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_none_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdblllE
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_172split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_S0_S0_S0_dddllldlllddllddlE
 split_embedding_codegen_lookup_approx_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
 split_embedding_codegen_lookup_approx_sgd_function_cpu
 split_embedding_codegen_lookup_approx_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_154split_embedding_codegen_lookup_approx_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_166split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddllE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_179split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_184split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_177split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_168split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
 split_embedding_backward_exact_cpu_outer
 CPU exact rowwise adagrad currently doesn't support embedding tables with more than 2B rows
 split_embedding_backward_codegen_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEXadL_Z44split_embedding_backward_codegen_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEE
 does not match c_block size: 
 num of rows processed by adagrad: 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
 split_embedding_backward_codegen_rowwise_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEXadL_Z52split_embedding_backward_codegen_rowwise_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
 split_embedding_backward_codegen_sgd_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEXadL_Z40split_embedding_backward_codegen_sgd_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEE
 GCC: (conda-forge gcc 10.4.0-19) 10.4.0
 .shstrtab
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -983951,15 +983951,15 @@
 	jne    602ab3 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, std::optional<at::Tensor>, long, std::optional<at::Tensor>, std::optional<at::Tensor>, std::optional<long>, std::optional<long>, std::optional<long>, std::optional<long>, std::optional<at::Tensor>, std::optional<long>, std::optional<at::Tensor>, std::optional<at::Tensor>, std::optional<at::Tensor>)@@Base+0x13b3>
 	movb   $0x1,0x30(%rdi)
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0xa0(%rsp)
 	vmovdqa %xmm0,0x90(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x30(%rsp),%rbx
 	lea    0x40(%rsp),%r15
 	mov    %rdx,0xa0(%rsp)
 	lea    0x38c51f(%rip),%rsi        # 98f018 <std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits@@Base+0x13f8>
 	mov    %rdx,0x98(%rsp)
 	mov    %r15,%rdi
@@ -1028169,15 +1028169,15 @@
 	vpinsrq $0x1,%rax,%xmm0,%xmm0
 	vmovdqu %xmm0,0x20(%rdi)
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x40(%rsp)
 	vmovdqa %xmm0,0x30(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x28(%rsp),%rbp
 	mov    %rdx,0x40(%rsp)
 	lea    0x364dfa(%rip),%rsi        
 	mov    %rbp,%rdi
 	mov    %rdx,0x38(%rsp)
 	lea    0x27(%rsp),%rdx
@@ -1028669,15 +1028669,15 @@
 	push   %rbx
 	sub    $0xd8,%rsp
 	mov    %rdi,0x10(%rsp)
 	mov    $0x4,%edi
 	movq   $0x0,0x40(%rsp)
 	vmovdqa %xmm0,0x30(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x28(%rsp),%rbp
 	mov    %rdx,0x40(%rsp)
 	lea    0x364512(%rip),%rsi        
 	mov    %rbp,%rdi
 	mov    %rdx,0x38(%rsp)
 	lea    0x27(%rsp),%rdx
@@ -1031521,15 +1031521,15 @@
 	jne    633847 <fbgemm_gpu::sum_reduce_to_one_cpu(std::vector<at::Tensor, std::allocator<at::Tensor> >, c10::Device)@@Base+0x14a7>
 	movb   $0x1,0x30(%rdi)
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x20(%rsp)
 	vmovdqa %xmm0,0x10(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	mov    $0x95,%edi
 	mov    %rax,0x10(%rsp)
 	mov    %rdx,0x20(%rsp)
 	mov    %rdx,0x18(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
 	vmovdqa 0x361931(%rip),%xmm0        # 9951c0 <typeinfo name for std::vector<at::Tensor, std::allocator<at::Tensor> > (std::vector<at::Tensor, std::allocator<at::Tensor> >, c10::Device)@@Base+0x40>
@@ -1041144,15 +1041144,15 @@
 	movq   $0x0,0x20(%rsp)
 	vmovdqa %xmm0,0x10(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
 	lea    0x4(%rax),%rdx
 	xor    %esi,%esi
 	mov    $0x93,%edi
 	mov    %rax,0x10(%rsp)
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	mov    %rdx,0x20(%rsp)
 	mov    %rdx,0x18(%rsp)
 	call   63de00 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0xc90>
 	mov    %rax,%rdx
 	lea    0x18(%rax),%rax
 	vmovdqa 0x3583b0(%rip),%xmm0        # 9962a0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0xa0>
 	mov    0x42c5b9(%rip),%rbx        
@@ -1041211,15 +1041211,15 @@
 	movq   $0x0,0x20(%rsp)
 	vmovdqa %xmm0,0x10(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
 	lea    0x4(%rax),%rdx
 	xor    %esi,%esi
 	mov    $0x9d,%edi
 	mov    %rax,0x10(%rsp)
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	mov    %rdx,0x20(%rsp)
 	mov    %rdx,0x18(%rsp)
 	call   63de00 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0xc90>
 	vmovdqa 0x358260(%rip),%xmm0        # 9962a0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0xa0>
 	mov    %rax,%rdx
 	lea    0x18(%rax),%rax
 	movabs $0x54203e2d20297473,%rcx
@@ -1128281,15 +1128281,15 @@
 	je     69e17c <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x143c>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	lea    0xc(%rsp),%r14
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	mov    %r14,%rsi
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x300e78(%rip),%rsi        # 99f018 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1ad8>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
@@ -1128304,15 +1128304,15 @@
 	je     69e1da <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x149a>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x300e7f(%rip),%rsi        # 99f078 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1b38>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128326,15 +1128326,15 @@
 	je     69e233 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x14f3>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x300e86(%rip),%rsi        # 99f0d8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1b98>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128348,15 +1128348,15 @@
 	je     69e28c <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x154c>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x300e85(%rip),%rsi        # 99f130 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1bf0>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128450,15 +1128450,15 @@
 	je     69e435 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x16f5>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x300fbc(%rip),%rsi        # 99f410 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1ed0>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128472,15 +1128472,15 @@
 	je     69e48e <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x174e>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x300fdb(%rip),%rsi        # 99f488 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1f48>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128494,15 +1128494,15 @@
 	je     69e4e7 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x17a7>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301002(%rip),%rsi        # 99f508 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x1fc8>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128516,15 +1128516,15 @@
 	je     69e540 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1800>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301009(%rip),%rsi        # 99f568 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2028>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128538,15 +1128538,15 @@
 	je     69e599 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1859>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301008(%rip),%rsi        # 99f5c0 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2080>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128560,15 +1128560,15 @@
 	je     69e5f2 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x18b2>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x30101f(%rip),%rsi        # 99f630 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x20f0>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128582,15 +1128582,15 @@
 	je     69e64b <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x190b>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301046(%rip),%rsi        # 99f6b0 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2170>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128604,15 +1128604,15 @@
 	je     69e6a4 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1964>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301075(%rip),%rsi        # 99f738 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x21f8>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128626,15 +1128626,15 @@
 	je     69e6fd <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x19bd>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301084(%rip),%rsi        # 99f7a0 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2260>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128648,15 +1128648,15 @@
 	je     69e756 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1a16>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x30108b(%rip),%rsi        # 99f800 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x22c0>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128670,15 +1128670,15 @@
 	je     69e7af <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1a6f>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x3010b2(%rip),%rsi        # 99f880 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2340>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128692,15 +1128692,15 @@
 	je     69e808 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1ac8>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x3010b1(%rip),%rsi        # 99f8d8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2398>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128714,15 +1128714,15 @@
 	je     69e861 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1b21>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x3010b8(%rip),%rsi        # 99f938 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x23f8>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128736,15 +1128736,15 @@
 	je     69e8ba <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1b7a>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x3010df(%rip),%rsi        # 99f9b8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2478>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128778,15 +1128778,15 @@
 	je     69e967 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1c27>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301132(%rip),%rsi        # 99fab8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2578>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128820,15 +1128820,15 @@
 	je     69ea14 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1cd4>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x3011cd(%rip),%rsi        # 99fc00 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x26c0>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128862,15 +1128862,15 @@
 	je     69eac1 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1d81>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301238(%rip),%rsi        # 99fd18 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x27d8>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128884,15 +1128884,15 @@
 	je     69eb1a <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1dda>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301237(%rip),%rsi        # 99fd70 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2830>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128946,15 +1128946,15 @@
 	je     69ec1b <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1edb>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x30123e(%rip),%rsi        # 99fe78 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2938>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1128988,15 +1128988,15 @@
 	je     69ecc8 <fbgemm_gpu::jagged_slice_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool)@@Base+0x1f88>
 	mov    0x20(%rsp),%rsi
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	mov    %r14,%rsi
 	mov    %r12,%rdi
 	mov    $0x1,%edx
-	movl   $0x9,0xc(%rsp)
+	movl   $0xa,0xc(%rsp)
 	call   6858c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x7e0>
 	lea    0x301259(%rip),%rsi        # 99ff40 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor, at::Tensor, c10::SymInt), &fbgemm_gpu::jagged_2d_to_dense_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, c10::SymInt> >@@Base+0x2a00>
 	mov    %rbp,%rdi
 	call   6861c0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt>, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x10e0>
 	xor    %r8d,%r8d
 	mov    %r12,%rcx
 	xor    %edx,%edx
@@ -1440037,15 +1440037,15 @@
 	jne    7f764c <fbgemm_gpu::padding_fused_tbe_input_combine_cpu(std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)@@Base+0x1acc>
 	movb   $0x1,0x30(%rdi)
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x20(%rsp)
 	vmovdqa %xmm0,0x10(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x7(%rsp),%r15
 	lea    0x8(%rsp),%r14
 	mov    %rdx,0x20(%rsp)
 	lea    0x1aa9df(%rip),%rsi        # 9a2068 <typeinfo name for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long> >@@Base+0xb68>
 	mov    %rdx,0x18(%rsp)
 	mov    %r14,%rdi
@@ -1440080,15 +1440080,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x20(%rsp)
 	vmovdqa %xmm0,0x10(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x1aa9c3(%rip),%rsi        # 9a2100 <typeinfo name for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long> >@@Base+0xc00>
 	mov    %r14,%rdi
 	mov    %rdx,0x20(%rsp)
 	mov    %rdx,0x18(%rsp)
 	mov    %r15,%rdx
 	mov    %rax,0x10(%rsp)
@@ -1449653,15 +1449653,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x1a1665(%rip),%rsi        # 9a31d8 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x4d8>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   7ffd20 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&), &fbgemm_gpu::recat_embedding_grad_output_mixed_D_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<long, std::allocator<long> > const&> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xf40>
@@ -1449780,15 +1449780,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x1a15ef(%rip),%rsi        # 9a3370 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x670>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   7ffd20 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&), &fbgemm_gpu::recat_embedding_grad_output_mixed_D_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<long, std::allocator<long> > const&> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xf40>
@@ -1531942,15 +1531942,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x14989d(%rip),%rsi        # 9a83b8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x32b8>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1531969,15 +1531969,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x1498c9(%rip),%rsi        # 9a8458 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x3358>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532016,15 +1532016,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x1498d3(%rip),%rsi        # 9a8528 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x3428>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532123,15 +1532123,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149b1f(%rip),%rsi        # 9a8930 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x3830>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532150,15 +1532150,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149ae3(%rip),%rsi        # 9a8968 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x3868>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532177,15 +1532177,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149aa7(%rip),%rsi        # 9a89a0 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x38a0>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532304,15 +1532304,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149c91(%rip),%rsi        # 9a8d98 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x3c98>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532391,15 +1532391,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149ef7(%rip),%rsi        # 9a9168 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x4068>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532478,15 +1532478,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149f35(%rip),%rsi        # 9a9310 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x4210>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532585,15 +1532585,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149f21(%rip),%rsi        # 9a94b8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x43b8>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532652,15 +1532652,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149f61(%rip),%rsi        # 9a9610 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x4510>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1532739,15 +1532739,15 @@
 	sub    %rdi,%rsi
 	call   1c2c10 <operator delete(void*, unsigned long)@plt>
 	vpxor  %xmm0,%xmm0,%xmm0
 	mov    $0x4,%edi
 	movq   $0x0,0x10(%rsp)
 	vmovdqa %xmm0,(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	lea    0x149f57(%rip),%rsi        # 9a9770 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool), &fbgemm_gpu::FloatToFP8RowwiseQuantized_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool> >@@Base+0x4670>
 	mov    %rbp,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x10(%rsp)
 	mov    %rdx,0x8(%rsp)
 	call   8180f0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, bool, long), &fbgemm_gpu::FP8rowwise_to_float_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, bool, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0xb5c0>
@@ -1614010,15 +1614010,15 @@
 	movq   $0x0,0x30(%rsp)
 	vmovq  %rbx,%xmm0
 	vpinsrq $0x1,%rax,%xmm0,%xmm0
 	vmovdqu %xmm0,0x20(%r12)
 	vpxor  %xmm0,%xmm0,%xmm0
 	vmovdqa %xmm0,0x20(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
-	movl   $0x9,(%rax)
+	movl   $0xa,(%rax)
 	lea    0x4(%rax),%rdx
 	mov    $0xd8,%edi
 	mov    %rax,0x20(%rsp)
 	mov    %rdx,0x30(%rsp)
 	mov    %rdx,0x28(%rsp)
 	call   1c1910 <operator new(unsigned long)@plt>
 	mov    %rax,%rdx
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -10935,24 +10935,24 @@
   0x0098cb40 78747261 5f6d6574 615f2d3e 73796d62 xtra_meta_->symb
   0x0098cb50 6f6c6963 5f736861 70655f6d 6574615f olic_shape_meta_
   0x0098cb60 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x0098cb70 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x0098cb80 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x0098cb90 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x0098cba0 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x0098cbb0 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x0098cbb0 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x0098cbc0 2f746f72 63682f69 6e636c75 64652f63 /torch/include/c
   0x0098cbd0 31302f63 6f72652f 54656e73 6f72496d 10/core/TensorIm
   0x0098cbe0 706c2e68 223a3137 32332c20 706c6561 pl.h":1723, plea
   0x0098cbf0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0098cc00 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0098cc10 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098cc20 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098cc30 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098cc40 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098cc40 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098cc50 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098cc60 64652f63 31302f63 6f72652f 54656e73 de/c10/core/Tens
   0x0098cc70 6f72496d 706c2e68 00000000 00000000 orImpl.h........
   0x0098cc80 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0098cc90 4d4d2f66 6267656d 6d5f6770 752f636f MM/fbgemm_gpu/co
   0x0098cca0 64656765 6e2f7472 61696e69 6e672f66 degen/training/f
   0x0098ccb0 6f727761 72642f65 6d626564 64696e67 orward/embedding
@@ -11027,15 +11027,15 @@
   0x0098d100 206c6179 6f757420 63616c63 756c6174  layout calculat
   0x0098d110 696f6e20 6c6f6769 632e0000 00000000 ion logic.......
   0x0098d120 69735f6d 6b6c646e 6e282920 494e5445 is_mkldnn() INTE
   0x0098d130 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x0098d140 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x0098d150 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x0098d160 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x0098d170 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x0098d170 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x0098d180 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x0098d190 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x0098d1a0 72652f54 656e736f 72496d70 6c2e6822 re/TensorImpl.h"
   0x0098d1b0 3a313239 302c2070 6c656173 65207265 :1290, please re
   0x0098d1c0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x0098d1d0 546f7263 682e2000 4f706572 61746f72 Torch. .Operator
   0x0098d1e0 73207461 6b696e67 2054656e 736f724f s taking TensorO
@@ -11044,15 +11044,15 @@
   0x0098d210 6e732077 69746820 6f707469 6f6e732e ns with options.
   0x0098d220 72657175 69726573 5f677261 64207365 requires_grad se
   0x0098d230 74206173 20747275 652e2054 68697320 t as true. This 
   0x0098d240 69736e27 7420696d 706c656d 656e7465 isn't implemente
   0x0098d250 64207965 742e0000 2f676974 6875622f d yet.../github/
   0x0098d260 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d270 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d280 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d280 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d290 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d2a0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098d2b0 636f7265 2f436865 636b4d65 6d6f7279 core/CheckMemory
   0x0098d2c0 466f726d 61742e68 00000000 00000000 Format.h........
   0x0098d2d0 63686563 6b5f7465 6e736f72 5f6f7074 check_tensor_opt
   0x0098d2e0 696f6e73 5f616e64 5f657874 72616374 ions_and_extract
   0x0098d2f0 5f6d656d 6f72795f 666f726d 61740000 _memory_format..
@@ -11070,51 +11070,51 @@
   0x0098d3b0 496e7441 72726179 52656620 636f6e74 IntArrayRef cont
   0x0098d3c0 61696e73 20616e20 696e7420 74686174 ains an int that
   0x0098d3d0 2063616e 6e6f7420 62652072 65707265  cannot be repre
   0x0098d3e0 73656e74 65642061 73206120 53796d49 sented as a SymI
   0x0098d3f0 6e743a20 00000000 2f676974 6875622f nt: ..../github/
   0x0098d400 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d410 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d420 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d420 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d430 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d440 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0098d450 6f72652f 53796d49 6e744172 72617952 ore/SymIntArrayR
   0x0098d460 65662e68 0066726f 6d496e74 41727261 ef.h.fromIntArra
   0x0098d470 79526566 536c6f77 00206469 6d732062 yRefSlow. dims b
   0x0098d480 75742074 656e736f 72206861 73200054 ut tensor has .T
   0x0098d490 656e736f 72416363 6573736f 72206578 ensorAccessor ex
   0x0098d4a0 70656374 65642000 61636365 73736f72 pected .accessor
   0x0098d4b0 00000000 00000000 2f676974 6875622f ......../github/
   0x0098d4c0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d4d0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d4e0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d4e0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d4f0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d500 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098d510 636f7265 2f54656e 736f7242 6173652e core/TensorBase.
   0x0098d520 68002d31 00496e64 65782000 20697320 h.-1.Index . is 
   0x0098d530 6f757420 6f662062 6f756e64 733a2000 out of bounds: .
   0x0098d540 2c207261 6e676520 0020746f 20007265 , range . to .re
   0x0098d550 706f7274 5f656d62 65646469 6e675f65 port_embedding_e
   0x0098d560 72726f72 00000000 2f5f5f77 2f464247 rror..../__w/FBG
   0x0098d570 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0098d580 6d5f6770 752f696e 636c7564 652f6662 m_gpu/include/fb
   0x0098d590 67656d6d 5f677075 2f637075 5f757469 gemm_gpu/cpu_uti
   0x0098d5a0 6c732e68 00000000 2f676974 6875622f ls.h..../github/
   0x0098d5b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d5c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d5d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d5d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d5e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d5f0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098d600 636f7265 2f697661 6c75652e 68000000 core/ivalue.h...
   0x0098d610 3020494e 5445524e 414c2041 53534552 0 INTERNAL ASSER
   0x0098d620 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x0098d630 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x0098d640 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x0098d650 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x0098d660 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x0098d660 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x0098d670 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x0098d680 4154656e 2f636f72 652f6976 616c7565 ATen/core/ivalue
   0x0098d690 2e68223a 3635322c 20706c65 61736520 .h":652, please 
   0x0098d6a0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0098d6b0 5079546f 7263682e 20006578 70656374 PyTorch. .expect
   0x0098d6c0 65642069 6e740074 6f496e74 00766563 ed int.toInt.vec
   0x0098d6d0 746f723a 3a5f4d5f 7265616c 6c6f635f tor::_M_realloc_
@@ -11122,25 +11122,25 @@
   0x0098d6f0 2053796d 496e7420 6f722069 6e742062  SymInt or int b
   0x0098d700 75742067 6f742000 69735379 6d496e74 ut got .isSymInt
   0x0098d710 2829207c 7c206973 496e7428 2920494e () || isInt() IN
   0x0098d720 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0098d730 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0098d740 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0098d750 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0098d760 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0098d760 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0098d770 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0098d780 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x0098d790 2f636f72 652f6976 616c7565 5f696e6c /core/ivalue_inl
   0x0098d7a0 2e68223a 3233372c 20706c65 61736520 .h":237, please 
   0x0098d7b0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0098d7c0 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x0098d7d0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098d7e0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098d7f0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098d800 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098d800 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098d810 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098d820 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x0098d830 6c75655f 696e6c2e 6800746f 53796d49 lue_inl.h.toSymI
   0x0098d840 6e740000 00000000 00000000 00000000 nt..............
   0x0098d850 53743139 6261645f 6f707469 6f6e616c St19bad_optional
   0x0098d860 5f616363 65737300 00000000 00000000 _access.........
   0x0098d870 4e336331 30323069 6e747275 73697665 N3c1020intrusive
@@ -11273,28 +11273,28 @@
   0x0098e060 6e642000 20646576 69636573 00676574 nd . devices.get
   0x0098e070 44657669 63654775 61726449 6d706c00 DeviceGuardImpl.
   0x0098e080 5079546f 72636820 6973206e 6f74206c PyTorch is not l
   0x0098e090 696e6b65 64207769 74682073 7570706f inked with suppo
   0x0098e0a0 72742066 6f722000 2f676974 6875622f rt for ./github/
   0x0098e0b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098e0c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098e0d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098e0d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098e0e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098e0f0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0098e100 6f72652f 696d706c 2f446576 69636547 ore/impl/DeviceG
   0x0098e110 75617264 496d706c 496e7465 72666163 uardImplInterfac
   0x0098e120 652e6800 4576656e 74206465 76696365 e.h.Event device
   0x0098e130 20747970 65200062 6c6f636b 00000000  type .block....
   0x0098e140 20646f65 73206e6f 74206d61 74636820  does not match 
   0x0098e150 626c6f63 6b696e67 20737472 65616d27 blocking stream'
   0x0098e160 73206465 76696365 20747970 65200000 s device type ..
   0x0098e170 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098e180 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098e190 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098e1a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098e1a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098e1b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098e1c0 64652f63 31302f63 6f72652f 696d706c de/c10/core/impl
   0x0098e1d0 2f496e6c 696e6545 76656e74 2e680000 /InlineEvent.h..
   0x0098e1e0 45787065 63746564 20216e61 6d652e65 Expected !name.e
   0x0098e1f0 6d707479 28292074 6f206265 20747275 mpty() to be tru
   0x0098e200 652c2062 75742067 6f742066 616c7365 e, but got false
   0x0098e210 2e202028 436f756c 64207468 69732065 .  (Could this e
@@ -11302,49 +11302,49 @@
   0x0098e230 696d7072 6f766564 3f202049 6620736f improved?  If so
   0x0098e240 2c20706c 65617365 20726570 6f727420 , please report 
   0x0098e250 616e2065 6e68616e 63656d65 6e742072 an enhancement r
   0x0098e260 65717565 73742074 6f205079 546f7263 equest to PyTorc
   0x0098e270 682e2900 00000000 2f676974 6875622f h.)...../github/
   0x0098e280 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098e290 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098e2a0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098e2a0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098e2b0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098e2c0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098e2d0 636f7265 2f717561 6c696669 65645f6e core/qualified_n
   0x0098e2e0 616d652e 68000000 496e7661 6c696420 ame.h...Invalid 
   0x0098e2f0 6e616d65 20666f72 20717561 6c696669 name for qualifi
   0x0098e300 6564206e 616d653a 20270000 00000000 ed name: '......
   0x0098e310 2161746f 6d2e656d 70747928 2920494e !atom.empty() IN
   0x0098e320 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0098e330 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0098e340 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0098e350 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0098e360 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0098e360 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0098e370 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0098e380 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x0098e390 2f636f72 652f7175 616c6966 6965645f /core/qualified_
   0x0098e3a0 6e616d65 2e68223a 32342c20 706c6561 name.h":24, plea
   0x0098e3b0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0098e3c0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0098e3d0 2166696e 616c4174 6f6d2e65 6d707479 !finalAtom.empty
   0x0098e3e0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x0098e3f0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x0098e400 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x0098e410 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x0098e420 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x0098e430 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x0098e430 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x0098e440 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x0098e450 2f415465 6e2f636f 72652f71 75616c69 /ATen/core/quali
   0x0098e460 66696564 5f6e616d 652e6822 3a33322c fied_name.h":32,
   0x0098e470 20706c65 61736520 7265706f 72742061  please report a
   0x0098e480 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x0098e490 20000000 00000000 2f676974 6875622f  ......./github/
   0x0098e4a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098e4b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098e4c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098e4c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098e4d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098e4e0 63682f69 6e636c75 64652f63 31302f75 ch/include/c10/u
   0x0098e4f0 74696c2f 41727261 79526566 2e680051 til/ArrayRef.h.Q
   0x0098e500 75616c69 66696564 4e616d65 00626173 ualifiedName.bas
   0x0098e510 69635f73 7472696e 673a3a73 75627374 ic_string::subst
   0x0098e520 72004172 72617952 65663a20 696e7661 r.ArrayRef: inva
   0x0098e530 6c696420 736c6963 652c204e 203d2000 lid slice, N = .
@@ -11355,27 +11355,27 @@
   0x0098e580 77697468 2064696d 656e7369 6f6e733a with dimensions:
   0x0098e590 20000000 00000000 74656e73 6f722e64  .......tensor.d
   0x0098e5a0 696d2829 203d3d20 3020494e 5445524e im() == 0 INTERN
   0x0098e5b0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x0098e5c0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x0098e5d0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x0098e5e0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x0098e5f0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x0098e5f0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x0098e600 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x0098e610 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x0098e620 72632f61 70692f69 6e636c75 64652f74 rc/api/include/t
   0x0098e630 6f726368 2f646574 61696c2f 54656e73 orch/detail/Tens
   0x0098e640 6f724461 7461436f 6e746169 6e65722e orDataContainer.
   0x0098e650 68223a33 31372c20 706c6561 73652072 h":317, please r
   0x0098e660 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0098e670 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0098e680 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098e690 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098e6a0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098e6b0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098e6b0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098e6c0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098e6d0 64652f74 6f726368 2f637372 632f6170 de/torch/csrc/ap
   0x0098e6e0 692f696e 636c7564 652f746f 7263682f i/include/torch/
   0x0098e6f0 64657461 696c2f54 656e736f 72446174 detail/TensorDat
   0x0098e700 61436f6e 7461696e 65722e68 00000000 aContainer.h....
   0x0098e710 20696e20 69747320 66697273 74206469  in its first di
   0x0098e720 6d656e73 696f6e2c 20627574 20676f74 mension, but got
@@ -11384,15 +11384,15 @@
   0x0098e750 697a6573 28295b30 5d203d3d 2028696e izes()[0] == (in
   0x0098e760 7436345f 7429696e 69745f6c 6973745f t64_t)init_list_
   0x0098e770 2e73697a 65282920 494e5445 524e414c .size() INTERNAL
   0x0098e780 20415353 45525420 4641494c 45442061  ASSERT FAILED a
   0x0098e790 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x0098e7a0 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x0098e7b0 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
-  0x0098e7c0 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
+  0x0098e7c0 70797468 6f6e332e 382f7369 74652d70 python3.8/site-p
   0x0098e7d0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x0098e7e0 636c7564 652f746f 7263682f 63737263 clude/torch/csrc
   0x0098e7f0 2f617069 2f696e63 6c756465 2f746f72 /api/include/tor
   0x0098e800 63682f64 65746169 6c2f5465 6e736f72 ch/detail/Tensor
   0x0098e810 44617461 436f6e74 61696e65 722e6822 DataContainer.h"
   0x0098e820 3a333234 2c20706c 65617365 20726570 :324, please rep
   0x0098e830 6f727420 61206275 6720746f 20507954 ort a bug to PyT
@@ -11403,15 +11403,15 @@
   0x0098e880 6f726020 73686f75 6c64206e 6f742062 or` should not b
   0x0098e890 65206361 6c6c6564 00000000 00000000 e called........
   0x0098e8a0 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x0098e8b0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098e8c0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098e8d0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098e8e0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098e8f0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098e8f0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098e900 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098e910 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x0098e920 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x0098e930 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x0098e940 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x0098e950 33382c20 706c6561 73652072 65706f72 38, please repor
   0x0098e960 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11419,15 +11419,15 @@
   0x0098e980 54656e73 6f724461 7461436f 6e746169 TensorDataContai
   0x0098e990 6e657220 74797065 00000000 00000000 ner type........
   0x0098e9a0 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x0098e9b0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098e9c0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098e9d0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098e9e0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098e9f0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098e9f0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098ea00 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098ea10 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x0098ea20 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x0098ea30 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x0098ea40 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x0098ea50 34322c20 706c6561 73652072 65706f72 42, please repor
   0x0098ea60 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11445,15 +11445,15 @@
   0x0098eb20 74686f75 74206c6f 7373206f 6620696e thout loss of in
   0x0098eb30 666f726d 6174696f 6e000000 00000000 formation.......
   0x0098eb40 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x0098eb50 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098eb60 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098eb70 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098eb80 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098eb90 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098eb90 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098eba0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098ebb0 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x0098ebc0 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x0098ebd0 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x0098ebe0 7461436f 6e746169 6e65722e 68223a32 taContainer.h":2
   0x0098ebf0 37322c20 706c6561 73652072 65706f72 72, please repor
   0x0098ec00 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11473,15 +11473,15 @@
   0x0098ece0 3b206974 20697320 6f6e6c79 20666f72 ; it is only for
   0x0098ecf0 20475055 2e000000 6973496e 744c6973  GPU....isIntLis
   0x0098ed00 74282920 494e5445 524e414c 20415353 t() INTERNAL ASS
   0x0098ed10 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x0098ed20 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x0098ed30 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x0098ed40 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x0098ed50 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x0098ed50 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x0098ed60 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x0098ed70 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x0098ed80 75655f69 6e6c2e68 223a3139 36362c20 ue_inl.h":1966, 
   0x0098ed90 706c6561 73652072 65706f72 74206120 please report a 
   0x0098eda0 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x0098edb0 00000000 00000000 76656374 6f723a3a ........vector::
   0x0098edc0 5f4d5f72 616e6765 5f636865 636b3a20 _M_range_check: 
@@ -11508,15 +11508,15 @@
   0x0098ef10 61726775 6d656e74 206f6620 5f5f7365 argument of __se
   0x0098ef20 74737461 74655f5f 2e20476f 74200000 tstate__. Got ..
   0x0098ef30 69735374 72696e67 28292049 4e544552 isString() INTER
   0x0098ef40 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0098ef50 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0098ef60 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0098ef70 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0098ef80 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0098ef80 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0098ef90 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0098efa0 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x0098efb0 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x0098efc0 3a323335 352c2070 6c656173 65207265 :2355, please re
   0x0098efd0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x0098efe0 546f7263 682e2000 2f2f6465 65706c65 Torch. .//deeple
   0x0098eff0 61726e69 6e672f66 6267656d 6d2f6662 arning/fbgemm/fb
@@ -11634,36 +11634,36 @@
   0x0098f6f0 73657473 29202d3e 2054656e 736f7200 sets) -> Tensor.
   0x0098f700 69734765 6e657269 63446963 74282920 isGenericDict() 
   0x0098f710 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x0098f720 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x0098f730 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x0098f740 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x0098f750 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x0098f760 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x0098f760 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x0098f770 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x0098f780 656e2f63 6f72652f 6976616c 75655f69 en/core/ivalue_i
   0x0098f790 6e6c2e68 223a3230 38322c20 706c6561 nl.h":2082, plea
   0x0098f7a0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0098f7b0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0098f7c0 73656c66 5f696d70 6c20494e 5445524e self_impl INTERN
   0x0098f7d0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x0098f7e0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x0098f7f0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x0098f800 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x0098f810 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x0098f810 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x0098f820 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x0098f830 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x0098f840 72632f61 75746f67 7261642f 76617269 rc/autograd/vari
   0x0098f850 61626c65 2e68223a 3330352c 20706c65 able.h":305, ple
   0x0098f860 61736520 7265706f 72742061 20627567 ase report a bug
   0x0098f870 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x0098f880 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098f890 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098f8a0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098f8b0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098f8b0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098f8c0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098f8d0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0098f8e0 746f6772 61642f76 61726961 626c652e tograd/variable.
   0x0098f8f0 68000000 00000000 4f6e6c79 2054656e h.......Only Ten
   0x0098f900 736f7273 206f6620 666c6f61 74696e67 sors of floating
   0x0098f910 20706f69 6e742061 6e642063 6f6d706c  point and compl
   0x0098f920 65782064 74797065 2063616e 20726571 ex dtype can req
@@ -11723,37 +11723,37 @@
   0x0098fc80 73657274 00000000 73636865 6d615f2e sert....schema_.
   0x0098fc90 72657475 726e7328 292e7369 7a652829 returns().size()
   0x0098fca0 203d3d20 3120494e 5445524e 414c2041  == 1 INTERNAL A
   0x0098fcb0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098fcc0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098fcd0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098fce0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098fcf0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098fcf0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098fd00 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098fd10 7564652f 4154656e 2f636f72 652f6275 ude/ATen/core/bu
   0x0098fd20 696c7469 6e5f6675 6e637469 6f6e2e68 iltin_function.h
   0x0098fd30 223a3232 2c20706c 65617365 20726570 ":22, please rep
   0x0098fd40 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x0098fd50 6f726368 2e200000 2f676974 6875622f orch. ../github/
   0x0098fd60 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098fd70 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098fd80 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098fd80 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098fd90 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098fda0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098fdb0 636f7265 2f627569 6c74696e 5f66756e core/builtin_fun
   0x0098fdc0 6374696f 6e2e6800 4275696c 74696e4f ction.h.BuiltinO
   0x0098fdd0 7046756e 6374696f 6e006465 66696e65 pFunction.define
   0x0098fde0 4d657468 6f640000 44656661 756c7420 Method..Default 
   0x0098fdf0 76616c75 6573206d 75737420 62652073 values must be s
   0x0098fe00 70656369 66696564 20666f72 206e6f6e pecified for non
   0x0098fe10 65206f72 20616c6c 20617267 756d656e e or all argumen
   0x0098fe20 74730000 00000000 2f676974 6875622f ts....../github/
   0x0098fe30 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098fe40 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098fe50 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098fe50 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098fe60 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098fe70 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x0098fe80 2f637573 746f6d5f 636c6173 732e6800 /custom_class.h.
   0x0098fe90 54656e73 6f72496d 706c2077 69746820 TensorImpl with 
   0x0098fea0 6e756c6c 70747220 6973206e 6f742073 nullptr is not s
   0x0098feb0 7570706f 72746564 00717565 75650069 upported.queue.i
   0x0098fec0 6e69745f 74656e73 6f720076 6563746f nit_tensor.vecto
@@ -11892,15 +11892,15 @@
   0x00990710 204f626a 65637420 62757420 676f7420  Object but got 
   0x00990720 00746f4f 626a6563 74000000 00000000 .toObject.......
   0x00990730 69734f62 6a656374 28292049 4e544552 isObject() INTER
   0x00990740 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00990750 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00990760 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00990770 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00990780 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00990780 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00990790 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x009907a0 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x009907b0 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x009907c0 3a313333 2c20706c 65617365 20726570 :133, please rep
   0x009907d0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x009907e0 6f726368 2e200000 41726775 6d656e74 orch. ..Argument
   0x009907f0 20706173 73656420 746f2061 74282920  passed to at() 
@@ -11908,15 +11908,15 @@
   0x00990810 61702e00 2f73697a 65002f00 00000000 ap../size./.....
   0x00990820 53747265 616d7320 68617665 2061206d Streams have a m
   0x00990830 6978206f 66206465 76696365 20747970 ix of device typ
   0x00990840 65733a20 73747265 616d2030 20697320 es: stream 0 is 
   0x00990850 6f6e2000 00000000 2f676974 6875622f on ...../github/
   0x00990860 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00990870 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00990880 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00990880 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00990890 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009908a0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x009908b0 6f72652f 696d706c 2f496e6c 696e6553 ore/impl/InlineS
   0x009908c0 74726561 6d477561 72642e68 00207768 treamGuard.h. wh
   0x009908d0 696c6520 73747265 616d2000 20697320 ile stream . is 
   0x009908e0 6f6e2064 65766963 65200067 65744465 on device .getDe
   0x009908f0 76696365 54797065 4f665374 7265616d viceTypeOfStream
@@ -11929,15 +11929,15 @@
   0x00990960 7320616c 72656164 79206d61 726b6564 s already marked
   0x00990970 20636f6d 706c6574 65640000 00000000  completed......
   0x00990980 21636f6d 706c6574 65642829 20494e54 !completed() INT
   0x00990990 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x009909a0 4c454420 61742022 2f676974 6875622f LED at "/github/
   0x009909b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009909c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009909d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009909d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009909e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009909f0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00990a00 636f7265 2f697661 6c75655f 696e6c2e core/ivalue_inl.
   0x00990a10 68223a31 3231352c 20706c65 61736520 h":1215, please 
   0x00990a20 7265706f 72742061 20627567 20746f20 report a bug to 
   0x00990a30 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x00990a40 20776869 63682061 7265206e 6f742061  which are not a
@@ -11973,15 +11973,15 @@
   0x00990c20 6965773c 63686172 3e5d0000 00000000 iew<char>]......
   0x00990c30 20636f75 6c64206e 6f742062 6520636f  could not be co
   0x00990c40 6e766572 74656420 746f2061 6e79206f nverted to any o
   0x00990c50 66207468 65206b6e 6f776e20 74797065 f the known type
   0x00990c60 732e0000 00000000 2f676974 6875622f s......./github/
   0x00990c70 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00990c80 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00990c90 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00990c90 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00990ca0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00990cb0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00990cc0 636f7265 2f6a6974 5f747970 652e6800 core/jit_type.h.
   0x00990cd0 54797065 20000000 636f6e73 74657870 Type ...constexp
   0x00990ce0 72206331 303a3a73 7472696e 675f7669 r c10::string_vi
   0x00990cf0 65772063 31303a3a 7574696c 3a3a6465 ew c10::util::de
   0x00990d00 7461696c 3a3a6675 6c6c795f 7175616c tail::fully_qual
@@ -12043,15 +12043,15 @@
   0x00991080 61696e20 61206375 73746f6d 20636c61 ain a custom cla
   0x00991090 73732100 00000000 69734361 7073756c ss!.....isCapsul
   0x009910a0 65282920 494e5445 524e414c 20415353 e() INTERNAL ASS
   0x009910b0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x009910c0 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x009910d0 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x009910e0 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x009910f0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x009910f0 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x00991100 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00991110 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00991120 75655f69 6e6c2e68 223a3232 352c2070 ue_inl.h":225, p
   0x00991130 6c656173 65207265 706f7274 20612062 lease report a b
   0x00991140 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x00991150 746f4375 73746f6d 436c6173 7300746f toCustomClass.to
   0x00991160 43617073 756c6500 45787065 63746564 Capsule.Expected
@@ -12059,15 +12059,15 @@
   0x00991180 676f7420 00746f54 656e736f 724c6973 got .toTensorLis
   0x00991190 74000000 00000000 69735465 6e736f72 t.......isTensor
   0x009911a0 4c697374 28292049 4e544552 4e414c20 List() INTERNAL 
   0x009911b0 41535345 52542046 41494c45 44206174 ASSERT FAILED at
   0x009911c0 20222f67 69746875 622f686f 6d652f6d  "/github/home/m
   0x009911d0 696e6963 6f6e6461 2f656e76 732f6275 iniconda/envs/bu
   0x009911e0 696c645f 62696e61 72792f6c 69622f70 ild_binary/lib/p
-  0x009911f0 7974686f 6e332e39 2f736974 652d7061 ython3.9/site-pa
+  0x009911f0 7974686f 6e332e38 2f736974 652d7061 ython3.8/site-pa
   0x00991200 636b6167 65732f74 6f726368 2f696e63 ckages/torch/inc
   0x00991210 6c756465 2f415465 6e2f636f 72652f69 lude/ATen/core/i
   0x00991220 76616c75 655f696e 6c2e6822 3a323033 value_inl.h":203
   0x00991230 382c2070 6c656173 65207265 706f7274 8, please report
   0x00991240 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x00991250 682e2000 54726965 6420746f 20636173 h. .Tried to cas
   0x00991260 74206120 44696374 3c003e20 746f2061 t a Dict<.> to a
@@ -12080,36 +12080,36 @@
   0x009912d0 6963742e 696d706c 5f2d3e65 6c656d65 ict.impl_->eleme
   0x009912e0 6e745479 7065732e 6b657954 79706520 ntTypes.keyType 
   0x009912f0 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x00991300 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x00991310 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x00991320 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x00991330 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x00991340 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x00991340 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x00991350 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x00991360 656e2f63 6f72652f 44696374 5f696e6c en/core/Dict_inl
   0x00991370 2e68223a 32362c20 706c6561 73652072 .h":26, please r
   0x00991380 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00991390 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x009913a0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009913b0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009913c0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009913d0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009913d0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009913e0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009913f0 64652f41 54656e2f 636f7265 2f446963 de/ATen/core/Dic
   0x00991400 745f696e 6c2e6800 2a676574 54797065 t_inl.h.*getType
   0x00991410 5074723c 56616c75 653e2829 203d3d20 Ptr<Value>() == 
   0x00991420 2a646963 742e696d 706c5f2d 3e656c65 *dict.impl_->ele
   0x00991430 6d656e74 54797065 732e7661 6c756554 mentTypes.valueT
   0x00991440 79706520 494e5445 524e414c 20415353 ype INTERNAL ASS
   0x00991450 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00991460 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x00991470 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x00991480 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x00991490 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x00991490 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x009914a0 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x009914b0 652f4154 656e2f63 6f72652f 44696374 e/ATen/core/Dict
   0x009914c0 5f696e6c 2e68223a 32372c20 706c6561 _inl.h":27, plea
   0x009914d0 73652072 65706f72 74206120 62756720 se report a bug 
   0x009914e0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x009914f0 4e336331 30313056 616c7565 4572726f N3c1010ValueErro
   0x00991500 72450000 00000000 00000000 00000000 rE..............
@@ -12492,15 +12492,15 @@
   0x00992c90 6a767020 6973206e 6f742069 6d706c65 jvp is not imple
   0x00992ca0 6d656e74 65642066 6f722074 68652063 mented for the c
   0x00992cb0 2b2b2041 5049206f 66206375 73746f6d ++ API of custom
   0x00992cc0 2046756e 6374696f 6e207965 742e0000  Function yet...
   0x00992cd0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00992ce0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00992cf0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00992d00 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00992d00 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00992d10 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00992d20 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x00992d30 746f6772 61642f63 7573746f 6d5f6675 tograd/custom_fu
   0x00992d40 6e637469 6f6e2e68 00000000 00000000 nction.h........
   0x00992d50 636f6d70 696c6564 5f617267 73206e6f compiled_args no
   0x00992d60 7420696d 706c656d 656e7465 6420666f t implemented fo
   0x00992d70 72206e6f 6e2d7472 61636561 626c6520 r non-traceable 
@@ -12540,25 +12540,25 @@
   0x00992f90 6620616c 6c206974 73206368 696c6472 f all its childr
   0x00992fa0 656e0000 00000000 21686173 5f706172 en......!has_par
   0x00992fb0 656e745f 20494e54 45524e41 4c204153 ent_ INTERNAL AS
   0x00992fc0 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x00992fd0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00992fe0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00992ff0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00993000 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00993000 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00993010 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00993020 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x00993030 746f6772 61642f66 756e6374 696f6e2e tograd/function.
   0x00993040 68223a32 36322c20 706c6561 73652072 h":262, please r
   0x00993050 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00993060 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x00993070 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00993080 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00993090 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009930a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009930a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009930b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009930c0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x009930d0 746f6772 61642f66 756e6374 696f6e2e tograd/function.
   0x009930e0 68000000 00000000 2f5f5f77 2f464247 h......./__w/FBG
   0x009930f0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x00993100 6d5f6770 752f636f 64656765 6e2f7472 m_gpu/codegen/tr
   0x00993110 61696e69 6e672f62 61636b77 6172642f aining/backward/
@@ -12582,147 +12582,147 @@
   0x00993230 6374785f 2e6e6f6e 5f646966 66657265 ctx_.non_differe
   0x00993240 6e746961 626c655f 2e656d70 74792829 ntiable_.empty()
   0x00993250 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x00993260 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x00993270 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x00993280 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x00993290 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x009932a0 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x009932a0 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x009932b0 2f746f72 63682f69 6e636c75 64652f74 /torch/include/t
   0x009932c0 6f726368 2f637372 632f6175 746f6772 orch/csrc/autogr
   0x009932d0 61642f63 7573746f 6d5f6675 6e637469 ad/custom_functi
   0x009932e0 6f6e2e68 223a3232 312c2070 6c656173 on.h":221, pleas
   0x009932f0 65207265 706f7274 20612062 75672074 e report a bug t
   0x00993300 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x00993310 6374785f 2e646972 74795f69 6e707574 ctx_.dirty_input
   0x00993320 735f2e65 6d707479 28292049 4e544552 s_.empty() INTER
   0x00993330 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00993340 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00993350 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00993360 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00993370 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00993370 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00993380 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00993390 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x009933a0 7372632f 6175746f 67726164 2f637573 src/autograd/cus
   0x009933b0 746f6d5f 66756e63 74696f6e 2e68223a tom_function.h":
   0x009933c0 3232322c 20706c65 61736520 7265706f 222, please repo
   0x009933d0 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x009933e0 7263682e 20000000 69742021 3d205f73 rch. ...it != _s
   0x009933f0 61766564 5f766172 6961626c 65732e65 aved_variables.e
   0x00993400 6e642829 20494e54 45524e41 4c204153 nd() INTERNAL AS
   0x00993410 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x00993420 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00993430 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00993440 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00993450 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00993450 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00993460 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00993470 64652f74 6f726368 2f637372 632f6479 de/torch/csrc/dy
   0x00993480 6e616d6f 2f636f6d 70696c65 645f6175 namo/compiled_au
   0x00993490 746f6772 61642e68 223a3133 382c2070 tograd.h":138, p
   0x009934a0 6c656173 65207265 706f7274 20612062 lease report a b
   0x009934b0 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x009934c0 6172672e 70726f78 795f7465 6e736f72 arg.proxy_tensor
   0x009934d0 2e646566 696e6564 28292049 4e544552 .defined() INTER
   0x009934e0 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x009934f0 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00993500 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00993510 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00993520 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00993520 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00993530 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00993540 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x00993550 7372632f 64796e61 6d6f2f63 6f6d7069 src/dynamo/compi
   0x00993560 6c65645f 6175746f 67726164 2e68223a led_autograd.h":
   0x00993570 3536312c 20706c65 61736520 7265706f 561, please repo
   0x00993580 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x00993590 7263682e 20000000 6374785f 2e746f5f rch. ...ctx_.to_
   0x009935a0 73617665 5f2e656d 70747928 2920494e save_.empty() IN
   0x009935b0 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x009935c0 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x009935d0 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x009935e0 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x009935f0 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x009935f0 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00993600 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00993610 7263682f 696e636c 7564652f 746f7263 rch/include/torc
   0x00993620 682f6373 72632f61 75746f67 7261642f h/csrc/autograd/
   0x00993630 63757374 6f6d5f66 756e6374 696f6e2e custom_function.
   0x00993640 68223a32 32342c20 706c6561 73652072 h":224, please r
   0x00993650 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00993660 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x00993670 69742021 3d207468 69732d3e 656e6428 it != this->end(
   0x00993680 2920494e 5445524e 414c2041 53534552 ) INTERNAL ASSER
   0x00993690 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x009936a0 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x009936b0 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x009936c0 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x009936d0 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x009936d0 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x009936e0 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x009936f0 746f7263 682f6373 72632f64 796e616d torch/csrc/dynam
   0x00993700 6f2f636f 6d70696c 65645f61 75746f67 o/compiled_autog
   0x00993710 7261642e 68223a37 36302c20 706c6561 rad.h":760, plea
   0x00993720 73652072 65706f72 74206120 62756720 se report a bug 
   0x00993730 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x00993740 6374785f 2e6e6f6e 5f646966 66657265 ctx_.non_differe
   0x00993750 6e746961 626c655f 2e656d70 74792829 ntiable_.empty()
   0x00993760 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x00993770 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x00993780 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x00993790 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x009937a0 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x009937b0 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x009937b0 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x009937c0 2f746f72 63682f69 6e636c75 64652f74 /torch/include/t
   0x009937d0 6f726368 2f637372 632f6175 746f6772 orch/csrc/autogr
   0x009937e0 61642f63 7573746f 6d5f6675 6e637469 ad/custom_functi
   0x009937f0 6f6e2e68 223a3233 312c2070 6c656173 on.h":231, pleas
   0x00993800 65207265 706f7274 20612062 75672074 e report a bug t
   0x00993810 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x00993820 6374785f 2e646972 74795f69 6e707574 ctx_.dirty_input
   0x00993830 735f2e65 6d707479 28292049 4e544552 s_.empty() INTER
   0x00993840 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00993850 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00993860 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00993870 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00993880 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00993880 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00993890 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x009938a0 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x009938b0 7372632f 6175746f 67726164 2f637573 src/autograd/cus
   0x009938c0 746f6d5f 66756e63 74696f6e 2e68223a tom_function.h":
   0x009938d0 3233322c 20706c65 61736520 7265706f 232, please repo
   0x009938e0 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x009938f0 7263682e 20000000 6374785f 2e746f5f rch. ...ctx_.to_
   0x00993900 73617665 5f2e656d 70747928 2920494e save_.empty() IN
   0x00993910 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00993920 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00993930 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00993940 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00993950 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00993950 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00993960 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00993970 7263682f 696e636c 7564652f 746f7263 rch/include/torc
   0x00993980 682f6373 72632f61 75746f67 7261642f h/csrc/autograd/
   0x00993990 63757374 6f6d5f66 756e6374 696f6e2e custom_function.
   0x009939a0 68223a32 33342c20 706c6561 73652072 h":234, please r
   0x009939b0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x009939c0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x009939d0 73796d5f 73697a65 735f696e 64657820 sym_sizes_index 
   0x009939e0 3c207379 6d5f7369 7a65732e 73697a65 < sym_sizes.size
   0x009939f0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x00993a00 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00993a10 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00993a20 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00993a30 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00993a40 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00993a40 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00993a50 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00993a60 2f746f72 63682f63 7372632f 64796e61 /torch/csrc/dyna
   0x00993a70 6d6f2f63 6f6d7069 6c65645f 6175746f mo/compiled_auto
   0x00993a80 67726164 2e68223a 3533312c 20706c65 grad.h":531, ple
   0x00993a90 61736520 7265706f 72742061 20627567 ase report a bug
   0x00993aa0 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x00993ab0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00993ac0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00993ad0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00993ae0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00993ae0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00993af0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00993b00 64652f74 6f726368 2f637372 632f6479 de/torch/csrc/dy
   0x00993b10 6e616d6f 2f636f6d 70696c65 645f6175 namo/compiled_au
   0x00993b20 746f6772 61642e68 006e6578 745f7379 tograd.h.next_sy
   0x00993b30 6d5f7369 7a650000 00000000 00000000 m_size..........
   0x00993b40 50467650 4e35746f 72636838 6175746f PFvPN5torch8auto
   0x00993b50 67726164 344e6f64 65454500 00000000 grad4NodeEE.....
@@ -13004,26 +13004,26 @@
   0x00994c90 04f2c9ff b4f1c9ff 6cf1c9ff 24f1c9ff ........l...$...
   0x00994ca0 c4f0c9ff 34f8c9ff 69734465 76696365 ....4...isDevice
   0x00994cb0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x00994cc0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00994cd0 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00994ce0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00994cf0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00994d00 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00994d00 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00994d10 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00994d20 2f415465 6e2f636f 72652f69 76616c75 /ATen/core/ivalu
   0x00994d30 652e6822 3a393331 2c20706c 65617365 e.h":931, please
   0x00994d40 20726570 6f727420 61206275 6720746f  report a bug to
   0x00994d50 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x00994d60 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x00994d70 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x00994d80 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x00994d90 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x00994da0 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
-  0x00994db0 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
+  0x00994db0 72792f6c 69622f70 7974686f 6e332e38 ry/lib/python3.8
   0x00994dc0 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x00994dd0 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x00994de0 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
   0x00994df0 6c2e6822 3a323033 342c2070 6c656173 l.h":2034, pleas
   0x00994e00 65207265 706f7274 20612062 75672074 e report a bug t
   0x00994e10 6f205079 546f7263 682e2000 746f4465 o PyTorch. .toDe
   0x00994e20 76696365 00000000 00000000 00000000 vice............
@@ -13123,23 +13123,23 @@
   0x00995400 65643f20 20496620 736f2c20 706c6561 ed?  If so, plea
   0x00995410 73652072 65706f72 7420616e 20656e68 se report an enh
   0x00995420 616e6365 6d656e74 20726571 75657374 ancement request
   0x00995430 20746f20 5079546f 7263682e 29000000  to PyTorch.)...
   0x00995440 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00995450 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00995460 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00995470 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00995470 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00995480 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00995490 64652f63 31302f63 6f72652f 53796d42 de/c10/core/SymB
   0x009954a0 6f6f6c2e 68000000 3020494e 5445524e ool.h...0 INTERN
   0x009954b0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x009954c0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x009954d0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x009954e0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x009954f0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x009954f0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x00995500 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x00995510 696e636c 7564652f 4154656e 2f636f72 include/ATen/cor
   0x00995520 652f6976 616c7565 2e68223a 3637362c e/ivalue.h":676,
   0x00995530 20706c65 61736520 7265706f 72742061  please report a
   0x00995540 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x00995550 20000000 00000000 7065726d 7574655f  .......permute_
   0x00995560 706f6f6c 65645f65 6d627320 646f6573 pooled_embs does
@@ -13159,25 +13159,25 @@
   0x00995640 68656d61 20726567 69737465 72656420 hema registered 
   0x00995650 79657400 00000000 73636865 6d615f2e yet.....schema_.
   0x00995660 6861735f 76616c75 65282920 494e5445 has_value() INTE
   0x00995670 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00995680 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00995690 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x009956a0 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x009956b0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x009956b0 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x009956c0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x009956d0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x009956e0 6f72652f 64697370 61746368 2f4f7065 ore/dispatch/Ope
   0x009956f0 7261746f 72456e74 72792e68 223a3830 ratorEntry.h":80
   0x00995700 2c20706c 65617365 20726570 6f727420 , please report 
   0x00995710 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00995720 2e200000 00000000 2f676974 6875622f . ....../github/
   0x00995730 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00995740 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00995750 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00995750 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00995760 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00995770 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00995780 636f7265 2f646973 70617463 682f4f70 core/dispatch/Op
   0x00995790 65726174 6f72456e 7472792e 68007363 eratorEntry.h.sc
   0x009957a0 68656d61 00000000 00000000 00000000 hema............
   0x009957b0 00000000 00000000 00000000 00000000 ................
   0x009957c0 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -13685,15 +13685,15 @@
   0x00997720 62617463 6865645f 64656e73 655f7665 batched_dense_ve
   0x00997730 635f6a61 67676564 5f32645f 6d756c00 c_jagged_2d_mul.
   0x00997740 69734c69 73742829 20494e54 45524e41 isList() INTERNA
   0x00997750 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x00997760 61742022 2f676974 6875622f 686f6d65 at "/github/home
   0x00997770 2f6d696e 69636f6e 64612f65 6e76732f /miniconda/envs/
   0x00997780 6275696c 645f6269 6e617279 2f6c6962 build_binary/lib
-  0x00997790 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
+  0x00997790 2f707974 686f6e33 2e382f73 6974652d /python3.8/site-
   0x009977a0 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x009977b0 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x009977c0 2f697661 6c75655f 696e6c2e 68223a32 /ivalue_inl.h":2
   0x009977d0 3036362c 20706c65 61736520 7265706f 066, please repo
   0x009977e0 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x009977f0 7263682e 20000000 2f5f5f77 2f464247 rch. .../__w/FBG
   0x00997800 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
@@ -13770,24 +13770,24 @@
   0x00997c70 75742067 6f742000 69735379 6d496e74 ut got .isSymInt
   0x00997c80 4c697374 2829207c 7c206973 496e744c List() || isIntL
   0x00997c90 69737428 2920494e 5445524e 414c2041 ist() INTERNAL A
   0x00997ca0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00997cb0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00997cc0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00997cd0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00997ce0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00997ce0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00997cf0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00997d00 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
   0x00997d10 616c7565 5f696e6c 2e68223a 31393738 alue_inl.h":1978
   0x00997d20 2c20706c 65617365 20726570 6f727420 , please report 
   0x00997d30 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00997d40 2e200000 00000000 2f676974 6875622f . ....../github/
   0x00997d50 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00997d60 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00997d70 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00997d70 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00997d80 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00997d90 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x00997da0 6f72652f 53796d49 6e742e68 00000000 ore/SymInt.h....
   0x00997db0 45787065 63746564 2064656e 73655f76 Expected dense_v
   0x00997dc0 616c7565 735f6772 61642e73 796d5f73 alues_grad.sym_s
   0x00997dd0 697a6573 2829203d 3d206465 6e73655f izes() == dense_
   0x00997de0 73686170 6520746f 20626520 74727565 shape to be true
@@ -13896,15 +13896,15 @@
   0x00998450 74797065 20776974 6820636f 6e746169 type with contai
   0x00998460 6e656420 74797065 73206469 64206e6f ned types did no
   0x00998470 74206f76 65726c6f 61642063 72656174 t overload creat
   0x00998480 65576974 68436f6e 7461696e 65643a20 eWithContained: 
   0x00998490 00000000 00000000 2f676974 6875622f ......../github/
   0x009984a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009984b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009984c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009984c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009984d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009984e0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009984f0 636f7265 2f6a6974 5f747970 655f6261 core/jit_type_ba
   0x00998500 73652e68 00637265 61746557 69746843 se.h.createWithC
   0x00998510 6f6e7461 696e6564 003b204c 656e6774 ontained.; Lengt
   0x00998520 68203d20 00000000 41727261 79526566 h = ....ArrayRef
   0x00998530 3a20696e 76616c69 6420696e 64657820 : invalid index 
@@ -14488,35 +14488,35 @@
   0x0099a950 45450000 00000000 00000000 78000000 EE..........x...
   0x0099a960 69735379 6d496e74 2829207c 7c206973 isSymInt() || is
   0x0099a970 496e7428 2920494e 5445524e 414c2041 Int() INTERNAL A
   0x0099a980 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0099a990 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0099a9a0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0099a9b0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0099a9c0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0099a9c0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0099a9d0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0099a9e0 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
   0x0099a9f0 616c7565 5f696e6c 2e68223a 3234352c alue_inl.h":245,
   0x0099aa00 20706c65 61736520 7265706f 72742061  please report a
   0x0099aa10 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x0099aa20 20005472 69656420 746f2063 61737420  .Tried to cast 
   0x0099aa30 61204c69 73743c00 3e20746f 2061204c a List<.> to a L
   0x0099aa40 6973743c 003e2e20 54797065 73206d69 ist<.>. Types mi
   0x0099aa50 736d6174 63682e00 746f5479 7065644c smatch..toTypedL
   0x0099aa60 69737400 00000000 2f676974 6875622f ist...../github/
   0x0099aa70 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0099aa80 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0099aa90 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0099aa90 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0099aaa0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0099aab0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0099aac0 636f7265 2f4c6973 745f696e 6c2e6800 core/List_inl.h.
   0x0099aad0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0099aae0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0099aaf0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0099ab00 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0099ab00 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0099ab10 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0099ab20 64652f41 54656e2f 636f7265 2f626f78 de/ATen/core/box
   0x0099ab30 696e672f 4b65726e 656c4675 6e637469 ing/KernelFuncti
   0x0099ab40 6f6e5f69 6d706c2e 68000000 00000000 on_impl.h.......
   0x0099ab50 45787065 63746564 20707472 5f2d3e69 Expected ptr_->i
   0x0099ab60 735f666c 6f617428 2920746f 20626520 s_float() to be 
   0x0099ab70 74727565 2c206275 7420676f 74206661 true, but got fa
@@ -14525,24 +14525,24 @@
   0x0099aba0 62652069 6d70726f 7665643f 20204966 be improved?  If
   0x0099abb0 20736f2c 20706c65 61736520 7265706f  so, please repo
   0x0099abc0 72742061 6e20656e 68616e63 656d656e rt an enhancemen
   0x0099abd0 74207265 71756573 7420746f 20507954 t request to PyT
   0x0099abe0 6f726368 2e290000 2f676974 6875622f orch.)../github/
   0x0099abf0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0099ac00 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0099ac10 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0099ac10 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0099ac20 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0099ac30 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0099ac40 6f72652f 53796d46 6c6f6174 2e680000 ore/SymFloat.h..
   0x0099ac50 3020494e 5445524e 414c2041 53534552 0 INTERNAL ASSER
   0x0099ac60 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x0099ac70 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x0099ac80 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x0099ac90 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x0099aca0 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x0099aca0 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x0099acb0 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x0099acc0 4154656e 2f636f72 652f6976 616c7565 ATen/core/ivalue
   0x0099acd0 2e68223a 3534302c 20706c65 61736520 .h":540, please 
   0x0099ace0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0099acf0 5079546f 7263682e 20006578 70656374 PyTorch. .expect
   0x0099ad00 65642064 6f75626c 6500746f 446f7562 ed double.toDoub
   0x0099ad10 6c650000 00000000 00000000 00000000 le..............
@@ -16008,15 +16008,15 @@
   0x009a0850 6a616767 65645f69 6e646578 5f616464 jagged_index_add
   0x009a0860 5f32645f 666f7277 61726400 00000000 _2d_forward.....
   0x009a0870 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x009a0880 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x009a0890 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x009a08a0 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x009a08b0 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x009a08c0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x009a08c0 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x009a08d0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x009a08e0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x009a08f0 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
   0x009a0900 223a3139 36322c20 706c6561 73652072 ":1962, please r
   0x009a0910 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x009a0920 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x009a0930 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -20225,15 +20225,15 @@
   0x009b0fe0 726f7665 643f2020 49662073 6f2c2070 roved?  If so, p
   0x009b0ff0 6c656173 65207265 706f7274 20616e20 lease report an 
   0x009b1000 656e6861 6e63656d 656e7420 72657175 enhancement requ
   0x009b1010 65737420 746f2050 79546f72 63682e29 est to PyTorch.)
   0x009b1020 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009b1030 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b1040 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b1050 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b1050 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b1060 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b1070 656d6265 6464696e 675f666f 72776172 embedding_forwar
   0x009b1080 645f7175 616e7469 7a65645f 756e7765 d_quantized_unwe
   0x009b1090 69676874 65645f63 6f646567 656e5f63 ighted_codegen_c
   0x009b10a0 70752e63 70700000 696e7438 206f7574 pu.cpp..int8 out
   0x009b10b0 70757420 61726520 6f6e6c79 20737570 put are only sup
   0x009b10c0 706f7274 65642066 6f722069 6e743820 ported for int8 
@@ -20366,15 +20366,15 @@
   0x009b18b0 98bff2ff 88bff2ff 78bff2ff 68bff2ff ........x...h...
   0x009b18c0 d8c0f2ff c8c0f2ff b8c0f2ff a8c0f2ff ................
   0x009b18d0 d8bff2ff c8bff2ff b8bff2ff a8bff2ff ................
   0x009b18e0 38bff2ff 28bff2ff 48bff2ff 06050010 8...(...H.......
   0x009b18f0 110f0000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009b1900 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b1910 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b1920 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b1920 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b1930 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b1940 656d6265 6464696e 675f666f 72776172 embedding_forwar
   0x009b1950 645f7175 616e7469 7a65645f 77656967 d_quantized_weig
   0x009b1960 68746564 5f636f64 6567656e 5f637075 hted_codegen_cpu
   0x009b1970 2e637070 00000000 7072756e 65645f68 .cpp....pruned_h
   0x009b1980 6173686d 61705f6c 6f6f6b75 705f7765 ashmap_lookup_we
   0x009b1990 69676874 65645f63 70750000 00000000 ighted_cpu......
@@ -20388,15 +20388,15 @@
   0x009b1a10 75737420 62652065 6d707479 206f7220 ust be empty or 
   0x009b1a20 61204350 55207465 6e736f72 3b206974 a CPU tensor; it
   0x009b1a30 20697320 63757272 656e746c 79206f6e  is currently on
   0x009b1a40 20646576 69636520 00000000 00000000  device ........
   0x009b1a50 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b1a60 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b1a70 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b1a80 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b1a80 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b1a90 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b1aa0 675f6261 636b7761 72645f64 656e7365 g_backward_dense
   0x009b1ab0 5f73706c 69745f63 70752e63 70700000 _split_cpu.cpp..
   0x009b1ac0 43686563 6b206661 696c6564 3a20686f Check failed: ho
   0x009b1ad0 73745f77 65696768 74732e64 696d2829 st_weights.dim()
   0x009b1ae0 203d3d20 31202800 73706c69 745f656d  == 1 (.split_em
   0x009b1af0 62656464 696e675f 6261636b 77617264 bedding_backward
@@ -20477,15 +20477,15 @@
   0x009b1fa0 70706572 00000000 73706c69 745f656d pper....split_em
   0x009b1fb0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b1fc0 666f7277 6172645f 756e7765 69676874 forward_unweight
   0x009b1fd0 65645f70 74325f77 72617070 65720000 ed_pt2_wrapper..
   0x009b1fe0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b1ff0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b2000 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b2010 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b2010 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b2020 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b2030 675f666f 72776172 645f7370 6c69745f g_forward_split_
   0x009b2040 7074325f 6370755f 77726170 7065722e pt2_cpu_wrapper.
   0x009b2050 63707000 00000000 66626765 6d6d3a3a cpp.....fbgemm::
   0x009b2060 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b2070 636f6465 67656e5f 67726164 5f696e64 codegen_grad_ind
   0x009b2080 6963655f 77656967 6874735f 63707500 ice_weights_cpu.
@@ -20616,15 +20616,15 @@
   0x009b2850 3d302920 2d3e2054 656e736f 72000000 =0) -> Tensor...
   0x009b2860 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b2870 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x009b2880 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x009b2890 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x009b28a0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b28b0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b28c0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b28c0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b28d0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b28e0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b28f0 72645f73 706c6974 5f616461 67726164 rd_split_adagrad
   0x009b2900 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009b2910 66626765 6d6d3a3a 73706c69 745f656d fbgemm::split_em
   0x009b2920 62656464 696e675f 6261636b 77617264 bedding_backward
   0x009b2930 5f636f64 6567656e 5f616461 67726164 _codegen_adagrad
@@ -20739,15 +20739,15 @@
   0x009b3000 9038f5ff 7838f5ff 6038f5ff 4838f5ff .8..x8..`8..H8..
   0x009b3010 3038f5ff 1838f5ff 0038f5ff f037f5ff 08...8...8...7..
   0x009b3020 e037f5ff d037f5ff c037f5ff b037f5ff .7...7...7...7..
   0x009b3030 a037f5ff 7837f5ff c839f5ff 00000000 .7..x7...9......
   0x009b3040 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b3050 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b3060 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b3070 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b3070 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b3080 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b3090 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b30a0 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x009b30b0 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x009b30c0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b30d0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009b30e0 5f616461 67726164 5f776569 67687465 _adagrad_weighte
@@ -20861,15 +20861,15 @@
   0x009b37a0 00000000 00000000 73706c69 745f656d ........split_em
   0x009b37b0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b37c0 6c6f6f6b 75705f72 6f777769 73655f61 lookup_rowwise_a
   0x009b37d0 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x009b37e0 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x009b37f0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b3800 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b3810 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b3810 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b3820 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b3830 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b3840 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b3850 5f616461 67726164 5f637075 2e637070 _adagrad_cpu.cpp
   0x009b3860 00000000 00000000 66626765 6d6d3a3a ........fbgemm::
   0x009b3870 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b3880 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -20989,15 +20989,15 @@
   0x009b3fa0 4c88f6ff 3488f6ff 1c88f6ff 0488f6ff L...4...........
   0x009b3fb0 ec87f6ff d487f6ff bc87f6ff a487f6ff ................
   0x009b3fc0 8c87f6ff 7487f6ff 6487f6ff 5487f6ff ....t...d...T...
   0x009b3fd0 4487f6ff 3487f6ff 2487f6ff 1487f6ff D...4...$.......
   0x009b3fe0 ec86f6ff 3c89f6ff 2f5f5f77 2f464247 ....<.../__w/FBG
   0x009b3ff0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b4000 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b4010 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b4010 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b4020 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b4030 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b4040 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b4050 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x009b4060 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x009b4070 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b4080 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -21101,15 +21101,15 @@
   0x009b46a0 745f6474 7970653d 3029202d 3e205465 t_dtype=0) -> Te
   0x009b46b0 6e736f72 00000000 73706c69 745f656d nsor....split_em
   0x009b46c0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b46d0 6c6f6f6b 75705f73 67645f66 756e6374 lookup_sgd_funct
   0x009b46e0 696f6e5f 63707500 2f5f5f77 2f464247 ion_cpu./__w/FBG
   0x009b46f0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b4700 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b4710 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b4710 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b4720 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b4730 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b4740 72645f73 706c6974 5f736764 5f637075 rd_split_sgd_cpu
   0x009b4750 2e637070 00000000 66626765 6d6d3a3a .cpp....fbgemm::
   0x009b4760 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b4770 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009b4780 5f736764 5f637075 00000000 00000000 _sgd_cpu........
@@ -21217,15 +21217,15 @@
   0x009b4de0 90b7f7ff 78b7f7ff 60b7f7ff 48b7f7ff ....x...`...H...
   0x009b4df0 30b7f7ff 18b7f7ff 00b7f7ff f0b6f7ff 0...............
   0x009b4e00 e0b6f7ff d0b6f7ff c0b6f7ff b0b6f7ff ................
   0x009b4e10 a0b6f7ff 78b6f7ff c8b8f7ff 00000000 ....x...........
   0x009b4e20 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b4e30 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b4e40 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b4e50 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b4e50 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b4e60 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b4e70 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b4e80 5f736764 5f707432 5f637075 5f777261 _sgd_pt2_cpu_wra
   0x009b4e90 70706572 2e637070 00000000 00000000 pper.cpp........
   0x009b4ea0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b4eb0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009b4ec0 5f736764 5f776569 67687465 645f6578 _sgd_weighted_ex
@@ -21297,15 +21297,15 @@
   0x009b52e0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b52f0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b5300 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b5310 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b5320 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b5330 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b5340 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b5350 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b5350 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b5360 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b5370 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b5380 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x009b5390 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b53a0 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x009b53b0 64616d5f 66756e63 74696f6e 5f637075 dam_function_cpu
   0x009b53c0 00000000 00000000 73706c69 745f656d ........split_em
@@ -21402,15 +21402,15 @@
   0x009b5970 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x009b5980 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x009b5990 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x009b59a0 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x009b59b0 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x009b59c0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b59d0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b59e0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b59e0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b59f0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b5a00 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b5a10 72645f73 706c6974 5f6c616d 625f6370 rd_split_lamb_cp
   0x009b5a20 752e6370 70000000 73706c69 745f656d u.cpp...split_em
   0x009b5a30 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b5a40 6c6f6f6b 75705f6c 616d625f 66756e63 lookup_lamb_func
   0x009b5a50 74696f6e 5f637075 00000000 00000000 tion_cpu........
@@ -21501,15 +21501,15 @@
   0x009b5fa0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b5fb0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b5fc0 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b5fd0 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b5fe0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b5ff0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b6000 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b6010 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b6010 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b6020 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b6030 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b6040 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x009b6050 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x009b6060 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b6070 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x009b6080 61727469 616c5f72 6f777769 73655f61 artial_rowwise_a
@@ -21604,15 +21604,15 @@
   0x009b6610 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b6620 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b6630 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b6640 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b6650 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b6660 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b6670 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b6680 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b6680 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b6690 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b66a0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b66b0 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x009b66c0 5f6c616d 625f6370 752e6370 70000000 _lamb_cpu.cpp...
   0x009b66d0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b66e0 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x009b66f0 61727469 616c5f72 6f777769 73655f6c artial_rowwise_l
@@ -21707,15 +21707,15 @@
   0x009b6c80 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x009b6c90 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x009b6ca0 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x009b6cb0 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x009b6cc0 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x009b6cd0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b6ce0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b6cf0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b6cf0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b6d00 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b6d10 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b6d20 72645f73 706c6974 5f6c6172 735f7367 rd_split_lars_sg
   0x009b6d30 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x009b6d40 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b6d50 636f6465 67656e5f 6c6f6f6b 75705f6c codegen_lookup_l
   0x009b6d60 6172735f 7367645f 66756e63 74696f6e ars_sgd_function
@@ -21806,15 +21806,15 @@
   0x009b72b0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b72c0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b72d0 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b72e0 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b72f0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b7300 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b7310 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b7320 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b7320 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b7330 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b7340 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b7350 5f6e6f6e 655f6370 752e6370 70000000 _none_cpu.cpp...
   0x009b7360 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b7370 636f6465 67656e5f 6c6f6f6b 75705f6e codegen_lookup_n
   0x009b7380 6f6e655f 66756e63 74696f6e 5f637075 one_function_cpu
   0x009b7390 00000000 00000000 73706c69 745f656d ........split_em
@@ -21892,15 +21892,15 @@
   0x009b7810 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x009b7820 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x009b7830 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x009b7840 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x009b7850 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x009b7860 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b7870 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b7880 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b7880 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b7890 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b78a0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b78b0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b78c0 5f616461 67726164 5f776974 685f636f _adagrad_with_co
   0x009b78d0 756e7465 725f6370 752e6370 70000000 unter_cpu.cpp...
   0x009b78e0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b78f0 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -22034,15 +22034,15 @@
   0x009b80f0 2f676974 6875622e 636f6d2f 7079746f /github.com/pyto
   0x009b8100 7263682f 46424745 4d4d2f64 69736375 rch/FBGEMM/discu
   0x009b8110 7373696f 6e732f31 37323720 666f7220 ssions/1727 for 
   0x009b8120 6d6f7265 20646574 61696c2e 00000000 more detail.....
   0x009b8130 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b8140 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b8150 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b8160 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b8160 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b8170 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b8180 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b8190 5f617070 726f785f 7367645f 6370752e _approx_sgd_cpu.
   0x009b81a0 63707000 00000000 73706c69 745f656d cpp.....split_em
   0x009b81b0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b81c0 6c6f6f6b 75705f61 7070726f 785f7367 lookup_approx_sg
   0x009b81d0 645f6675 6e637469 6f6e5f63 70750000 d_function_cpu..
@@ -22115,15 +22115,15 @@
   0x009b8600 70733a2f 2f676974 6875622e 636f6d2f ps://github.com/
   0x009b8610 7079746f 7263682f 46424745 4d4d2f64 pytorch/FBGEMM/d
   0x009b8620 69736375 7373696f 6e732f31 37323720 iscussions/1727 
   0x009b8630 666f7220 6d6f7265 20646574 61696c2e for more detail.
   0x009b8640 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009b8650 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b8660 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b8670 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b8670 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b8680 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b8690 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b86a0 72645f73 706c6974 5f617070 726f785f rd_split_approx_
   0x009b86b0 726f7777 6973655f 61646167 7261645f rowwise_adagrad_
   0x009b86c0 6370752e 63707000 73706c69 745f656d cpu.cpp.split_em
   0x009b86d0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b86e0 6c6f6f6b 75705f61 7070726f 785f726f lookup_approx_ro
@@ -22218,15 +22218,15 @@
   0x009b8c70 2f2f6769 74687562 2e636f6d 2f707974 //github.com/pyt
   0x009b8c80 6f726368 2f464247 454d4d2f 64697363 orch/FBGEMM/disc
   0x009b8c90 75737369 6f6e732f 31373237 20666f72 ussions/1727 for
   0x009b8ca0 206d6f72 65206465 7461696c 2e000000  more detail....
   0x009b8cb0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b8cc0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b8cd0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b8ce0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b8ce0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b8cf0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b8d00 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b8d10 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x009b8d20 61646167 7261645f 77697468 5f636f75 adagrad_with_cou
   0x009b8d30 6e746572 5f637075 2e637070 00000000 nter_cpu.cpp....
   0x009b8d40 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b8d50 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
@@ -22354,15 +22354,15 @@
   0x009b94f0 69746875 622e636f 6d2f7079 746f7263 ithub.com/pytorc
   0x009b9500 682f4642 47454d4d 2f646973 63757373 h/FBGEMM/discuss
   0x009b9510 696f6e73 2f313732 3720666f 72206d6f ions/1727 for mo
   0x009b9520 72652064 65746169 6c2e0000 00000000 re detail.......
   0x009b9530 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b9540 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b9550 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b9560 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b9560 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b9570 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b9580 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b9590 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x009b95a0 61646167 7261645f 77697468 5f776569 adagrad_with_wei
   0x009b95b0 6768745f 64656361 795f6370 752e6370 ght_decay_cpu.cp
   0x009b95c0 70000000 00000000 73706c69 745f656d p.......split_em
   0x009b95d0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -22454,15 +22454,15 @@
   0x009b9b30 68747470 733a2f2f 67697468 75622e63 https://github.c
   0x009b9b40 6f6d2f70 79746f72 63682f46 4247454d om/pytorch/FBGEM
   0x009b9b50 4d2f6469 73637573 73696f6e 732f3137 M/discussions/17
   0x009b9b60 32372066 6f72206d 6f726520 64657461 27 for more deta
   0x009b9b70 696c2e00 00000000 2f5f5f77 2f464247 il....../__w/FBG
   0x009b9b80 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b9b90 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b9ba0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b9ba0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b9bb0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b9bc0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b9bd0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b9be0 5f616461 67726164 5f776974 685f7765 _adagrad_with_we
   0x009b9bf0 69676874 5f646563 61795f63 70752e63 ight_decay_cpu.c
   0x009b9c00 70700000 00000000 73706c69 745f656d pp......split_em
   0x009b9c10 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -22553,15 +22553,15 @@
   0x009ba160 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x009ba170 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x009ba180 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x009ba190 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x009ba1a0 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x009ba1b0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009ba1c0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009ba1d0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009ba1d0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009ba1e0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009ba1f0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009ba200 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009ba210 5f776569 67687465 645f6164 61677261 _weighted_adagra
   0x009ba220 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x009ba230 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009ba240 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -22654,15 +22654,15 @@
   0x009ba7b0 a86af9ff 906af9ff 786af9ff 606af9ff .j...j..xj..`j..
   0x009ba7c0 486af9ff 306af9ff 186af9ff 006af9ff Hj..0j...j...j..
   0x009ba7d0 e869f9ff d869f9ff c869f9ff b869f9ff .i...i...i...i..
   0x009ba7e0 a869f9ff 9869f9ff 8869f9ff 6069f9ff .i...i...i..`i..
   0x009ba7f0 b06bf9ff 00000000 2f5f5f77 2f464247 .k....../__w/FBG
   0x009ba800 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009ba810 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009ba820 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009ba820 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009ba830 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009ba840 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009ba850 72645f61 64616772 61645f73 706c6974 rd_adagrad_split
   0x009ba860 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009ba870 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009ba880 6261636b 77617264 5f657861 63745f63 backward_exact_c
   0x009ba890 70755f6f 75746572 00000000 00000000 pu_outer........
@@ -22741,15 +22741,15 @@
   0x009bad20 c8eef9ff b8eef9ff a8eef9ff 80eef9ff ................
   0x009bad30 d0f0f9ff 00000000 6e756d20 6f662072 ........num of r
   0x009bad40 6f777320 70726f63 65737365 64206279 ows processed by
   0x009bad50 20616461 67726164 3a200000 00000000  adagrad: ......
   0x009bad60 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009bad70 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009bad80 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009bad90 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009bad90 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009bada0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009badb0 675f6261 636b7761 72645f72 6f777769 g_backward_rowwi
   0x009badc0 73655f61 64616772 61645f73 706c6974 se_adagrad_split
   0x009badd0 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009bade0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009badf0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009bae00 5f726f77 77697365 5f616461 67726164 _rowwise_adagrad
@@ -22821,15 +22821,15 @@
   0x009bb220 1c52faff 0452faff ec51faff d451faff .R...R...Q...Q..
   0x009bb230 bc51faff a451faff 8c51faff 7451faff .Q...Q...Q..tQ..
   0x009bb240 5c51faff 4451faff 3451faff 2451faff \Q..DQ..4Q..$Q..
   0x009bb250 1451faff 0451faff f450faff e450faff .Q...Q...P...P..
   0x009bb260 bc50faff 0c53faff 2f5f5f77 2f464247 .P...S../__w/FBG
   0x009bb270 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009bb280 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009bb290 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009bb290 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009bb2a0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009bb2b0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009bb2c0 72645f73 67645f73 706c6974 5f637075 rd_sgd_split_cpu
   0x009bb2d0 2e637070 00000000 73706c69 745f656d .cpp....split_em
   0x009bb2e0 62656464 696e675f 6261636b 77617264 bedding_backward
   0x009bb2f0 5f636f64 6567656e 5f736764 5f637075 _codegen_sgd_cpu
   0x009bb300 2854656e 736f7220 67726164 5f6f7574 (Tensor grad_out
```

## fbgemm_gpu/sparse_ops.py

```diff
@@ -98,14 +98,51 @@
     permuted_weights = None
     if weights is not None:
         # pyre-fixme
         permuted_weights = weights.new_empty(permuted_indices_size)
     return permuted_lengths, permuted_indices, permuted_weights
 
 
+@impl_abstract("fbgemm::invert_permute")
+def invert_permute_abstract(permute: Tensor) -> Tensor:
+    return torch.empty_like(permute)
+
+
+# pyre-ignore
+def permute_2D_sparse_data_setup_context(ctx, inputs, output):
+    permute, lengths, values, weights, permuted_lengths_sum = inputs
+    permuted_lengths, permuted_values, permuted_weights = output
+    ctx.permute = permute
+    ctx.permuted_lengths = permuted_lengths
+
+
+# pyre-ignore
+def permute_2D_sparse_data_backward(ctx, grad_lengths, grad_values, grad_weights):
+    inv_permute = torch.ops.fbgemm.invert_permute(ctx.permute)
+    permuted_grad_lengths, permuted_grad_values, permuted_grad_weights = (
+        torch.ops.fbgemm.permute_2D_sparse_data(
+            inv_permute, ctx.permuted_lengths, grad_values, grad_weights
+        )
+    )
+    return (
+        None,
+        permuted_grad_lengths,
+        permuted_grad_values,
+        permuted_grad_weights,
+        None,
+    )
+
+
+torch.library.register_autograd(
+    "fbgemm::permute_2D_sparse_data",
+    permute_2D_sparse_data_backward,
+    setup_context=permute_2D_sparse_data_setup_context,
+)
+
+
 @impl_abstract("fbgemm::permute_1D_sparse_data")
 def permute_1D_sparse_data_meta(
     permute: Tensor,
     lengths: Tensor,
     values: Tensor,
     weights: Optional[Tensor] = None,
     permuted_lengths_sum: Optional[int] = None,
```

## fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py

```diff
@@ -13,15 +13,15 @@
 import logging
 from math import log2
 from typing import List, Optional, Tuple
 
 import torch  # usort:skip
 
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers as invokers
-from fbgemm_gpu.split_embedding_configs import SparseType
+from fbgemm_gpu.split_embedding_configs import EmbOptimType as OptimType, SparseType
 
 from fbgemm_gpu.split_table_batched_embeddings_ops_common import (
     CacheAlgorithm,
     DEFAULT_SCALE_BIAS_SIZE_IN_BYTES,
     EmbeddingLocation,
     PoolingMode,
 )
@@ -89,14 +89,15 @@
         ssd_compaction_trigger: int = 8,
         ssd_write_buffer_size: int = 2 * 1024 * 1024 * 1024,
         ssd_max_write_buffer_num: int = 16,
         ssd_cache_location: EmbeddingLocation = EmbeddingLocation.MANAGED,
         ssd_uniform_init_lower: float = -0.01,
         ssd_uniform_init_upper: float = 0.01,
         ssd_block_cache_size: int = 0,
+        optimizer: OptimType = OptimType.EXACT_ROWWISE_ADAGRAD,
         # General Optimizer args
         stochastic_rounding: bool = True,
         gradient_clipping: bool = False,
         max_gradient: float = 1.0,
         max_norm: float = 0.0,
         learning_rate: float = 0.01,
         eps: float = 1.0e-8,  # used by Adagrad, LAMB, and Adam
@@ -238,28 +239,31 @@
         )
         # pyre-fixme[20]: Argument `self` expected.
         (low_priority, high_priority) = torch.cuda.Stream.priority_range()
         self.ssd_stream = torch.cuda.Stream(priority=low_priority)
         self.ssd_set_start = torch.cuda.Event()
         self.ssd_set_end = torch.cuda.Event()
         self.timesteps_prefetched: List[int] = []
+        self.ssd_scratch_pads: List[Tuple[Tensor, Tensor, Tensor]] = []
+        # TODO: add type annotation
+        self.ssd_prefetch_data = []
 
         if weight_decay_mode == WeightDecayMode.COUNTER or counter_based_regularization:
             raise AssertionError(
                 "weight_decay_mode = WeightDecayMode.COUNTER is not supported for SSD TBE."
             )
         counter_based_regularization = CounterBasedRegularizationDefinition()
 
         if weight_decay_mode == WeightDecayMode.COWCLIP or cowclip_regularization:
             raise AssertionError(
                 "weight_decay_mode = WeightDecayMode.COWCLIP is not supported for SSD TBE."
             )
         cowclip_regularization = CowClipDefinition()
 
-        self.optimizer_args = invokers.lookup_args.OptimizerArgs(
+        self.optimizer_args = invokers.lookup_args_ssd.OptimizerArgs(
             stochastic_rounding=stochastic_rounding,
             gradient_clipping=gradient_clipping,
             max_gradient=max_gradient,
             max_norm=max_norm,
             learning_rate=learning_rate,
             eps=eps,
             beta1=beta1,
@@ -297,17 +301,18 @@
         self.register_buffer(
             "weights_placements",
             torch.tensor(
                 [EmbeddingLocation.MANAGED_CACHING for _ in range(T_)],
                 dtype=torch.int32,
             ),
         )
-        weights_offsets = [0] + list(
-            itertools.accumulate([row * dim for (row, dim) in zip(rows, dims)])
-        )
+        # weights_offsets = [0] + list(
+        #    itertools.accumulate([row * dim for (row, dim) in zip(rows, dims)])
+        # )
+        weights_offsets = [0] * (len(rows) + 1)
         self.register_buffer(
             "weights_offsets",
             torch.tensor(
                 weights_offsets[:-1],
                 device=self.current_device,
                 dtype=torch.int64,
             ),
@@ -348,118 +353,198 @@
 
         # add placeholder require_grad param to enable autograd without nn.parameter
         # this is needed to enable int8 embedding weights for SplitTableBatchedEmbedding
         self.placeholder_autograd_tensor = nn.Parameter(
             torch.zeros(0, device=self.current_device, dtype=torch.float)
         )
 
+        # Register backward hook for evicting rows from a scratch pad to SSD
+        # post backward
+        self.placeholder_autograd_tensor.register_hook(self._evict_from_scratch_pad)
+
+        assert optimizer in (
+            OptimType.EXACT_ROWWISE_ADAGRAD,
+        ), f"Optimizer {optimizer} is not supported by SSDTableBatchedEmbeddingBags"
+        self.optimizer = optimizer
+
+    def to_pinned_cpu(self, t: torch.Tensor) -> torch.Tensor:
+        t_cpu = torch.empty(t.shape, pin_memory=True, dtype=t.dtype)
+        t_cpu.copy_(t, non_blocking=True)
+        return t_cpu
+
+    def evict(
+        self, evicted_rows: Tensor, evicted_indices: Tensor, actions_count_cpu: Tensor
+    ) -> None:
+        """
+        Evict data from the given input tensors to SSD via RocksDB
+        """
+        with torch.cuda.stream(self.ssd_stream):
+            self.ssd_stream.wait_event(self.ssd_set_start)
+            evicted_rows_cpu = self.to_pinned_cpu(evicted_rows)
+            evicted_indices_cpu = self.to_pinned_cpu(evicted_indices)
+            evicted_rows.record_stream(self.ssd_stream)
+            evicted_indices.record_stream(self.ssd_stream)
+            self.ssd_db.set_cuda(
+                evicted_indices_cpu, evicted_rows_cpu, actions_count_cpu, self.timestep
+            )
+            # TODO: is this needed?
+            # Need a way to synchronize
+            #  actions_count_cpu.record_stream(self.ssd_stream)
+            self.ssd_stream.record_event(self.ssd_set_end)
+
+    def _evict_from_scratch_pad(self, grad: Tensor) -> None:
+        assert len(self.ssd_scratch_pads) > 0, "There must be at least one scratch pad"
+        (inserted_rows_gpu, post_bwd_evicted_indices, actions_count_cpu) = (
+            self.ssd_scratch_pads.pop(0)
+        )
+        self.evict(inserted_rows_gpu, post_bwd_evicted_indices, actions_count_cpu)
+
+    def _compute_cache_ptrs(
+        self,
+        linear_cache_indices: torch.Tensor,
+        assigned_cache_slots: torch.Tensor,
+        linear_index_inverse_indices: torch.Tensor,
+        unique_indices_count_cumsum: torch.Tensor,
+        cache_set_inverse_indices: torch.Tensor,
+        inserted_rows_gpu: torch.Tensor,
+        unique_indices_length: torch.Tensor,
+        inserted_indices: torch.Tensor,
+        actions_count_cpu: torch.Tensor,
+    ) -> torch.Tensor:
+        lxu_cache_locations = torch.ops.fbgemm.lxu_cache_lookup(
+            linear_cache_indices,
+            self.lxu_cache_state,
+            self.hash_size_cumsum[-1].item(),
+        )
+        lxu_cache_ptrs, post_bwd_evicted_indices = (
+            torch.ops.fbgemm.ssd_generate_row_addrs(
+                lxu_cache_locations,
+                assigned_cache_slots,
+                linear_index_inverse_indices,
+                unique_indices_count_cumsum,
+                cache_set_inverse_indices,
+                self.lxu_cache_weights,
+                inserted_rows_gpu,
+                unique_indices_length,
+                inserted_indices,
+            )
+        )
+        # Store scratch pad info for post backward eviction
+        self.ssd_scratch_pads.append(
+            (inserted_rows_gpu, post_bwd_evicted_indices, actions_count_cpu)
+        )
+        assert lxu_cache_ptrs[lxu_cache_ptrs == 0].numel() == 0
+        return (
+            lxu_cache_ptrs,
+            inserted_rows_gpu,
+            post_bwd_evicted_indices,
+            actions_count_cpu,
+        )
+
     def prefetch(self, indices: Tensor, offsets: Tensor) -> Optional[Tensor]:
         (indices, offsets) = indices.long(), offsets.long()
+
         linear_cache_indices = torch.ops.fbgemm.linearize_cache_indices(
             self.hash_size_cumsum,
             indices,
             offsets,
         )
         self.timestep += 1
         self.timesteps_prefetched.append(self.timestep)
         (
             inserted_indices,
             evicted_indices,
             assigned_cache_slots,
             actions_count_gpu,
-            _,
-            _,
-            _,
-            _,
+            linear_index_inverse_indices,
+            unique_indices_count_cumsum,
+            cache_set_inverse_indices,
+            unique_indices_length,
         ) = torch.ops.fbgemm.ssd_cache_populate_actions(
             linear_cache_indices,
             self.total_hash_size,
             self.lxu_cache_state,
             self.timestep,
             1,  # for now assume prefetch_dist == 1
             self.lru_state,
         )
 
-        def to_pinned_cpu(t: torch.Tensor) -> torch.Tensor:
-            t_cpu = torch.empty(t.shape, pin_memory=True, dtype=t.dtype)
-            t_cpu.copy_(t, non_blocking=True)
-            return t_cpu
-
-        actions_count_cpu = to_pinned_cpu(actions_count_gpu)
+        actions_count_cpu = self.to_pinned_cpu(actions_count_gpu)
         assigned_cache_slots = assigned_cache_slots.long()
         evicted_rows = self.lxu_cache_weights[
-            assigned_cache_slots.clamp_(min=0).long(), :
+            assigned_cache_slots.clamp(min=0).long(), :
         ]
         inserted_rows = torch.empty(
             evicted_rows.shape,
             dtype=self.lxu_cache_weights.dtype,
             pin_memory=True,
         )
 
         current_stream = torch.cuda.current_stream()
 
         # Ensure the previous iterations l3_db.set(..) has completed.
         current_stream.wait_event(self.ssd_set_end)
         self.ssd_db.get_cuda(
-            to_pinned_cpu(inserted_indices), inserted_rows, actions_count_cpu
+            self.to_pinned_cpu(inserted_indices), inserted_rows, actions_count_cpu
         )
         current_stream.record_event(self.ssd_set_start)
         # TODO: T123943415 T123943414 this is a big copy that is (mostly) unnecessary with a decent cache hit rate.
         # Should we allocate on HBM?
         inserted_rows_gpu = inserted_rows.cuda(non_blocking=True)
 
-        # self.lxu_cache_weights[assigned_cache_slots, :] = inserted_rows.cuda(non_blocking=True)
         torch.ops.fbgemm.masked_index_put(
             self.lxu_cache_weights,
             assigned_cache_slots,
             inserted_rows_gpu,
             actions_count_gpu,
         )
 
-        with torch.cuda.stream(self.ssd_stream):
-            self.ssd_stream.wait_event(self.ssd_set_start)
-            evicted_rows_cpu = to_pinned_cpu(evicted_rows)
-            evicted_indices_cpu = to_pinned_cpu(evicted_indices)
-            evicted_rows.record_stream(self.ssd_stream)
-            evicted_indices.record_stream(self.ssd_stream)
-            self.ssd_db.set_cuda(
-                evicted_indices_cpu, evicted_rows_cpu, actions_count_cpu, self.timestep
+        # Evict rows from cache to SSD
+        self.evict(evicted_rows, evicted_indices, actions_count_cpu)
+
+        # TODO: keep only necessary tensors
+        self.ssd_prefetch_data.append(
+            (
+                linear_cache_indices,
+                assigned_cache_slots,
+                linear_index_inverse_indices,
+                unique_indices_count_cumsum,
+                cache_set_inverse_indices,
+                inserted_rows_gpu,
+                unique_indices_length,
+                inserted_indices,
+                actions_count_cpu,
             )
-            # TODO: is this needed?
-            # Need a way to synchronize
-            #  actions_count_cpu.record_stream(self.ssd_stream)
-            self.ssd_stream.record_event(self.ssd_set_end)
-        return linear_cache_indices
+        )
 
     def forward(
         self,
         indices: Tensor,
         offsets: Tensor,
         per_sample_weights: Optional[Tensor] = None,
         feature_requires_grad: Optional[Tensor] = None,
     ) -> Tensor:
         (indices, offsets) = indices.long(), offsets.long()
         # Force casting per_sample_weights to float
         if per_sample_weights is not None:
             per_sample_weights = per_sample_weights.float()
         if len(self.timesteps_prefetched) == 0:
             with record_function("## prefetch ##"):
-                linear_cache_indices = self.prefetch(indices, offsets)
-        else:
-            linear_cache_indices = torch.ops.fbgemm.linearize_cache_indices(
-                self.hash_size_cumsum,
-                indices,
-                offsets,
-            )
-        lxu_cache_locations = torch.ops.fbgemm.lxu_cache_lookup(
-            linear_cache_indices,
-            self.lxu_cache_state,
-            self.hash_size_cumsum[-1].item(),
-        )
-        common_args = invokers.lookup_args.CommonArgs(
+                self.prefetch(indices, offsets)
+        assert len(self.ssd_prefetch_data) > 0
+
+        prefetch_data = self.ssd_prefetch_data.pop(0)
+        (
+            lxu_cache_ptrs,
+            inserted_rows_gpu,
+            post_bwd_evicted_indices,
+            actions_count_cpu,
+        ) = self._compute_cache_ptrs(*prefetch_data)
+
+        common_args = invokers.lookup_args_ssd.CommonArgs(
             placeholder_autograd_tensor=self.placeholder_autograd_tensor,
             output_dtype=SparseType.FP32.as_int(),
             dev_weights=self.weights_dev,
             host_weights=self.weights_host,
             uvm_weights=self.weights_uvm,
             lxu_cache_weights=self.lxu_cache_weights,
             weights_placements=self.weights_placements,
@@ -470,42 +555,58 @@
             hash_size_cumsum=self.hash_size_cumsum,
             total_hash_size_bits=self.total_hash_size_bits,
             indices=indices,
             offsets=offsets,
             pooling_mode=self.pooling_mode,
             indice_weights=per_sample_weights,
             feature_requires_grad=feature_requires_grad,
-            lxu_cache_locations=lxu_cache_locations,
+            lxu_cache_locations=lxu_cache_ptrs,
             uvm_cache_stats=None,
-            vbe_metadata=invokers.lookup_args.VBEMetadata(
+            vbe_metadata=invokers.lookup_args_ssd.VBEMetadata(
                 B_offsets=None,
                 output_offsets_feature_rank=None,
                 B_offsets_rank_per_feature=None,
                 max_B=-1,
                 max_B_feature_rank=-1,
                 output_size=-1,
             ),
             # Unused arguments
             is_experimental=False,
             use_uniq_cache_locations_bwd=False,
             use_homogeneous_placements=True,
+            # The keys for ssd_tensors are controlled by ssd_tensors in
+            # codegen/genscript/optimizer_args.py
+            ssd_tensors={
+                "row_addrs": lxu_cache_ptrs,
+                "inserted_rows": inserted_rows_gpu,
+                "post_bwd_evicted_indices": post_bwd_evicted_indices,
+                "actions_count": actions_count_cpu,
+            },
         )
 
-        momentum1 = invokers.lookup_args.Momentum(
+        self.timesteps_prefetched.pop(0)
+
+        if self.optimizer == OptimType.EXACT_SGD:
+            raise AssertionError(
+                "SSDTableBatchedEmbeddingBags currently does not support SGD"
+            )
+            return invokers.lookup_sgd_ssd.invoke(common_args, self.optimizer_args)
+
+        momentum1 = invokers.lookup_args_ssd.Momentum(
             dev=self.momentum1_dev,
             host=self.momentum1_host,
             uvm=self.momentum1_uvm,
             offsets=self.momentum1_offsets,
             placements=self.momentum1_placements,
         )
 
-        self.timesteps_prefetched.pop(0)
-        return invokers.lookup_rowwise_adagrad.invoke(
-            common_args, self.optimizer_args, momentum1
-        )
+        if self.optimizer == OptimType.EXACT_ROWWISE_ADAGRAD:
+            return invokers.lookup_rowwise_adagrad_ssd.invoke(
+                common_args, self.optimizer_args, momentum1
+            )
 
     @torch.jit.ignore
     def debug_split_optimizer_states(self) -> List[Tuple[torch.Tensor]]:
         """
         Returns a list of states, split by table
         Testing only
         """
@@ -888,15 +989,14 @@
             linear_cache_indices,
             self.total_hash_size,
             self.lxu_cache_state,
             self.timestep_counter.get(),
             1,  # for now assume prefetch_dist == 1
             self.lru_state,
         )
-
         actions_count_cpu = torch.empty(
             actions_count_gpu.shape, pin_memory=True, dtype=actions_count_gpu.dtype
         )
         actions_count_cpu.copy_(actions_count_gpu, non_blocking=True)
         assigned_cache_slots = assigned_cache_slots.long()
         evicted_rows = self.lxu_cache_weights[
             assigned_cache_slots.clamp_(min=0).long(), :
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.5.24"
+__version__: str = "2024.5.25"
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py

```diff
@@ -2,18 +2,28 @@
 
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
+# All optimizers
+import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_args as lookup_args  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_adagrad as lookup_adagrad  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_adam as lookup_adam  # noqa: F401
-import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_args as lookup_args  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_lamb as lookup_lamb  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_lars_sgd as lookup_lars_sgd  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_partial_rowwise_adam as lookup_partial_rowwise_adam  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_partial_rowwise_lamb as lookup_partial_rowwise_lamb  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_rowwise_adagrad as lookup_rowwise_adagrad  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_rowwise_adagrad_with_counter as lookup_rowwise_adagrad_with_counter  # noqa: F401
 import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_sgd as lookup_sgd  # noqa: F401
-import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_none as lookup_none # noqa: F401
+import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_none as lookup_none  # noqa: F401
+
+# SSD optimizers (putting them under try-except for BC as they are
+# experimental ops which can be removed/updated in the future)
+try:
+    import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_args_ssd as lookup_args_ssd
+    import fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_rowwise_adagrad_ssd as lookup_rowwise_adagrad_ssd
+except:
+    import logging
+    logging.warn("fbgemm_gpu.split_embedding_codegen_lookup_invokers.lookup_args_ssd import failed")
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py

```diff
@@ -45,14 +45,15 @@
             # momentum2
             # prev_iter
             # row_counter
             # iter
             # max counter
         )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_adagrad_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py

```diff
@@ -45,14 +45,15 @@
             # momentum2
             # prev_iter
             # row_counter
             # iter
             # max counter
         )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_adagrad_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py

```diff
@@ -24,14 +24,15 @@
         f"""\033[93m
         [FBGEMM_GPU] NOTE: The training optimizer 'adam' is marked as
         EXPERIMENTAL and thus not optimized, in order to reduce code compilation
         times and build sizes!
         \033[0m"""
     )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_adam_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py

```diff
@@ -24,14 +24,15 @@
         f"""\033[93m
         [FBGEMM_GPU] NOTE: The training optimizer 'adam' is marked as
         EXPERIMENTAL and thus not optimized, in order to reduce code compilation
         times and build sizes!
         \033[0m"""
     )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_adam_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 # pyre-strict
 
-from typing import NamedTuple, Optional
+from typing import NamedTuple, Optional, Dict
 
 import torch
 
 
 class VBEMetadata(NamedTuple):
     B_offsets: Optional[torch.Tensor]
     output_offsets_feature_rank: Optional[torch.Tensor]
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py

```diff
@@ -24,14 +24,15 @@
         f"""\033[93m
         [FBGEMM_GPU] NOTE: The training optimizer 'lamb' is marked as
         EXPERIMENTAL and thus not optimized, in order to reduce code compilation
         times and build sizes!
         \033[0m"""
     )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_lamb_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py

```diff
@@ -24,14 +24,15 @@
         f"""\033[93m
         [FBGEMM_GPU] NOTE: The training optimizer 'lamb' is marked as
         EXPERIMENTAL and thus not optimized, in order to reduce code compilation
         times and build sizes!
         \033[0m"""
     )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_lamb_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py

```diff
@@ -22,14 +22,15 @@
         f"""\033[93m
         [FBGEMM_GPU] NOTE: The training optimizer 'lars_sgd' is marked as
         EXPERIMENTAL and thus not optimized, in order to reduce code compilation
         times and build sizes!
         \033[0m"""
     )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_lars_sgd_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py

```diff
@@ -22,14 +22,15 @@
         f"""\033[93m
         [FBGEMM_GPU] NOTE: The training optimizer 'lars_sgd' is marked as
         EXPERIMENTAL and thus not optimized, in order to reduce code compilation
         times and build sizes!
         \033[0m"""
     )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_lars_sgd_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py

```diff
@@ -13,14 +13,15 @@
 
 def invoke(
     common_args: CommonArgs,
     optimizer_args: OptimizerArgs,
     total_unique_indices: int,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_none_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py

```diff
@@ -13,14 +13,15 @@
 
 def invoke(
     common_args: CommonArgs,
     optimizer_args: OptimizerArgs,
     total_unique_indices: int,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_none_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py

```diff
@@ -15,14 +15,15 @@
     common_args: CommonArgs,
     optimizer_args: OptimizerArgs,
     momentum1: Momentum,
     momentum2: Momentum,
     iter: int,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_partial_rowwise_adam_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py

```diff
@@ -15,14 +15,15 @@
     common_args: CommonArgs,
     optimizer_args: OptimizerArgs,
     momentum1: Momentum,
     momentum2: Momentum,
     iter: int,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_partial_rowwise_adam_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py

```diff
@@ -15,14 +15,15 @@
     common_args: CommonArgs,
     optimizer_args: OptimizerArgs,
     momentum1: Momentum,
     momentum2: Momentum,
     iter: int,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_partial_rowwise_lamb_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py

```diff
@@ -15,14 +15,15 @@
     common_args: CommonArgs,
     optimizer_args: OptimizerArgs,
     momentum1: Momentum,
     momentum2: Momentum,
     iter: int,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_partial_rowwise_lamb_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py

```diff
@@ -48,14 +48,15 @@
             # momentum2
             # prev_iter
             # row_counter
             # iter
             # max counter
         )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_rowwise_adagrad_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py

```diff
@@ -48,14 +48,15 @@
             # momentum2
             # prev_iter
             # row_counter
             # iter
             # max counter
         )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_rowwise_adagrad_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py

```diff
@@ -17,14 +17,15 @@
     momentum1: Momentum,
     prev_iter: Momentum,
     row_counter: Momentum,
     iter: int,
     max_counter: float,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py

```diff
@@ -17,14 +17,15 @@
     momentum1: Momentum,
     prev_iter: Momentum,
     row_counter: Momentum,
     iter: int,
     max_counter: float,
 ) -> torch.Tensor:
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py

```diff
@@ -40,14 +40,15 @@
             # momentum2
             # prev_iter
             # row_counter
             # iter
             # max counter
         )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_sgd_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py

```diff
@@ -40,14 +40,15 @@
             # momentum2
             # prev_iter
             # row_counter
             # iter
             # max counter
         )
     vbe_metadata = common_args.vbe_metadata
+
     return torch.ops.fbgemm.split_embedding_codegen_lookup_sgd_function(
         # common_args
         placeholder_autograd_tensor=common_args.placeholder_autograd_tensor,
         dev_weights=common_args.dev_weights,
         uvm_weights=common_args.uvm_weights,
         lxu_cache_weights=common_args.lxu_cache_weights,
         weights_placements=common_args.weights_placements,
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm_gpu_nightly-cpu
-Version: 2024.5.24
+Version: 2024.5.25
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 fbgemm_gpu/__init__.py,sha256=plInYJM4Eqp01xDgYvEdYAYLy9btsh6_mTqqmXysarc,1342
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=dpxZAueNsadJVuK7Dwo8GbOlho9r67Lfh8kesqRKJNI,3079
 fbgemm_gpu/enums.py,sha256=GVuzF5cFTLzttkvlH1SdcGrxrppMhDSbQj_Vm_4zmEo,789
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=SDCoos4pVP0q38KNAKfIwzp4MZkc5bGsLCEu3BO_xkw,10953208
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=Qv0UQsTIvmFZIkan8Ea--651gEBSI1BJcWJDNMYyYbI,10953208
 fbgemm_gpu/metrics.py,sha256=TsurFLJf0nJvPDN7urWb4LMQlf5RgdWPTTTDO7S4wtI,5663
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=4mHJ2fo3SeG25iSwdm2YsM8q_oWsF1LxRguYmxSnuDI,2362
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=cUrEbRIvLFW_3Zmh07QkN4S1Cfvvge6TYO1VXBFCpz8,2752
 fbgemm_gpu/quantize_comm.py,sha256=UZcVSC2JQ0oSkwsJQnjaZ2k8mm2p3hvVzpyg7X5xFXM,7885
 fbgemm_gpu/quantize_utils.py,sha256=TmlA7g74cxhP0TEbrNOgpR2TOYmfMc_LiDMVCYa-Sw4,4020
 fbgemm_gpu/runtime_monitor.py,sha256=tIdxkJIWkJ8705btxs9NqzEXC7QprFh3sA8Q4LpvtJ8,6947
-fbgemm_gpu/sparse_ops.py,sha256=WL1l9d7qUTjF4S57o6ZNUswH4gIWzbW41_mHNzodAp8,31526
+fbgemm_gpu/sparse_ops.py,sha256=oTjzi-j49nH_RmNRulju0kFpBmAI55EY8vrqTgkO5jE,32627
 fbgemm_gpu/split_embedding_configs.py,sha256=PIdR7c_Y-G1A4WuWP6qzv6uMzx4J9CNo_IrZI_JFZ9w,5859
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=W61ps3tyNQYv__V3vNnAjEK9Q_LKNUqDB2cLtDNvEyE,7058
 fbgemm_gpu/split_embedding_optimizer_ops.py,sha256=qIf00N56cFF5AX0zSoB8k1v60HnDBoq8JniSDFhdPC0,540
 fbgemm_gpu/split_embedding_utils.py,sha256=BVq7Jo4hLN7TVp8h0soxz3xouv6NBzPvaFn-Xn3IYRc,26853
 fbgemm_gpu/split_table_batched_embeddings_ops.py,sha256=_MIp6uHYHLn4GxGdrGsfddfSsZ2Z9mjsYIrih3ncI1I,2339
 fbgemm_gpu/split_table_batched_embeddings_ops_common.py,sha256=--NWgslR2aip-8yIIyt8dytlmvuxRujgQ0z86xqzVjo,4035
 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py,sha256=py6bt2FS3Kl5_pi_KfEIdJoRP-F5E8Og5iiZutOS1m4,67230
 fbgemm_gpu/split_table_batched_embeddings_ops_training.py,sha256=dQC2q5CnyDoQPCBEmBtjdFi5UVhI-UIUXWOhX_fC5jw,101933
-fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=hh8LlWzODuHHW6lp8cyjIBFlMH8v6wzaBQnU162dM24,40873
+fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=A7GLMdnH19AxCK9bgPNcHhNYvtRQ9ty6EI7bL40pUs0,44844
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=Rh8Kn4L7LJRqCFWILZD7wReoBy8ZD2R_TfEzWHVCoA0,419
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=H8HFCicLB9gaH0OogGbtsmVlRAA69bJnevdZCt2Dd74,264
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=lfob_IDNeAs2FjS2WCldKlw0gm_qUZdp043fngI8sGE,1466
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=ibfUa6H9BY85_e9VgbKujKi4nuR7Mgyw77VbFMkLKCs,2147
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py,sha256=xhDnYR0vVDSK96nbcNSs5NbGXqFF3FGIs3DPDBJYt08,3395
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py,sha256=xhDnYR0vVDSK96nbcNSs5NbGXqFF3FGIs3DPDBJYt08,3395
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py,sha256=izbpTM7obzQZ0FmCW22GvHvro337yMK1B0BhipykJik,3144
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py,sha256=izbpTM7obzQZ0FmCW22GvHvro337yMK1B0BhipykJik,3144
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py,sha256=hafQfCDpsPd_pxs6a8V2-QJ_Tzu8YMJgaCjsVfpeFYQ,2420
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py,sha256=hafQfCDpsPd_pxs6a8V2-QJ_Tzu8YMJgaCjsVfpeFYQ,2420
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=8fvC-BAOBlXlr_M35HQ25g5lkOFpCIm1X8lfS1xz59c,3100
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py,sha256=8fvC-BAOBlXlr_M35HQ25g5lkOFpCIm1X8lfS1xz59c,3100
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=6OceYmQDKDTRBi-w4UIrYvcErWovxzim23ws0o9JKMY,3100
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py,sha256=6OceYmQDKDTRBi-w4UIrYvcErWovxzim23ws0o9JKMY,3100
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=Aljkdf4GB0zetL2j5YIhTZaOqiIMIlQ9iTDM421lbiM,4512
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=Aljkdf4GB0zetL2j5YIhTZaOqiIMIlQ9iTDM421lbiM,4512
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
-fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
+fbgemm_gpu/docs/version.py,sha256=IBbTS8AeqPe24QGr72F36nxWZzH7IYml5ej-Pwrd6DU,264
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=zjUGbYZIC0yGtsNCPoCbTZ0-_Nj0Pd_yqHiRWTKeuT8,1964
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=eHXy3WvsqeDDAAG2IKQKW-TYKtkO7rwqqaa-ypPK19w,4181
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=eHXy3WvsqeDDAAG2IKQKW-TYKtkO7rwqqaa-ypPK19w,4181
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=npe6C60ZLb3oWCni9OCfNYty22Lrw4br_7x8hG4IEcw,3396
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=npe6C60ZLb3oWCni9OCfNYty22Lrw4br_7x8hG4IEcw,3396
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=iaVc4tedyUEfN-TDKYu2jgcUEgHcCA5O9gw2H4uNBBA,2153
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args_ssd.py,sha256=VVJhaeY78p2LYRWejF_CI17VWJ58vbNJBAPIrlrITdU,2194
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py,sha256=JMk5n_HYDop89SZmbKXgVYb9a_yDzvpQBPjyFKmoceM,3396
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py,sha256=JMk5n_HYDop89SZmbKXgVYb9a_yDzvpQBPjyFKmoceM,3396
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py,sha256=TNLgaV5nCNdyVQEJfAaq0FlvafRmTjR9k0o14shx2ek,3145
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py,sha256=TNLgaV5nCNdyVQEJfAaq0FlvafRmTjR9k0o14shx2ek,3145
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py,sha256=BXGQoQ-A1k0TGduxew8niAn_-1UGyGJJbTwLsX_sb4g,2421
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py,sha256=BXGQoQ-A1k0TGduxew8niAn_-1UGyGJJbTwLsX_sb4g,2421
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=drqumva1Vcz_7e_5FRAOX9ms3MUt2epjQA-21uCUHnU,3101
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py,sha256=drqumva1Vcz_7e_5FRAOX9ms3MUt2epjQA-21uCUHnU,3101
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=A-1Jtv_MFF5JOgT3fbA0LRyicbFz-urL046yJTQUPzI,3101
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py,sha256=A-1Jtv_MFF5JOgT3fbA0LRyicbFz-urL046yJTQUPzI,3101
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=GxmRzYhOqcepsIKt3cI4opD57i6wB-l5ZR6bbu0obok,4513
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=GxmRzYhOqcepsIKt3cI4opD57i6wB-l5ZR6bbu0obok,4513
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_ssd.py,sha256=05q-71clT4s8fIfxJzX-_jgPMhpebGTtwA96IXco3Yc,3902
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=A5IrCcJjdf3ZxZ_3VbbMsd0xqs4qFjlu4F9HQkkIOLA,3965
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=A5IrCcJjdf3ZxZ_3VbbMsd0xqs4qFjlu4F9HQkkIOLA,3965
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=kmd4ezZHdWF7TWI4V_SUUv04prmu_Hq_CvzslCIEawc,3763
+fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=kmd4ezZHdWF7TWI4V_SUUv04prmu_Hq_CvzslCIEawc,3763
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
 fbgemm_gpu/tbe/__init__.py,sha256=fE0IHi1JJpxsNVBNzWNee2thrNXFFRhY94c80RxNSIE,231
 fbgemm_gpu/tbe/cache/__init__.py,sha256=kueJp-xYnDflz4DYf7dh5_xtx5ItzrbQc_1neoe5XQc,308
 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py,sha256=F2XIec8Kgcihy1vXJRp0tQErqIQSQIDZRuzLfkasE70,1660
-fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/METADATA,sha256=_eqymJkoMVbaMEjecLVUxz-DhyEZ39uI28njQhrBjqk,2602
-fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.5.24.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/METADATA,sha256=gw_afd5G-la3_CacfLAFWtjM1PzB0U5zHXthF6ssWm0,2602
+fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/WHEEL,sha256=OEmkRrFcnutAqrz0YyBUaC3hh1288y58dKLCWma58N0,105
+fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.5.25.dist-info/RECORD,,
```

