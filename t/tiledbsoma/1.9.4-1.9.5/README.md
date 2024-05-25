# Comparing `tmp/tiledbsoma-1.9.4.tar.gz` & `tmp/tiledbsoma-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.9.4.tar", last modified: Fri Apr  5 16:18:15 2024, max compression
+gzip compressed data, was "tiledbsoma-1.9.5.tar", last modified: Thu Apr 11 13:37:08 2024, max compression
```

## Comparing `tiledbsoma-1.9.4.tar` & `tiledbsoma-1.9.5.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.831182 tiledbsoma-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 16:18:11.000000 tiledbsoma-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-05 16:18:15.831182 tiledbsoma-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-05 16:18:11.000000 tiledbsoma-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 16:18:13.000000 tiledbsoma-1.9.4/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-05 16:18:11.000000 tiledbsoma-1.9.4/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.819182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.819182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/khash/
--rw-r--r--   0 runner    (1001) docker     (127)    32575 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/khash/khash.h
--rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/khash/khashl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.819182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.819182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/reindexer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/reindexer.h
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.819182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/array_buffers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/enums.h
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (127)    19394 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_collection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_collection.h
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_context.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_context.h
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_experiment.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_experiment.h
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_group.h
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_measurement.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_measurement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_object.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_object.h
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.819182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.823182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (127)   114830 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/nanoarrow.c
--rw-r--r--   0 runner    (1001) docker     (127)   143114 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/nanoarrow.h
--rw-r--r--   0 runner    (1001) docker     (127)    16393 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/nanoarrow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.823182 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/test_indexer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_collection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.823182 tiledbsoma-1.9.4/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     3300 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/scripts/bld
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/scripts/bld.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1403 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:18:15.831182 tiledbsoma-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.815182 tiledbsoma-1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.827182 tiledbsoma-1.9.4/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28479 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    37351 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/common.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.827182 tiledbsoma-1.9.4/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.831182 tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/ambient_label_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/id_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)   101507 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/io/outgest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.831182 tiledbsoma-1.9.4/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/query_condition.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/reindexer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28814 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_collection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_context.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_dataframe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_dense_ndarray.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_object.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/src/tiledbsoma/soma_sparse_ndarray.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:18:15.827182 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-05 16:18:15.000000 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-05 16:18:15.000000 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:18:15.000000 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:18:15.000000 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 16:18:15.000000 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 16:18:15.000000 tiledbsoma-1.9.4/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-05 16:18:12.000000 tiledbsoma-1.9.4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17772 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/khash/
+-rw-r--r--   0 runner    (1001) docker     (127)    32575 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/khash/khash.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/khash/khashl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.966575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/reindexer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/reindexer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.970575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/array_buffers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/enums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19394 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_collection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_context.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_context.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dataframe.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_experiment.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_experiment.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_group.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_measurement.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_measurement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_object.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_object.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.970575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.970575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    22059 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (127)   114830 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/nanoarrow.c
+-rw-r--r--   0 runner    (1001) docker     (127)   143114 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/nanoarrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16393 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/nanoarrow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.970575 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/test_indexer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.974575 tiledbsoma-1.9.5/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3300 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/scripts/bld
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/scripts/bld.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1403 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.962575 tiledbsoma-1.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28479 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37351 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/common.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/ambient_label_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/id_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101507 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/io/outgest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/query_condition.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/reindexer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28814 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_collection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_context.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_dataframe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_dense_ndarray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_object.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-11 13:37:06.000000 tiledbsoma-1.9.5/src/tiledbsoma/soma_sparse_ndarray.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:08.978575 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-11 13:37:08.000000 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-11 13:37:08.000000 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:37:08.000000 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:37:08.000000 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-11 13:37:08.000000 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 13:37:08.000000 tiledbsoma-1.9.5/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-11 13:37:07.000000 tiledbsoma-1.9.5/version.py
```

### Comparing `tiledbsoma-1.9.4/PKG-INFO` & `tiledbsoma-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.9.4
+Version: 1.9.5
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.9.4/README.md` & `tiledbsoma-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/khash/khash.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/khash/khash.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/khash/khashl.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/khash/khashl.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/example.py` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/example.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/reindexer.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/reindexer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/reindexer.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/reindexer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/reindexer/test_indexer_data_types_perf.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/array_buffers.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/array_buffers.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/array_buffers.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/array_buffers.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/column_buffer.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/column_buffer.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/column_buffer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/enums.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/enums.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/logger_public.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_collection.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_collection.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_collection.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_collection.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_context.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_context.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_context.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_context.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dataframe.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dataframe.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dataframe.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_dense_ndarray.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_experiment.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_experiment.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_experiment.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_experiment.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_group.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_group.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_group.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_measurement.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_measurement.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_measurement.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_measurement.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_object.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_object.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_object.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_object.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/soma/soma_sparse_ndarray.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.cc`

 * *Files 2% similar despite different names*

```diff
@@ -294,22 +294,14 @@
         default:
             throw TileDBSOMAError(fmt::format(
                 "ArrowAdapter: Unsupported TileDB dict datatype: {} ",
                 tiledb::impl::type_to_str(enmr.type())));
     }
 }
 
-bool ArrowAdapter::_isstr(const char* format) {
-    if ((strcmp(format, "U") == 0) || (strcmp(format, "Z") == 0) ||
-        (strcmp(format, "u") == 0) || (strcmp(format, "z") == 0)) {
-        return true;
-    }
-    return false;
-}
-
 inline void exitIfError(const ArrowErrorCode ec, const std::string& msg) {
     if (ec != NANOARROW_OK)
         throw TileDBSOMAError(
             fmt::format("ArrowAdapter: Arrow Error {} ", msg));
 }
 
 std::pair<std::unique_ptr<ArrowArray>, std::unique_ptr<ArrowSchema>>
@@ -354,14 +346,17 @@
         n_buffers,
         array->n_buffers,
         column->is_nullable()));
 
     // After allocating and initializing via nanoarrow we
     // hook our custom release function in
     array->release = &release_array;
+    if (array->private_data != nullptr) {  // as we use nanoarrow's init
+        free(array->private_data);         // free what was allocated before
+    }                                      // assigning our ArrowBuffer pointer
     array->private_data = (void*)arrow_buffer;
 
     LOG_TRACE(fmt::format(
         "[ArrowAdapter] create array name='{}' use_count={}",
         column->name(),
         column.use_count()));
 
@@ -441,18 +436,15 @@
         dict_sch->release = &release_schema;
 
         exitIfError(
             ArrowArrayInitFromType(dict_arr, dnatype), "Bad array init");
         exitIfError(
             ArrowArrayAllocateChildren(dict_arr, 0),
             "Bad array children alloc");
-        const int n_buf = ArrowAdapter::_isstr(dict_sch->format) == true ? 3 :
-                                                                           2;
-        dict_arr->buffers = (const void**)malloc(sizeof(void*) * n_buf);
-        dict_arr->buffers[0] = nullptr;  // validity: none here
+        // hook up our custom release function
         dict_arr->release = &release_array;
 
         // TODO string types currently get the data and offset
         // buffers from ColumnBuffer::enum_offsets and
         // ColumnBuffer::enum_string which is retrieved via
         // ColumnBuffer::convert_enumeration. This may be refactored
         // to all use ColumnBuffer::get_enumeration_info. Note that
```

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/nanoarrow.c` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/nanoarrow.c`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/nanoarrow.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/nanoarrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/nanoarrow.hpp` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/nanoarrow.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/src/utils/version.h` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/test_indexer.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/test_indexer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_collection.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_collection.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_dataframe.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_dense_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_group.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_soma_sparse_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.9.5/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/scripts/bld` & `tiledbsoma-1.9.5/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/scripts/bld.ps1` & `tiledbsoma-1.9.5/dist_links/scripts/bld.ps1`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.9.5/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/scripts/show-versions.py` & `tiledbsoma-1.9.5/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.9.5/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/pyproject.toml` & `tiledbsoma-1.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/setup.py` & `tiledbsoma-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/__init__.py` & `tiledbsoma-1.9.5/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_collection.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_collection.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_common_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_exception.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_factory.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_indexer.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_indexer.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_sparse_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_tiledb_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_tiledb_object.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_types.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/_util.py` & `tiledbsoma-1.9.5/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/common.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/common.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/common.h` & `tiledbsoma-1.9.5/src/tiledbsoma/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/eta.py` & `tiledbsoma-1.9.5/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.9.5/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/__init__.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/_common.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/_common.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/__init__.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/ambient_label_mappings.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/ambient_label_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         obs_field_name: str,
         var_field_name: str,
         context: Optional[SOMATileDBContext] = None,
     ) -> Self:
         """Acquires label-to-ID mappings from the baseline, already-written SOMA experiment."""
 
         if experiment_uri is not None:
-            if not tiledbsoma.Experiment.exists(experiment_uri):
+            if not tiledbsoma.Experiment.exists(experiment_uri, context=context):
                 raise ValueError("cannot find experiment at URI {experiment_uri}")
 
             # Pre-check
             with tiledbsoma.Experiment.open(experiment_uri, context=context) as exp:
                 if measurement_name not in exp.ms:
                     raise ValueError(
                         f"cannot append: target measurement {measurement_name} is not in experiment {experiment_uri}"
```

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/id_mappings.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/id_mappings.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/_registration/signatures.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/_registration/signatures.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/_util.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/ingest.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/io/outgest.py` & `tiledbsoma-1.9.5/src/tiledbsoma/io/outgest.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/logging.py` & `tiledbsoma-1.9.5/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.9.5/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.9.5/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/reindexer.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/reindexer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_array.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_collection.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_collection.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_context.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_context.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_dataframe.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_dataframe.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_dense_ndarray.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_dense_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_group.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_object.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_object.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma/soma_sparse_ndarray.cc` & `tiledbsoma-1.9.5/src/tiledbsoma/soma_sparse_ndarray.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.9.5/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.9.4
+Version: 1.9.5
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.9.4/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.9.5/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.9.4/version.py` & `tiledbsoma-1.9.5/version.py`

 * *Files identical despite different names*

