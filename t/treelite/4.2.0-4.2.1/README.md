# Comparing `tmp/treelite-4.2.0.tar.gz` & `tmp/treelite-4.2.1.tar.gz`

## Comparing `treelite-4.2.0.tar` & `treelite-4.2.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/LICENSE
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Doxygen.cmake
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/ExternalLibs.cmake
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Sanitizer.cmake
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Utils.cmake
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/Version.cmake
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/cmake/version.h.in
--rw-r--r--   0        0        0    42322 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/c_api.h
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/c_api_error.h
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/contiguous_array.h
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/error.h
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/gtil.h
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/logging.h
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/model_builder.h
--rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/model_loader.h
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/pybuffer_frame.h
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/thread_local.h
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/tree.h
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/contiguous_array.h
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/file_utils.h
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/omp_exception.h
--rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/serializer.h
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/serializer_mixins.h
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/threading_utils.h
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/detail/tree.h
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/operator.h
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/task_type.h
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/tree_node_type.h
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/include/treelite/enum/typeinfo.h
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/CMakeLists.txt
--rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/field_accessor.cc
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/json_serializer.cc
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/logging.cc
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_concat.cc
--rw-r--r--   0        0        0    19505 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/serializer.cc
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/c_api_error.cc
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/c_api_utils.h
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/field_accessor.cc
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/gtil.cc
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/logging.cc
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/model.cc
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/model_builder.cc
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/model_loader.cc
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/serializer.cc
--rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/c_api/sklearn.cc
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/operator.cc
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/task_type.cc
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/tree_node_type.cc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/enum/typeinfo.cc
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/config.cc
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/output_shape.cc
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/postprocessor.cc
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/postprocessor.h
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/gtil/predict.cc
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_builder/metadata.cc
--rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_builder/model_builder.cc
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_builder/detail/json_parsing.h
--rw-r--r--   0        0        0    22109 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/lightgbm.cc
--rw-r--r--   0        0        0    26078 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/sklearn.cc
--rw-r--r--   0        0        0    31217 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/xgboost_json.cc
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/xgboost_legacy.cc
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/lightgbm.h
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/string_utils.h
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.cc
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.h
--rw-r--r--   0        0        0    19413 2020-02-02 00:00:00.000000 treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost_json.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/build_config.py
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/nativelib.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/pep517.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/sdist.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 treelite-4.2.0/packager/util.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/VERSION
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/__init__.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/compat.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/core.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/frontend.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/libpath.py
--rw-r--r--   0        0        0    19254 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/model.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/model_builder.py
--rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/model_builder_legacy.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/path_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/py.typed
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/util.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/gtil/__init__.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/gtil/gtil.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/sklearn/__init__.py
--rw-r--r--   0        0        0    19233 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/sklearn/importer.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 treelite-4.2.0/treelite/sklearn/isolation_forest.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 treelite-4.2.0/README.rst
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 treelite-4.2.0/hatch_build.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 treelite-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 treelite-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/LICENSE
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/Doxygen.cmake
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/ExternalLibs.cmake
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/Sanitizer.cmake
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/Utils.cmake
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/Version.cmake
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/cmake/version.h.in
+-rw-r--r--   0        0        0    42322 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/c_api.h
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/c_api_error.h
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/contiguous_array.h
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/error.h
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/gtil.h
+-rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/logging.h
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/model_builder.h
+-rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/model_loader.h
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/pybuffer_frame.h
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/thread_local.h
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/tree.h
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/contiguous_array.h
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/file_utils.h
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/omp_exception.h
+-rw-r--r--   0        0        0     7948 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/serializer.h
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/serializer_mixins.h
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/threading_utils.h
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/detail/tree.h
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/enum/operator.h
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/enum/task_type.h
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/enum/tree_node_type.h
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/include/treelite/enum/typeinfo.h
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/CMakeLists.txt
+-rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/field_accessor.cc
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/json_serializer.cc
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/logging.cc
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_concat.cc
+-rw-r--r--   0        0        0    19505 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/serializer.cc
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/c_api_error.cc
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/c_api_utils.h
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/field_accessor.cc
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/gtil.cc
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/logging.cc
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/model.cc
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/model_builder.cc
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/model_loader.cc
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/serializer.cc
+-rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/c_api/sklearn.cc
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/enum/operator.cc
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/enum/task_type.cc
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/enum/tree_node_type.cc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/enum/typeinfo.cc
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/gtil/config.cc
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/gtil/output_shape.cc
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/gtil/postprocessor.cc
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/gtil/postprocessor.h
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/gtil/predict.cc
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_builder/metadata.cc
+-rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_builder/model_builder.cc
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_builder/detail/json_parsing.h
+-rw-r--r--   0        0        0    22109 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/lightgbm.cc
+-rw-r--r--   0        0        0    26078 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/sklearn.cc
+-rw-r--r--   0        0        0    31217 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/xgboost_json.cc
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/xgboost_legacy.cc
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/detail/lightgbm.h
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/detail/string_utils.h
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/detail/xgboost.cc
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/detail/xgboost.h
+-rw-r--r--   0        0        0    19413 2020-02-02 00:00:00.000000 treelite-4.2.1/cpp_src/src/model_loader/detail/xgboost_json.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.2.1/packager/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 treelite-4.2.1/packager/build_config.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 treelite-4.2.1/packager/nativelib.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 treelite-4.2.1/packager/pep517.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 treelite-4.2.1/packager/sdist.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 treelite-4.2.1/packager/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/VERSION
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/__init__.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/compat.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/core.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/frontend.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/libpath.py
+-rw-r--r--   0        0        0    19254 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/model.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/model_builder.py
+-rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/model_builder_legacy.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/path_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/py.typed
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/util.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/gtil/__init__.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/gtil/gtil.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/sklearn/__init__.py
+-rw-r--r--   0        0        0    19233 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/sklearn/importer.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 treelite-4.2.1/treelite/sklearn/isolation_forest.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 treelite-4.2.1/README.rst
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 treelite-4.2.1/hatch_build.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 treelite-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 treelite-4.2.1/PKG-INFO
```

### Comparing `treelite-4.2.0/cpp_src/CMakeLists.txt` & `treelite-4.2.1/cpp_src/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_policy(SET CMP0025 NEW)
 cmake_policy(SET CMP0091 NEW)
 set(CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
 cmake_minimum_required(VERSION 3.16 FATAL_ERROR)
 
-project(treelite LANGUAGES CXX C VERSION 4.2.0)
+project(treelite LANGUAGES CXX C VERSION 4.2.1)
 
 # Check compiler versions
 # Use latest compilers to ensure that std::filesystem is available
 if(MSVC)
   if(MSVC_VERSION LESS 1930)
     message(FATAL_ERROR "Need Visual Studio 2022 or newer to build Treelite")
   endif()
```

### Comparing `treelite-4.2.0/cpp_src/LICENSE` & `treelite-4.2.1/cpp_src/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/cmake/ExternalLibs.cmake` & `treelite-4.2.1/cpp_src/cmake/ExternalLibs.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 include(FetchContent)
 
 # RapidJSON (header-only library)
 add_library(rapidjson INTERFACE)
 target_compile_definitions(rapidjson INTERFACE -DRAPIDJSON_HAS_STDSTRING=1)
 find_package(RapidJSON)
 if(RapidJSON_FOUND)
-  target_include_directories(rapidjson INTERFACE ${RAPIDJSON_INCLUDE_DIRS})
+  if(DEFINED RAPIDJSON_INCLUDE_DIRS)
+    # Compatibility with 1.1.0 stable (circa 2016)
+    set(RapidJSON_include_dir "${RAPIDJSON_INCLUDE_DIRS}")
+  else()
+    # Latest RapidJSON (1.1.0.post*)
+    set(RapidJSON_include_dir "${RapidJSON_INCLUDE_DIRS}")
+  endif()
+  target_include_directories(rapidjson INTERFACE ${RapidJSON_include_dir})
+  message(STATUS "Found RapidJSON: ${RapidJSON_include_dir}")
 else()
   message(STATUS "Did not find RapidJSON in the system root. Fetching RapidJSON now...")
   FetchContent_Declare(
     RapidJSON
     GIT_REPOSITORY      https://github.com/Tencent/rapidjson
-    GIT_TAG             v1.1.0
+    GIT_TAG             ab1842a2dae061284c0a62dca1cc6d5e7e37e346
   )
   FetchContent_Populate(RapidJSON)
   message(STATUS "RapidJSON was downloaded at ${rapidjson_SOURCE_DIR}.")
   target_include_directories(rapidjson INTERFACE $<BUILD_INTERFACE:${rapidjson_SOURCE_DIR}/include>)
 endif()
 add_library(RapidJSON::rapidjson ALIAS rapidjson)
```

### Comparing `treelite-4.2.0/cpp_src/cmake/Sanitizer.cmake` & `treelite-4.2.1/cpp_src/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/cmake/Utils.cmake` & `treelite-4.2.1/cpp_src/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/c_api.h` & `treelite-4.2.1/cpp_src/include/treelite/c_api.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/c_api_error.h` & `treelite-4.2.1/cpp_src/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/contiguous_array.h` & `treelite-4.2.1/cpp_src/include/treelite/contiguous_array.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/gtil.h` & `treelite-4.2.1/cpp_src/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/logging.h` & `treelite-4.2.1/cpp_src/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/model_builder.h` & `treelite-4.2.1/cpp_src/include/treelite/model_builder.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/model_loader.h` & `treelite-4.2.1/cpp_src/include/treelite/model_loader.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/pybuffer_frame.h` & `treelite-4.2.1/cpp_src/include/treelite/pybuffer_frame.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/thread_local.h` & `treelite-4.2.1/cpp_src/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/tree.h` & `treelite-4.2.1/cpp_src/include/treelite/tree.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/contiguous_array.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/contiguous_array.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/file_utils.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/file_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/omp_exception.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/serializer.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/serializer.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/serializer_mixins.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/serializer_mixins.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/threading_utils.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/threading_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/detail/tree.h` & `treelite-4.2.1/cpp_src/include/treelite/detail/tree.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/enum/operator.h` & `treelite-4.2.1/cpp_src/include/treelite/enum/operator.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/enum/task_type.h` & `treelite-4.2.1/cpp_src/include/treelite/enum/task_type.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/enum/tree_node_type.h` & `treelite-4.2.1/cpp_src/include/treelite/enum/tree_node_type.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/include/treelite/enum/typeinfo.h` & `treelite-4.2.1/cpp_src/include/treelite/enum/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/CMakeLists.txt` & `treelite-4.2.1/cpp_src/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/field_accessor.cc` & `treelite-4.2.1/cpp_src/src/field_accessor.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/json_serializer.cc` & `treelite-4.2.1/cpp_src/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/logging.cc` & `treelite-4.2.1/cpp_src/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_concat.cc` & `treelite-4.2.1/cpp_src/src/model_concat.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/serializer.cc` & `treelite-4.2.1/cpp_src/src/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/c_api_error.cc` & `treelite-4.2.1/cpp_src/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/c_api_utils.h` & `treelite-4.2.1/cpp_src/src/c_api/c_api_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/field_accessor.cc` & `treelite-4.2.1/cpp_src/src/c_api/field_accessor.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/gtil.cc` & `treelite-4.2.1/cpp_src/src/c_api/gtil.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/logging.cc` & `treelite-4.2.1/cpp_src/src/c_api/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/model.cc` & `treelite-4.2.1/cpp_src/src/c_api/model.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/model_builder.cc` & `treelite-4.2.1/cpp_src/src/c_api/model_builder.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/model_loader.cc` & `treelite-4.2.1/cpp_src/src/c_api/model_loader.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/serializer.cc` & `treelite-4.2.1/cpp_src/src/c_api/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/c_api/sklearn.cc` & `treelite-4.2.1/cpp_src/src/c_api/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/enum/operator.cc` & `treelite-4.2.1/cpp_src/src/enum/operator.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/enum/task_type.cc` & `treelite-4.2.1/cpp_src/src/enum/task_type.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/enum/tree_node_type.cc` & `treelite-4.2.1/cpp_src/src/enum/tree_node_type.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/enum/typeinfo.cc` & `treelite-4.2.1/cpp_src/src/enum/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/gtil/config.cc` & `treelite-4.2.1/cpp_src/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/gtil/output_shape.cc` & `treelite-4.2.1/cpp_src/src/gtil/output_shape.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/gtil/postprocessor.cc` & `treelite-4.2.1/cpp_src/src/gtil/postprocessor.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/gtil/postprocessor.h` & `treelite-4.2.1/cpp_src/src/gtil/postprocessor.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/gtil/predict.cc` & `treelite-4.2.1/cpp_src/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_builder/metadata.cc` & `treelite-4.2.1/cpp_src/src/model_builder/metadata.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_builder/model_builder.cc` & `treelite-4.2.1/cpp_src/src/model_builder/model_builder.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_builder/detail/json_parsing.h` & `treelite-4.2.1/cpp_src/src/model_builder/detail/json_parsing.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/lightgbm.cc` & `treelite-4.2.1/cpp_src/src/model_loader/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/sklearn.cc` & `treelite-4.2.1/cpp_src/src/model_loader/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/xgboost_json.cc` & `treelite-4.2.1/cpp_src/src/model_loader/xgboost_json.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/xgboost_legacy.cc` & `treelite-4.2.1/cpp_src/src/model_loader/xgboost_legacy.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/detail/lightgbm.h` & `treelite-4.2.1/cpp_src/src/model_loader/detail/lightgbm.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/detail/string_utils.h` & `treelite-4.2.1/cpp_src/src/model_loader/detail/string_utils.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.cc` & `treelite-4.2.1/cpp_src/src/model_loader/detail/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost.h` & `treelite-4.2.1/cpp_src/src/model_loader/detail/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/cpp_src/src/model_loader/detail/xgboost_json.h` & `treelite-4.2.1/cpp_src/src/model_loader/detail/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/packager/build_config.py` & `treelite-4.2.1/packager/build_config.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/packager/nativelib.py` & `treelite-4.2.1/packager/nativelib.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/packager/pep517.py` & `treelite-4.2.1/packager/pep517.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/packager/sdist.py` & `treelite-4.2.1/packager/sdist.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/packager/util.py` & `treelite-4.2.1/packager/util.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/compat.py` & `treelite-4.2.1/treelite/compat.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/core.py` & `treelite-4.2.1/treelite/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         # Building docs
         return None  # type: ignore
     if sys.version_info >= (3, 8) and sys.platform == "win32":
         # pylint: disable=no-member
         os.add_dll_directory(
             os.path.join(os.path.normpath(sys.base_prefix), "Library", "bin")
         )
-    lib = ctypes.CDLL(lib_path[0], mode=ctypes.RTLD_GLOBAL)
+    lib = ctypes.cdll.LoadLibrary(lib_path[0])
     lib.TreeliteGetLastError.restype = ctypes.c_char_p
     lib.log_callback = _log_callback
     lib.warn_callback = _warn_callback
     if lib.TreeliteRegisterLogCallback(lib.log_callback) != 0:
         raise TreeliteError(py_str(lib.TreeliteGetLastError()))
     if lib.TreeliteRegisterWarningCallback(lib.warn_callback) != 0:
         raise TreeliteError(py_str(lib.TreeliteGetLastError()))
```

### Comparing `treelite-4.2.0/treelite/frontend.py` & `treelite-4.2.1/treelite/frontend.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/libpath.py` & `treelite-4.2.1/treelite/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/model.py` & `treelite-4.2.1/treelite/model.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/model_builder.py` & `treelite-4.2.1/treelite/model_builder.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/model_builder_legacy.py` & `treelite-4.2.1/treelite/model_builder_legacy.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/util.py` & `treelite-4.2.1/treelite/util.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/gtil/gtil.py` & `treelite-4.2.1/treelite/gtil/gtil.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/sklearn/__init__.py` & `treelite-4.2.1/treelite/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/sklearn/importer.py` & `treelite-4.2.1/treelite/sklearn/importer.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/treelite/sklearn/isolation_forest.py` & `treelite-4.2.1/treelite/sklearn/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/hatch_build.py` & `treelite-4.2.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `treelite-4.2.0/pyproject.toml` & `treelite-4.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.12.1"
 ]
 backend-path = ["."]
 build-backend = "packager.pep517"
 
 [project]
 name = "treelite"
-version = "4.2.0"
+version = "4.2.1"
 authors = [
     {name = "Hyunsu Cho", email = "chohyu01@cs.washington.edu"}
 ]
 description = "Treelite: Universal model exchange format for decision tree forests"
 readme = {file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.8"
 license = {text = "Apache-2.0"}
```

### Comparing `treelite-4.2.0/PKG-INFO` & `treelite-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: treelite
-Version: 4.2.0
+Version: 4.2.1
 Summary: Treelite: Universal model exchange format for decision tree forests
 Project-URL: documentation, https://treelite.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/dmlc/treelite
 Author-email: Hyunsu Cho <chohyu01@cs.washington.edu>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

