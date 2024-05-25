# Comparing `tmp/kuzu-0.4.3.dev8.tar.gz` & `tmp/kuzu-0.4.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.3.dev8.tar", last modified: Wed May 22 08:04:57 2024, max compression
+gzip compressed data, was "kuzu-0.4.3.dev9.tar", last modified: Thu May 23 08:04:51 2024, max compression
```

## Comparing `kuzu-0.4.3.dev8.tar` & `kuzu-0.4.3.dev9.tar`

### file list

```diff
@@ -1,2848 +1,2848 @@
-drwx------   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:57.592278 sdist/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 08:04:51.844297 sdist/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 08:04:53.416293 sdist/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-22 08:04:51.848297 sdist/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-22 08:04:53.416293 sdist/README_PYTHON_BUILD.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:57.404278 sdist/kuzu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:57.404278 sdist/kuzu-source/
--rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-05-22 08:04:54.000000 sdist/kuzu-source/.clang-format
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-22 08:04:54.000000 sdist/kuzu-source/.clang-tidy
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-22 08:04:54.000000 sdist/kuzu-source/.clang-tidy-analyzer
--rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-05-22 08:04:54.000000 sdist/kuzu-source/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-05-22 08:04:54.000000 sdist/kuzu-source/.lcovrc
--rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-05-22 08:04:54.000000 sdist/kuzu-source/CLA.md
--rw-rw-r--   0 runner    (1001) docker     (127)     9844 2024-05-22 08:04:54.000000 sdist/kuzu-source/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-05-22 08:04:54.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-22 08:04:54.000000 sdist/kuzu-source/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-22 08:04:54.000000 sdist/kuzu-source/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     6868 2024-05-22 08:04:54.000000 sdist/kuzu-source/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-05-22 08:04:54.000000 sdist/kuzu-source/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    27670 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
--rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
--rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/check-include-guards.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
--rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
--rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
--rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
--rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)      293 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/generate_binary_datasets.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
--rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/http-server.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
--rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/pip-package/
--rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/pip-package/README.md
--rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     4432 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/pip-package/setup.py
--rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/run-clang-format.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-22 08:04:54.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/
--rw-rw-r--   0 runner    (1001) docker     (127)     2644 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    27670 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/
--rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1226 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21973 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6114 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2115 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5283 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32718 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3636 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11880 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17247 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/bind_use_database.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8100 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/read/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5724 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2013 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2202 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15097 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1284 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1677 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3195 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8265 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      807 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7048 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      472 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11384 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/node_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1315 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/node_rel_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1022 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression/variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5187 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6353 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      699 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9929 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6783 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5310 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2653 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/data_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1122 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7617 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19821 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/c_api/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    22055 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1547 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1295 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2516 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5183 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3770 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4535 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4874 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/sequence_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6589 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8047 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1605 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/catalog/property.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    24685 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10576 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    35459 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5340 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/constants.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3100 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2669 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12601 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      377 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/exception/exception.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2665 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/exception/message.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/expression_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15088 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3024 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      977 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/md5.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/metric.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8989 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/null_mask.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/profiler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/random_engine.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2842 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/sha256.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/signal/
--rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/signal/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/signal/register.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5079 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/string_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/system_message.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2748 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/task_system/task.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9750 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/type_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4494 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/blob.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/date_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1174 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    58160 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/uuid.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2379 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    35482 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/types/value/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1298 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3332 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28656 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/common/windows_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3322 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1545 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9731 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1280 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      239 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/extension/catalog_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/extension/extension.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3878 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5533 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/array/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/array/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7204 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/array/array_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1328 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/array/array_value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20338 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5428 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    33750 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/date/
--rw-rw-r--   0 runner    (1001) docker     (127)      183 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/date/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      671 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/date/date_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/find_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13035 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/function_collection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/
--rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2745 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_agg_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1855 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_any_value_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2618 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_append_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2166 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_concat_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_contains_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2146 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_creation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_distinct_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2189 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1184 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_position_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2488 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_prepend_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3640 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_range_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_reverse_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3355 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_slice_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_sort_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_to_string_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2240 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/list_unique_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1904 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/list/size_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/map/
--rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/map/map_creation_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/map/map_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      961 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/map/map_keys_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/map/map_values_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2255 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/length_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1144 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/nodes_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3841 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/properties_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1164 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/rels_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1997 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/path/semantic_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1775 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/sequence/
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/sequence/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1994 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/sequence/sequence_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/struct/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2617 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/struct/struct_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3356 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/struct/struct_pack_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      387 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/checkpoint.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2232 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/show_attached_databases.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5816 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5195 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/show_sequences.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4154 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11070 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5471 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/union/
--rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/union/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/union/union_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/union/union_tag_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1873 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/union/union_value_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/
--rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3471 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/coalesce.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3205 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/constant_or_null.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1277 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/count_if.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      870 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/error.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      892 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/md5.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1455 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/nullif.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1534 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/utility/typeof.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18398 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47661 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5487 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9214 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14505 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      573 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)    12916 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
--rw-rw-r--   0 runner    (1001) docker     (127)      592 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_attach_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_database_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1874 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_export_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      713 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      877 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_import_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1140 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1001 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3141 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/bound_use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3438 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      594 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      938 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_sequence_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5837 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4768 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2480 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4539 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3650 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2736 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5949 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2370 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6587 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
--rw-rw-r--   0 runner    (1001) docker     (127)      608 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)      811 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1345 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      773 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1432 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      611 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/c_api/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    50669 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)     7595 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)     3000 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/dummy_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1286 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2690 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1720 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1392 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2704 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/sequence_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3749 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2385 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1894 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/catalog/property.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/api.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2921 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1245 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/assert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/column_data_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4183 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/concurrent_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9497 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/constants.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2116 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      492 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1203 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      571 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
--rw-rw-r--   0 runner    (1001) docker     (127)      287 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)      296 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/exception.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/io.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/message.h
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
--rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/test.h
--rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)     1066 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2470 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2068 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2067 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1863 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/keyword/
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/md5.h
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/metric.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/null_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9142 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/null_mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/profiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)      351 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/random_engine.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2229 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/static_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/string_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4653 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/system_message.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/task_system/task.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/timer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11129 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/type_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/blob.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/date_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)    19577 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/types.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/uuid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21563 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/types/value/value.h
--rw-rw-r--   0 runner    (1001) docker     (127)      782 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13651 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/common/windows_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      404 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/extension/catalog_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1491 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/extension/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/extension/extension_action.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)     3518 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4091 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2903 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6996 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24872 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/blob/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/blob/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/boolean/
--rw-rw-r--   0 runner    (1001) docker     (127)    15040 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3911 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      539 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7573 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8003 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/comparison/
--rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10062 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/date/
--rw-rw-r--   0 runner    (1001) docker     (127)     4820 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1510 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2897 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/function_collection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/hash/
--rw-rw-r--   0 runner    (1001) docker     (127)     6081 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/interval/
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1206 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1312 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_to_string_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1231 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3221 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2268 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/null/
--rw-rw-r--   0 runner    (1001) docker     (127)     2749 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)     6247 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1133 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      789 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10779 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/scalar_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/schema/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/sequence/
--rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/sequence/sequence_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5537 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)     1702 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4127 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/table_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21690 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/timestamp/
--rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/udf_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8381 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/union/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/union/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/utility/
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/utility/function_string_bind_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/utility/vector_utility_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/uuid/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/uuid/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      438 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/attached_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1450 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/client_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6985 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/client_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7803 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5111 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      812 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/database_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1851 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/db_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1463 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/kuzu.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3470 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/plan_printer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1682 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4968 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/query_summary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6918 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/settings.h
--rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/storage_driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/main/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1982 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3621 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6653 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2393 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      475 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1772 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/database_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      460 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/create_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      867 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/create_sequence_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
--rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3173 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1495 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/parsed_data/
--rw-rw-r--   0 runner    (1001) docker     (127)      480 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2755 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      954 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/port_db.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1500 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      592 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13030 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/transformer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      330 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1359 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
--rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      863 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1004 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1107 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1041 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3611 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6044 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      852 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_simple.h
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/sip/
--rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
--rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16701 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/planner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/data_pos.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/execution_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)    11095 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3664 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1361 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_sequence.h
--rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      820 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1242 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)     4405 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4687 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3282 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     2787 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2426 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3239 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2850 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1583 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5846 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5440 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5761 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1481 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1359 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4637 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1881 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3427 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6782 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7424 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
--rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4081 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4999 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6229 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5296 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2873 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1067 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1913 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2179 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1085 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      807 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/database_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      696 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      690 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      941 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/install_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/load_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/simple.h
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/simple/use_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13122 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/processor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/processor_task.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12804 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3030 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/factorized_table_schema.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/factorized_table_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1519 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)    10155 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)    15859 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/file_handle.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)    14362 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1656 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2296 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7541 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)     2514 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3159 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9200 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3125 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4449 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3147 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)     2297 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16597 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4969 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8115 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)     4852 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14251 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9626 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3021 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5856 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3467 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6212 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7138 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12842 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2910 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2397 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/undo_buffer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6109 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)     2787 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/transaction/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3396 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1676 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/attached_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22019 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/client_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5780 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2483 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/database_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/db_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/plan_printer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4305 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/storage_driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/main/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9985 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5363 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13464 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/create_macro.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4587 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10461 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2722 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2639 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transform/transform_use_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/transformer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/
--rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      678 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6271 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5973 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      185 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/simple/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/operator/simple/logical_simple.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1074 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1310 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13578 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7525 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27311 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2684 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6062 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3711 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/query_planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4798 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8210 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9149 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15415 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4131 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3111 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5184 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1560 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2008 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4299 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6872 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3425 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4736 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8000 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    36261 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5452 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4824 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1388 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2972 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      310 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      586 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/create_sequence.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      758 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_sequence.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2472 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1148 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2056 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8164 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9244 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4450 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     9643 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14049 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9038 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12676 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7757 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8358 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5010 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4759 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7210 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3034 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11774 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
--rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8578 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6515 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13924 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24123 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5989 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    30053 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1404 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13995 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13456 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11290 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6494 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16444 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11700 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8541 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1022 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7361 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5063 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12941 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2478 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3737 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      792 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      675 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4537 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4683 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/export_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/import_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/install_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2205 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/load_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      616 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/simple/use_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2443 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2677 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2416 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/processor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/processor_task.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7137 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    30659 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/factorized_table_schema.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2744 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/factorized_table_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2287 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6820 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15736 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2145 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35355 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/file_handle.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    33537 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17160 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6051 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12337 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6968 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7988 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5521 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4338 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5792 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11516 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5262 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21095 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4291 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2108 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43152 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27570 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10644 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22097 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16059 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9501 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10804 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8460 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9148 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    51121 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11782 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7813 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9257 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6184 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1774 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7688 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/undo_buffer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4121 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5210 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13919 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)      240 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      611 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/transaction/transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2976 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6237 2024-05-22 08:04:54.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)      489 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/
--rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    58616 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   493757 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     3378 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    92992 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/
--rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
--rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
--rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
--rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
--rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
--rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
--rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
--rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4216 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
--rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
--rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
--rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/
--rw-rw-r--   0 runner    (1001) docker     (127)     5677 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12841 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      652 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/README
--rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      314 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/SECURITY.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.c
--rw-rw-r--   0 runner    (1001) docker     (127)     8011 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7965 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/context.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4666 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/context.h
--rw-rw-r--   0 runner    (1001) docker     (127)   122784 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin
--rw-rw-r--   0 runner    (1001) docker     (127)    51687 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin.br
--rw-rw-r--   0 runner    (1001) docker     (127)   472009 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1951 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.c
--rw-rw-r--   0 runner    (1001) docker     (127)    18385 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17424 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2413 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10677 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/common/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/
--rw-rw-r--   0 runner    (1001) docker     (127)     2285 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)    14854 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)   103991 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/decode.c
--rw-rw-r--   0 runner    (1001) docker     (127)    11996 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.h
--rw-rw-r--   0 runner    (1001) docker     (127)    31612 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/prefix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5659 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.c
--rw-rw-r--   0 runner    (1001) docker     (127)    12546 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/
--rw-rw-r--   0 runner    (1001) docker     (127)     5673 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1301 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36639 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8181 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1685 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4109 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1137 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_encoder_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7395 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18673 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    50750 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3477 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1485 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11826 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1019 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.c
--rw-rw-r--   0 runner    (1001) docker     (127)     6892 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6645 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)    33255 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3598 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27182 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2879 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.h
--rw-rw-r--   0 runner    (1001) docker     (127)   147154 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.c
--rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.h
--rw-rw-r--   0 runner    (1001) docker     (127)    77547 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/encode.c
--rw-rw-r--   0 runner    (1001) docker     (127)    23290 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.c
--rw-rw-r--   0 runner    (1001) docker     (127)     5046 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14584 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4057 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    32951 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2194 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/find_match_length.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24481 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5097 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_composite_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11250 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_forgetful_chain_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10413 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match64_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10349 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9414 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_quickly_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7226 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_rolling_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13081 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_to_binary_tree_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1875 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1401 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5839 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.c
--rw-rw-r--   0 runner    (1001) docker     (127)      916 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5630 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4358 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26659 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4051 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7642 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/params.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1969 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/prefix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7592 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/quality.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6009 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/ringbuffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3040 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/state.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21117 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.h
--rw-rw-r--   0 runner    (1001) docker     (127)   469710 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict_lut.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2269 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.c
--rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/enc/write_bits.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/
--rw-rw-r--   0 runner    (1001) docker     (127)      338 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/BUILD.bazel
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/WORKSPACE.bazel
--rw-rw-r--   0 runner    (1001) docker     (127)     1837 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/decode_fuzzer.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1073 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/run_decode_fuzzer.c
--rwxrwxr-x   0 runner    (1001) docker     (127)      703 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/test_fuzzer.sh
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/
--rw-rw-r--   0 runner    (1001) docker     (127)    16886 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/decode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    19841 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/encode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11439 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/port.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/shared_dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2615 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/types.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)    51996 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4028 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)   215208 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/brotli-comparison-study-2015-09-22.pdf
--rw-rw-r--   0 runner    (1001) docker     (127)     5130 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.1
--rw-rw-r--   0 runner    (1001) docker     (127)      244 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.svg
--rw-rw-r--   0 runner    (1001) docker     (127)     1767 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/constants.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)    17452 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/decode.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)    24109 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/encode.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/docs/types.h.3
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/
--rw-rw-r--   0 runner    (1001) docker     (127)     6077 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/shared-brotli-fetch-spec.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/
--rw-rw-r--   0 runner    (1001) docker     (127)      176 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-01-download-rfc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      882 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-02-rfc-to-bin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      875 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-03-validate-bin.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2214 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-04-generate-java-literals.py
--rwxrwxr-x   0 runner    (1001) docker     (127)      283 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/download_testdata.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlicommon.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlidec.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlienc.pc.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fast_float/
--rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fast_float/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/README
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/glob/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/httplib/
--rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/httplib/httplib.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
--rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
--rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/
--rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26309 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
--rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
--rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
--rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3470 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
--rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
--rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
--rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniz/
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
--rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniz/LICENSE
--rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/nlohmann_json/
--rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pcg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pcg/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
--rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
--rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
--rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
--rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pyparse/
--rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/compile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/logging.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/mix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/prog.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
--rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/utf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/prog.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/re2.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/rune.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/include/serd.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
--rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/base64.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/env.c
--rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/n3.c
--rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/node.c
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/stack.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/string.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/system.c
--rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/system.h
--rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/try.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/uri.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/serd/src/writer.c
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
--rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
--rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
--rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
--rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)   154517 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
--rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
--rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/taywee_args/
--rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/taywee_args/include/
--rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/
--rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
--rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
--rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
--rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-05-22 08:04:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/example/
--rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/benchmark/main.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/jni/
--rw-rw-r--   0 runner    (1001) docker     (127)    52884 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
--rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2637 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
--rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     9598 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
--rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
--rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1454 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1663 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
--rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/test.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/build.js
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4446 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/install.js
--rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/package.js
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/package.json
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     4385 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1567 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5760 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4098 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2332 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4835 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14214 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
--rw-rw-r--   0 runner    (1001) docker     (127)    10896 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4009 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
--rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
--rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
--rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4951 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     2212 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
--rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
--rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
--rw-rw-r--   0 runner    (1001) docker     (127)     9201 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
--rw-rw-r--   0 runner    (1001) docker     (127)    10088 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
--rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
--rw-rw-r--   0 runner    (1001) docker     (127)     6242 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
--rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
--rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3938 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1959 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_udf.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2219 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)     9637 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)     3945 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21636 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16192 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7703 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7733 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_udf.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4410 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/
--rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8353 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
--rw-rw-r--   0 runner    (1001) docker     (127)     9620 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
--rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14438 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
--rw-rw-r--   0 runner    (1001) docker     (127)    24584 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)      879 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_connection.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2687 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_database.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
--rw-rw-r--   0 runner    (1001) docker     (127)    20051 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2331 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
--rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
--rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4300 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_issue.py
--rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8013 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14156 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
--rw-rw-r--   0 runner    (1001) docker     (127)    24852 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas_pyarrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1422 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_scan_polars.py
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
--rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5062 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_udf.py
--rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/
--rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
--rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     5878 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/build.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9653 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
-lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:57.168279 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     5838 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
--rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12852 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11867 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12831 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     9314 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/rust_api/update_version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/
--rw-rw-r--   0 runner    (1001) docker     (127)      699 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    27833 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3212 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/conftest.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/files/
--rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
--rw-rw-r--   0 runner    (1001) docker     (127)     1393 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4790 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4804 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
--rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-05-22 08:04:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:04:57.592278 sdist/kuzu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-22 08:04:57.592278 sdist/kuzu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 08:04:57.596278 sdist/kuzu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:04:57.592278 sdist/kuzu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 08:04:57.592278 sdist/kuzu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:04:57.592278 sdist/kuzu.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-22 08:04:57.404278 sdist/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 08:04:53.416293 sdist/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-22 08:04:53.416293 sdist/setup.py
+drwx------   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:51.401648 sdist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 08:04:45.089683 sdist/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 08:04:46.669674 sdist/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-23 08:04:45.089683 sdist/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-23 08:04:46.669674 sdist/README_PYTHON_BUILD.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:50.749652 sdist/kuzu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:50.749652 sdist/kuzu-source/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-05-23 08:04:47.000000 sdist/kuzu-source/.clang-format
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-23 08:04:47.000000 sdist/kuzu-source/.clang-tidy
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-23 08:04:47.000000 sdist/kuzu-source/.clang-tidy-analyzer
+-rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-05-23 08:04:47.000000 sdist/kuzu-source/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-05-23 08:04:47.000000 sdist/kuzu-source/.lcovrc
+-rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-05-23 08:04:47.000000 sdist/kuzu-source/CLA.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     9844 2024-05-23 08:04:47.000000 sdist/kuzu-source/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-05-23 08:04:47.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-23 08:04:47.000000 sdist/kuzu-source/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-23 08:04:47.000000 sdist/kuzu-source/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     6868 2024-05-23 08:04:47.000000 sdist/kuzu-source/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-05-23 08:04:47.000000 sdist/kuzu-source/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    27670 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
+-rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
+-rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/check-include-guards.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
+-rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
+-rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)      293 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/generate_binary_datasets.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/http-server.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/
+-rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/README.md
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     4432 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/setup.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/run-clang-format.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-23 08:04:47.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2644 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    27670 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/
+-rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1226 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21973 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6114 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2115 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5283 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32718 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3636 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11880 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17247 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_use_database.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8100 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5724 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2013 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2202 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15097 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1284 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1677 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3195 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8265 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      807 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7048 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      472 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11384 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/node_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1315 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/node_rel_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1022 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression/variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5187 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6353 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      699 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9929 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6783 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5310 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2653 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/data_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1122 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7617 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19821 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/c_api/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22094 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1547 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1295 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2516 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5183 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3770 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4535 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4874 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/sequence_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6589 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8047 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1605 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/catalog/property.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    24685 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10576 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    35459 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5340 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/constants.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3100 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2669 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12601 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      377 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/exception/exception.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2665 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/exception/message.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/expression_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15088 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2799 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      977 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/md5.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/metric.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8989 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/null_mask.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/profiler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/random_engine.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2842 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/sha256.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/signal/
+-rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/signal/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/signal/register.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5079 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/string_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/system_message.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2748 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/task_system/task.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9750 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/type_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4494 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/blob.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/date_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1174 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    58160 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/uuid.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2379 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    35482 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/types/value/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1298 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3332 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28656 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/common/windows_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3322 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1545 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9731 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1280 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      239 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/extension/catalog_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/extension/extension.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3878 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5533 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/array/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/array/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7204 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/array/array_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1328 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/array/array_value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20338 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5428 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    33750 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/date/
+-rw-rw-r--   0 runner    (1001) docker     (127)      183 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/date/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      671 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/date/date_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/find_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13035 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/function_collection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/
+-rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2745 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_agg_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1855 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_any_value_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2618 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_append_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2166 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_concat_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_contains_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2146 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_creation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_distinct_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2189 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1184 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_position_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2488 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_prepend_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3640 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_range_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_reverse_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3355 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_slice_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_sort_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_to_string_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2240 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/list_unique_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1904 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/list/size_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/map/map_creation_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/map/map_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      961 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/map/map_keys_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/map/map_values_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2255 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/length_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1144 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/nodes_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3841 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/properties_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1164 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/rels_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1997 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/path/semantic_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1775 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/sequence/
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/sequence/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1994 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/sequence/sequence_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/struct/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2617 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/struct/struct_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3356 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/struct/struct_pack_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      387 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/checkpoint.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2232 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_attached_databases.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5816 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5195 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_sequences.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4154 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11070 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5471 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/union/
+-rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/union/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/union/union_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/union/union_tag_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1873 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/union/union_value_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/
+-rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3471 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/coalesce.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3205 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/constant_or_null.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1277 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/count_if.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      870 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/error.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      892 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/md5.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1455 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/nullif.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1534 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/utility/typeof.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18398 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47661 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5487 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9214 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14505 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      573 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12916 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      592 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_attach_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_database_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1874 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_export_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      713 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      877 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_import_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1140 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1001 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3141 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3438 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      594 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      938 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_sequence_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5837 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4768 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2480 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4539 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3650 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2736 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5949 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2370 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6587 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      608 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      811 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1345 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      773 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1432 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      611 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/c_api/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    50669 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7906 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3000 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/dummy_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1286 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2690 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1720 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1392 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2704 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/sequence_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3749 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2385 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1894 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/catalog/property.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/api.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2921 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1245 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/assert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/column_data_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4183 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/concurrent_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9497 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/constants.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2116 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      492 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1203 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      571 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      287 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      296 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      403 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/exception.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/io.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/message.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/test.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1066 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2470 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2068 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1908 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1863 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/keyword/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/md5.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/metric.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/null_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9142 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/null_mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/profiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      351 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/random_engine.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2229 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/static_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/string_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4653 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/system_message.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/task.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/timer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11129 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/type_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/blob.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/date_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    19577 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/uuid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21563 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/value.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      782 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13651 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/common/windows_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      404 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/extension/catalog_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1491 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/extension/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/extension/extension_action.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3518 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4091 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2903 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6996 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24872 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15040 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3911 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      539 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7573 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8003 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/comparison/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10062 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/date/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4820 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1510 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2897 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/function_collection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6081 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/interval/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1206 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1312 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_to_string_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1231 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3221 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2268 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/null/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2749 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6247 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1133 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      789 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10779 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/scalar_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/sequence/
+-rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/sequence/sequence_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5537 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1702 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4127 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/table_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21690 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/timestamp/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/udf_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8381 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/union/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/union/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/utility/
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/utility/function_string_bind_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/utility/vector_utility_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      438 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1371 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/attached_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1450 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/client_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6985 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/client_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7803 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5111 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      812 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/database_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1851 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/db_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1463 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/kuzu.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3470 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/plan_printer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1682 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4968 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/query_summary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6918 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/settings.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/storage_driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/main/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1982 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3621 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6653 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2393 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      475 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1772 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/database_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      460 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/create_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      867 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/create_sequence_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3173 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1495 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_data/
+-rw-rw-r--   0 runner    (1001) docker     (127)      480 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2755 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      954 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/port_db.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1500 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      592 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13030 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/transformer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      330 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1359 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      863 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1004 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1107 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1041 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3611 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6044 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      852 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_simple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/sip/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16701 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/planner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/data_pos.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/execution_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11095 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3664 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1361 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_sequence.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      820 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1242 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4405 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4687 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3282 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2787 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2426 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3239 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2850 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1583 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5846 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5440 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5860 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1481 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1359 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4637 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1881 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3427 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6782 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7424 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4419 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4081 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4999 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6229 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5296 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2873 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1067 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1913 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2179 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1085 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      807 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/database_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      696 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      690 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      941 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/install_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/load_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/simple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/use_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13122 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/processor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/processor_task.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12804 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3030 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/factorized_table_schema.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/factorized_table_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1519 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10185 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13111 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2885 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15859 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3515 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/file_handle.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14415 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1656 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2296 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7541 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2514 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3159 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9200 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3163 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4479 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3373 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2297 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16597 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5037 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8115 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4852 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14175 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9626 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5846 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3467 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6336 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3487 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2524 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7182 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12906 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2906 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2397 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/undo_buffer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2577 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6109 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2787 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2482 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3396 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2311 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/attached_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22019 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/client_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5794 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2483 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/database_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/db_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/plan_printer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4305 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/storage_driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/main/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9985 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5363 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13464 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/create_macro.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4587 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10461 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2722 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2639 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_use_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/transformer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/
+-rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      678 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6271 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5973 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      185 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/simple/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/operator/simple/logical_simple.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1074 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1310 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13578 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7525 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27311 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2684 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6062 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3711 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/query_planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4798 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8210 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9149 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15415 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4131 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3111 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5184 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1560 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2008 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4299 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6872 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3425 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4736 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8000 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    36261 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5452 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4824 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1388 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2972 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      310 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1375 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      586 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/create_sequence.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      749 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_sequence.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2472 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1148 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2056 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8164 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9244 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4450 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     9643 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14049 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9038 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12676 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7757 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8358 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5010 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4759 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7210 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3034 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
+-rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8578 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6515 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13924 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24123 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5989 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    30053 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1404 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13995 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13456 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11395 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6494 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16444 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11700 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8541 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1022 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7361 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5063 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12941 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2478 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3737 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      792 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      675 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5159 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4537 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4683 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/export_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/import_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/install_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2205 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/load_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      616 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/use_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2443 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2677 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2416 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/processor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/processor_task.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7137 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    30659 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/factorized_table_schema.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2744 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/factorized_table_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2287 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6859 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15736 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2192 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35355 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1950 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/file_handle.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    33653 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17160 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6051 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12337 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6968 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7988 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4398 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5832 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11930 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5262 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21095 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4291 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2108 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43158 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27570 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10742 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22186 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16059 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9583 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10906 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8475 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9148 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    51559 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11756 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7813 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9257 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6184 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1774 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7688 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/undo_buffer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4169 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5210 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13949 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)      240 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      611 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/transaction/transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2976 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6267 2024-05-23 08:04:47.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)      489 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/
+-rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    58616 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   493757 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3378 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    92992 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
+-rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4216 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
+-rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
+-rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5677 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12841 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      652 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/README
+-rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      314 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/SECURITY.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     8011 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7965 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/context.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4666 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   122784 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin
+-rw-rw-r--   0 runner    (1001) docker     (127)    51687 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin.br
+-rw-rw-r--   0 runner    (1001) docker     (127)   472009 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1951 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    18385 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17424 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2413 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10677 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2285 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    14854 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   103991 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/decode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    11996 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    31612 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/prefix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5659 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    12546 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5673 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1301 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36639 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8181 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1685 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4109 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1137 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_encoder_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7395 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18673 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    50750 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3477 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1485 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11826 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1019 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     6892 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6645 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    33255 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3598 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27182 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2879 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   147154 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    77547 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/encode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    23290 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     5046 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14584 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4057 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    32951 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2194 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/find_match_length.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24481 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5097 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_composite_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11250 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_forgetful_chain_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10413 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match64_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10349 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9414 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_quickly_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7226 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_rolling_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13081 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_to_binary_tree_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1875 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1401 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5839 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      916 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5630 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4358 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26659 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4051 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7642 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/params.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1969 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/prefix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7592 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/quality.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6009 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/ringbuffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3040 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21117 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   469710 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict_lut.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2269 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/write_bits.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      338 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/BUILD.bazel
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/WORKSPACE.bazel
+-rw-rw-r--   0 runner    (1001) docker     (127)     1837 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/decode_fuzzer.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1073 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/run_decode_fuzzer.c
+-rwxrwxr-x   0 runner    (1001) docker     (127)      703 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/test_fuzzer.sh
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (127)    16886 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/decode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    19841 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/encode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11439 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/port.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/shared_dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2615 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/types.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51996 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4028 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)   215208 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/brotli-comparison-study-2015-09-22.pdf
+-rw-rw-r--   0 runner    (1001) docker     (127)     5130 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.1
+-rw-rw-r--   0 runner    (1001) docker     (127)      244 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.svg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1767 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/constants.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)    17452 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/decode.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)    24109 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/encode.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/types.h.3
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6077 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/shared-brotli-fetch-spec.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/
+-rw-rw-r--   0 runner    (1001) docker     (127)      176 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-01-download-rfc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      882 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-02-rfc-to-bin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      875 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-03-validate-bin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2214 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-04-generate-java-literals.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)      283 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/download_testdata.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlicommon.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlidec.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlienc.pc.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/
+-rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/README
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/glob/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/httplib/
+-rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/httplib/httplib.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/
+-rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26309 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3470 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniz/LICENSE
+-rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/nlohmann_json/
+-rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pcg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pcg/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pyparse/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/compile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/logging.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/mix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/prog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/utf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/prog.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/re2.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/rune.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/include/serd.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/base64.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/env.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/n3.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/node.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/stack.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/string.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/system.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/try.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/uri.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/writer.c
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   154517 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/
+-rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-05-23 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/example/
+-rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/benchmark/main.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/jni/
+-rw-rw-r--   0 runner    (1001) docker     (127)    52884 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2637 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     9598 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1454 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1663 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
+-rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/test.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/build.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4446 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/install.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/package.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/package.json
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4385 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1567 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5760 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4098 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2332 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4835 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14214 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10896 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4009 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4951 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2212 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     9201 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    10088 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     6242 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1322 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3938 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1959 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      379 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_udf.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2219 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9637 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3945 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6572 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21636 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16192 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7703 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7733 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_udf.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4410 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8353 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     9620 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14438 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    24584 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      879 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_connection.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2687 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    20051 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2331 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4300 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_issue.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8013 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14156 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    24852 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas_pyarrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1422 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_scan_polars.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5062 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_udf.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
+-rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5878 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/build.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9653 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
+lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:50.513653 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     5838 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12852 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11867 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12831 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     9314 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/rust_api/update_version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/
+-rw-rw-r--   0 runner    (1001) docker     (127)      699 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    27833 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3212 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/conftest.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/files/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
+-rw-rw-r--   0 runner    (1001) docker     (127)     1393 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4790 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4804 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-05-23 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:04:51.401648 sdist/kuzu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-23 08:04:51.401648 sdist/kuzu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 08:04:51.401648 sdist/kuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:04:51.401648 sdist/kuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 08:04:51.401648 sdist/kuzu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:04:51.401648 sdist/kuzu.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-23 08:04:50.749652 sdist/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 08:04:46.669674 sdist/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-23 08:04:46.669674 sdist/setup.py
```

### sdist/kuzu-source/CMakeLists.txt

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.15)
 
-project(Kuzu VERSION 0.4.3.8 LANGUAGES CXX C)
+project(Kuzu VERSION 0.4.3.9 LANGUAGES CXX C)
 
 find_package(Threads REQUIRED)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
 set(CMAKE_CXX_VISIBILITY_PRESET hidden)
 set(CMAKE_C_VISIBILITY_PRESET hidden)
@@ -252,15 +252,15 @@
 include_directories(third_party/pcg)
 
 add_subdirectory(third_party)
 
 if(${BUILD_KUZU})
 add_definitions(-DKUZU_ROOT_DIRECTORY="${PROJECT_SOURCE_DIR}")
 add_definitions(-DKUZU_CMAKE_VERSION="${CMAKE_PROJECT_VERSION}")
-add_definitions(-DKUZU_EXTENSION_VERSION="0.3.7")
+add_definitions(-DKUZU_EXTENSION_VERSION="0.3.8")
 
 include_directories(src/include)
 
 add_subdirectory(src)
 if (${BUILD_TESTS})
     add_definitions(-DTEST_FILES_DIR="test/test_files")
     add_subdirectory(test)
```

### sdist/kuzu-source/src/catalog/catalog.cpp

```diff
@@ -366,18 +366,18 @@
     serializer.serializeValue(StorageVersionInfo::getStorageVersion());
     tables->serialize(serializer);
     sequences->serialize(serializer);
     functions->serialize(serializer);
 }
 
 void Catalog::readFromFile(const std::string& directory, common::VirtualFileSystem* fs,
-    common::FileVersionType versionType) {
+    common::FileVersionType versionType, main::ClientContext* context) {
     auto catalogPath = StorageUtils::getCatalogFilePath(fs, directory, versionType);
     Deserializer deserializer(
-        std::make_unique<BufferedFileReader>(fs->openFile(catalogPath, O_RDONLY)));
+        std::make_unique<BufferedFileReader>(fs->openFile(catalogPath, O_RDONLY, context)));
     validateMagicBytes(deserializer);
     storage_version_t savedStorageVersion;
     deserializer.deserializeValue(savedStorageVersion);
     validateStorageVersion(savedStorageVersion);
     tables = CatalogSet::deserialize(deserializer);
     sequences = CatalogSet::deserialize(deserializer);
     functions = CatalogSet::deserialize(deserializer);
```

### sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp

```diff
@@ -3,29 +3,27 @@
 #include "common/assert.h"
 #include "common/file_system/local_file_system.h"
 #include "main/client_context.h"
 
 namespace kuzu {
 namespace common {
 
-VirtualFileSystem::VirtualFileSystem(main::Database* database)
-    : context{std::make_unique<main::ClientContext>(database)} {
+VirtualFileSystem::VirtualFileSystem() {
     defaultFS = std::make_unique<LocalFileSystem>();
 }
 
 VirtualFileSystem::~VirtualFileSystem() = default;
 
 void VirtualFileSystem::registerFileSystem(std::unique_ptr<FileSystem> fileSystem) {
     subSystems.push_back(std::move(fileSystem));
 }
 
 std::unique_ptr<FileInfo> VirtualFileSystem::openFile(const std::string& path, int flags,
-    main::ClientContext* userContext, FileLockType lockType) {
-    return findFileSystem(path)->openFile(path, flags,
-        userContext == nullptr ? this->context.get() : userContext, lockType);
+    main::ClientContext* context, FileLockType lockType) {
+    return findFileSystem(path)->openFile(path, flags, context, lockType);
 }
 
 std::vector<std::string> VirtualFileSystem::glob(main::ClientContext* context,
     const std::string& path) const {
     return findFileSystem(path)->glob(context, path);
 }
 
@@ -38,17 +36,14 @@
 }
 
 void VirtualFileSystem::removeFileIfExists(const std::string& path) {
     findFileSystem(path)->removeFileIfExists(path);
 }
 
 bool VirtualFileSystem::fileOrPathExists(const std::string& path, main::ClientContext* context) {
-    if (context == nullptr) {
-        context = this->context.get();
-    }
     return findFileSystem(path)->fileOrPathExists(path, context);
 }
 
 std::string VirtualFileSystem::expandPath(main::ClientContext* context,
     const std::string& path) const {
     return findFileSystem(path)->expandPath(context, path);
 }
```

### sdist/kuzu-source/src/include/catalog/catalog.h

```diff
@@ -1,13 +1,17 @@
 #pragma once
 
 #include "catalog/catalog_set.h"
 #include "common/cast.h"
 
 namespace kuzu {
+namespace main {
+class AttachedKuzuDatabase;
+} // namespace main
+
 namespace binder {
 struct BoundAlterInfo;
 struct BoundCreateTableInfo;
 struct BoundCreateSequenceInfo;
 } // namespace binder
 
 namespace function {
@@ -28,14 +32,16 @@
 class RelTableCatalogEntry;
 class RelGroupCatalogEntry;
 class RDFGraphCatalogEntry;
 
 class SequenceCatalogEntry;
 
 class Catalog {
+    friend class main::AttachedKuzuDatabase;
+
 public:
     // This is extended by DuckCatalog and PostgresCatalog.
     KUZU_API Catalog();
     Catalog(std::string directory, common::VirtualFileSystem* vfs);
     virtual ~Catalog() = default;
 
     // ----------------------------- Table Schemas ----------------------------
@@ -100,16 +106,18 @@
 
     template<class TARGET>
     TARGET* ptrCast() {
         return common::ku_dynamic_cast<Catalog*, TARGET*>(this);
     }
 
 private:
+    // The clientContext needs to be used when reading from a remote filesystem which
+    // requires some user-specific configs (e.g. s3 username, password).
     void readFromFile(const std::string& directory, common::VirtualFileSystem* fs,
-        common::FileVersionType versionType);
+        common::FileVersionType versionType, main::ClientContext* context = nullptr);
     void saveToFile(const std::string& directory, common::VirtualFileSystem* fs,
         common::FileVersionType versionType);
 
 private:
     // ----------------------------- Functions ----------------------------
     void registerBuiltInFunctions();
```

### sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h

```diff
@@ -11,15 +11,15 @@
 }
 
 namespace common {
 
 class KUZU_API VirtualFileSystem final : public FileSystem {
 
 public:
-    explicit VirtualFileSystem(main::Database* database);
+    VirtualFileSystem();
 
     ~VirtualFileSystem() override;
 
     void registerFileSystem(std::unique_ptr<FileSystem> fileSystem);
 
     std::unique_ptr<FileInfo> openFile(const std::string& path, int flags,
         main::ClientContext* context = nullptr,
@@ -57,13 +57,11 @@
 
 private:
     FileSystem* findFileSystem(const std::string& path) const;
 
 private:
     std::vector<std::unique_ptr<FileSystem>> subSystems;
     std::unique_ptr<FileSystem> defaultFS;
-    // The default clientContext which is created when the database starts.
-    std::unique_ptr<main::ClientContext> context;
 };
 
 } // namespace common
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/main/attached_database.h

```diff
@@ -36,13 +36,16 @@
         ClientContext* clientContext);
 
     storage::StorageManager* getStorageManager() { return storageManager.get(); }
 
     transaction::TransactionManager* getTransactionManager() { return transactionManager.get(); }
 
 private:
+    void initCatalog(const std::string& path, ClientContext* context);
+
+private:
     std::unique_ptr<storage::StorageManager> storageManager;
     std::unique_ptr<transaction::TransactionManager> transactionManager;
 };
 
 } // namespace main
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h

```diff
@@ -108,34 +108,37 @@
     void finalize(ExecutionContext* context) override;
 
     inline std::unique_ptr<PhysicalOperator> clone() override {
         return std::make_unique<NodeBatchInsert>(info->copy(), sharedState,
             resultSetDescriptor->copy(), children[0]->clone(), id, paramsString);
     }
 
-    static void writeAndResetNewNodeGroup(common::node_group_idx_t nodeGroupIdx,
-        std::optional<IndexBuilder>& indexBuilder, common::column_id_t pkColumnID,
-        storage::NodeTable* table, storage::ChunkedNodeGroup* nodeGroup);
+    static void writeAndResetNewNodeGroup(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx, std::optional<IndexBuilder>& indexBuilder,
+        common::column_id_t pkColumnID, storage::NodeTable* table,
+        storage::ChunkedNodeGroup* nodeGroup);
 
     // The node group will be reset so that the only values remaining are the ones which were not
     // written
-    void writeAndResetNodeGroup(common::node_group_idx_t nodeGroupIdx, ExecutionContext* context,
+    void writeAndResetNodeGroup(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx,
         std::unique_ptr<storage::ChunkedNodeGroup>& nodeGroup,
         std::optional<IndexBuilder>& indexBuilder);
 
 private:
     // Returns the number of nodes written from the group
     uint64_t writeToExistingNodeGroup(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, std::optional<IndexBuilder>& indexBuilder,
         common::column_id_t pkColumnID, storage::NodeTable* table,
         storage::ChunkedNodeGroup* nodeGroup);
 
-    void appendIncompleteNodeGroup(std::unique_ptr<storage::ChunkedNodeGroup> localNodeGroup,
-        std::optional<IndexBuilder>& indexBuilder, ExecutionContext* context);
+    void appendIncompleteNodeGroup(transaction::Transaction* transaction,
+        std::unique_ptr<storage::ChunkedNodeGroup> localNodeGroup,
+        std::optional<IndexBuilder>& indexBuilder);
     void clearToIndex(std::unique_ptr<storage::ChunkedNodeGroup>& nodeGroup,
         common::offset_t startIndexInGroup);
 
-    void copyToNodeGroup(ExecutionContext* context);
+    void copyToNodeGroup(transaction::Transaction* transaction);
 };
 
 } // namespace processor
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h

```diff
@@ -56,20 +56,20 @@
 
     inline std::unique_ptr<PhysicalOperator> clone() override {
         return std::make_unique<RelBatchInsert>(info->copy(), partitionerSharedState, sharedState,
             resultSetDescriptor->copy(), id, paramsString);
     }
 
 private:
-    static void appendNewNodeGroup(const RelBatchInsertInfo& relInfo,
-        RelBatchInsertLocalState& localState, BatchInsertSharedState& sharedState,
-        const PartitionerSharedState& partitionerSharedState);
-    static void mergeNodeGroup(ExecutionContext* context, const RelBatchInsertInfo& relInfo,
-        RelBatchInsertLocalState& localState, BatchInsertSharedState& sharedState,
-        const PartitionerSharedState& partitionerSharedState);
+    static void appendNewNodeGroup(transaction::Transaction* transaction,
+        const RelBatchInsertInfo& relInfo, RelBatchInsertLocalState& localState,
+        BatchInsertSharedState& sharedState, const PartitionerSharedState& partitionerSharedState);
+    static void mergeNodeGroup(transaction::Transaction* transaction,
+        const RelBatchInsertInfo& relInfo, RelBatchInsertLocalState& localState,
+        BatchInsertSharedState& sharedState, const PartitionerSharedState& partitionerSharedState);
 
     static void prepareCSRNodeGroup(const storage::ChunkedNodeGroupCollection& partition,
         common::offset_t startNodeOffset, const RelBatchInsertInfo& relInfo,
         RelBatchInsertLocalState& localState, common::offset_t numNodes);
 
     static common::length_t getGapSize(common::length_t length);
     static std::vector<common::offset_t> populateStartCSROffsetsAndLengths(
```

### sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h

```diff
@@ -143,15 +143,15 @@
     enum class FileVersionedType : uint8_t {
         VERSIONED_FILE = 0,    // The file is backed by versioned pages in wal file.
         NON_VERSIONED_FILE = 1 // The file does not have any versioned pages in wal file.
     };
 
     BMFileHandle(const std::string& path, uint8_t flags, BufferManager* bm,
         common::PageSizeClass pageSizeClass, FileVersionedType fileVersionedType,
-        common::VirtualFileSystem* vfs);
+        common::VirtualFileSystem* vfs, main::ClientContext* context);
 
     ~BMFileHandle() override;
 
     // This function assumes the page is already LOCKED.
     inline void setLockedPageDirty(common::page_idx_t pageIdx) {
         KU_ASSERT(pageIdx < numPages);
         pageStates[pageIdx].setDirty();
```

### sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h

```diff
@@ -178,19 +178,19 @@
     void removeFilePagesFromFrames(BMFileHandle& fileHandle);
     void flushAllDirtyPagesInFrames(BMFileHandle& fileHandle);
     void updateFrameIfPageIsInFrameWithoutLock(BMFileHandle& fileHandle, uint8_t* newPage,
         common::page_idx_t pageIdx);
     void removePageFromFrameIfNecessary(BMFileHandle& fileHandle, common::page_idx_t pageIdx);
 
     // For files that are managed by BM, their FileHandles should be created through this function.
-    inline std::unique_ptr<BMFileHandle> getBMFileHandle(const std::string& filePath, uint8_t flags,
+    std::unique_ptr<BMFileHandle> getBMFileHandle(const std::string& filePath, uint8_t flags,
         BMFileHandle::FileVersionedType fileVersionedType, common::VirtualFileSystem* vfs,
-        common::PageSizeClass pageSizeClass = common::PAGE_4KB) {
+        main::ClientContext* context, common::PageSizeClass pageSizeClass = common::PAGE_4KB) {
         return std::make_unique<BMFileHandle>(filePath, flags, this, pageSizeClass,
-            fileVersionedType, vfs);
+            fileVersionedType, vfs, context);
     }
     inline common::frame_group_idx_t addNewFrameGroup(common::PageSizeClass pageSizeClass) {
         return vmRegions[pageSizeClass]->addNewFrameGroup();
     }
     inline void clearEvictionQueue() { evictionQueue = std::make_unique<EvictionQueue>(); }
 
 private:
```

### sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h

```diff
@@ -5,14 +5,18 @@
 #include <mutex>
 #include <stack>
 
 #include "common/constants.h"
 #include "common/types/types.h"
 
 namespace kuzu {
+namespace main {
+class ClientContext;
+}
+
 namespace common {
 class VirtualFileSystem;
 }
 
 namespace storage {
 
 class MemoryAllocator;
@@ -32,15 +36,17 @@
     uint64_t size;
 };
 
 class MemoryAllocator {
     friend class MemoryBuffer;
 
 public:
-    explicit MemoryAllocator(BufferManager* bm, common::VirtualFileSystem* vfs);
+    MemoryAllocator(BufferManager* bm, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
+
     ~MemoryAllocator();
 
     std::unique_ptr<MemoryBuffer> allocateBuffer(bool initializeToZero, uint64_t size);
     inline common::page_offset_t getPageSize() const { return pageSize; }
 
 private:
     void freeBlock(common::page_idx_t pageIdx, uint8_t* buffer);
@@ -66,16 +72,18 @@
  * at the same time.
  *
  * MM will return a MemoryBuffer to the caller, which is a wrapper of the allocated memory block,
  * and it will automatically call its allocator to reclaim the memory block when it is destroyed.
  */
 class MemoryManager {
 public:
-    explicit MemoryManager(BufferManager* bm, common::VirtualFileSystem* vfs) : bm{bm} {
-        allocator = std::make_unique<MemoryAllocator>(bm, vfs);
+    explicit MemoryManager(BufferManager* bm, common::VirtualFileSystem* vfs,
+        main::ClientContext* context)
+        : bm{bm} {
+        allocator = std::make_unique<MemoryAllocator>(bm, vfs, context);
     }
 
     std::unique_ptr<MemoryBuffer> allocateBuffer(bool initializeToZero = false,
         uint64_t size = common::BufferPoolConstants::PAGE_256KB_SIZE) {
         return allocator->allocateBuffer(initializeToZero, size);
     }
     BufferManager* getBufferManager() const { return bm; }
```

### sdist/kuzu-source/src/include/storage/file_handle.h

```diff
@@ -5,14 +5,18 @@
 
 #include "common/assert.h"
 #include "common/constants.h"
 #include "common/file_system/file_info.h"
 #include "common/types/types.h"
 
 namespace kuzu {
+namespace main {
+class ClientContext;
+}
+
 namespace common {
 class VirtualFileSystem;
 }
 
 namespace storage {
 // FileHandle holds basic state information of a file, including FileInfo, flags, pageSize,
 // numPages, and pageCapacity. Also, FileHandle provides utility methods to read/write pages from/to
@@ -27,15 +31,16 @@
 
     // READ_ONLY subsumes DEFAULT_PAGED, PERSISTENT, and NO_CREATE.
     constexpr static uint8_t O_PERSISTENT_FILE_READ_ONLY{0b0000'1000};
     constexpr static uint8_t O_PERSISTENT_FILE_NO_CREATE{0b0000'0000};
     constexpr static uint8_t O_PERSISTENT_FILE_CREATE_NOT_EXISTS{0b0000'0100};
     constexpr static uint8_t O_IN_MEM_TEMP_FILE{0b0000'0011};
 
-    FileHandle(const std::string& path, uint8_t flags, common::VirtualFileSystem* vfs);
+    FileHandle(const std::string& path, uint8_t flags, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
     virtual ~FileHandle() = default;
 
     common::page_idx_t addNewPage();
     common::page_idx_t addNewPages(common::page_idx_t numPages);
 
     inline void readPage(uint8_t* frame, common::page_idx_t pageIdx) const {
         KU_ASSERT(pageIdx < numPages);
@@ -56,16 +61,18 @@
     inline uint64_t getPageSize() const {
         return isLargePaged() ? common::BufferPoolConstants::PAGE_256KB_SIZE :
                                 common::BufferPoolConstants::PAGE_4KB_SIZE;
     }
 
 protected:
     virtual common::page_idx_t addNewPageWithoutLock();
-    void constructExistingFileHandle(const std::string& path, common::VirtualFileSystem* vfs);
-    void constructNewFileHandle(const std::string& path);
+    void constructExistingFileHandle(const std::string& path, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
+    void constructNewFileHandle(const std::string& path, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
 
 protected:
     uint8_t flags;
     std::unique_ptr<common::FileInfo> fileInfo;
     // Actually allocated/used number of pages in the file.
     uint32_t numPages;
     // This is the maximum number of pages the filehandle can currently support.
```

### sdist/kuzu-source/src/include/storage/index/hash_index.h

```diff
@@ -231,15 +231,15 @@
 inline bool HashIndex<common::ku_string_t>::equals(transaction::TransactionType trxType,
     std::string_view keyToLookup, const common::ku_string_t& keyInEntry) const;
 
 class PrimaryKeyIndex {
 public:
     PrimaryKeyIndex(const DBFileIDAndName& dbFileIDAndName, bool readOnly,
         common::PhysicalTypeID keyDataType, BufferManager& bufferManager, WAL* wal,
-        common::VirtualFileSystem* vfs);
+        common::VirtualFileSystem* vfs, main::ClientContext* context);
 
     void initHashIndices();
 
     ~PrimaryKeyIndex();
 
     template<typename T>
     using HashIndexType =
@@ -310,18 +310,18 @@
     void checkpointInMemory();
     void rollbackInMemory();
     void prepareCommit();
     void prepareRollback();
     BMFileHandle* getFileHandle() { return fileHandle.get(); }
     OverflowFile* getOverflowFile() { return overflowFile.get(); }
 
-    inline common::PhysicalTypeID keyTypeID() { return keyDataTypeID; }
+    common::PhysicalTypeID keyTypeID() { return keyDataTypeID; }
 
     static void createEmptyHashIndexFiles(common::PhysicalTypeID typeID, const std::string& fName,
-        common::VirtualFileSystem* vfs);
+        common::VirtualFileSystem* vfs, main::ClientContext* context);
 
 private:
     // When doing batch inserts, prepareCommit needs to be run before the COPY TABLE record is
     // logged to the WAL file, since the index is reloaded when that record is replayed. However
     // prepareCommit will also be run later, and the local storage can't cleared from the
     // HashIndices until checkpointing is done, and entries will get added twice if
     // HashIndex::prepareCommit is run twice. It seems simplest to just track whether or not
```

### sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h

```diff
@@ -10,15 +10,16 @@
 
 // Manages the disk image of the maxNodeOffsets and deleted node IDs (per node table).
 // Note: This class is *not* thread-safe.
 class NodesStoreStatsAndDeletedIDs : public TablesStatistics {
 public:
     // Should be used when an already loaded database is started from a directory.
     NodesStoreStatsAndDeletedIDs(const std::string& databasePath, BMFileHandle* metadataFH,
-        BufferManager* bufferManager, WAL* wal, common::VirtualFileSystem* fs);
+        BufferManager* bufferManager, WAL* wal, common::VirtualFileSystem* fs,
+        main::ClientContext* context);
 
     NodeTableStatsAndDeletedIDs* getNodeStatisticsAndDeletedIDs(
         transaction::Transaction* transaction, common::table_id_t tableID) const {
         return getNodeTableStats(transaction->getType(), tableID);
     }
 
     void updateNumTuplesByValue(common::table_id_t tableID, int64_t value) override;
```

### sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h

```diff
@@ -8,15 +8,16 @@
 namespace storage {
 
 // Manages the disk image of the numRels and numRelsPerDirectionBoundTable.
 class RelsStoreStats : public TablesStatistics {
 public:
     // Should be used when an already loaded database is started from a directory.
     RelsStoreStats(const std::string& databasePath, BMFileHandle* metadataFH,
-        BufferManager* bufferManager, WAL* wal, common::VirtualFileSystem* vfs);
+        BufferManager* bufferManager, WAL* wal, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
 
     RelTableStats* getRelStatistics(common::table_id_t tableID,
         transaction::Transaction* transaction) const {
         auto& tableStatisticPerTable =
             transaction->getType() == transaction::TransactionType::READ_ONLY ?
                 readOnlyVersion->tableStatisticPerTable :
                 readWriteVersion->tableStatisticPerTable;
```

### sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h

```diff
@@ -95,15 +95,15 @@
 
     const TablesStatisticsContent* getVersion(transaction::TransactionType type) const {
         return type == transaction::TransactionType::READ_ONLY ? readOnlyVersion.get() :
                                                                  readWriteVersion.get();
     }
 
     void readFromFile(const std::string& dbPath, common::FileVersionType dbFileType,
-        common::VirtualFileSystem* fs);
+        common::VirtualFileSystem* fs, main::ClientContext* context);
 
     void initTableStatisticsForWriteTrxNoLock();
 
     void resetToNotUpdated() { isUpdated = false; }
 
 protected:
     BMFileHandle* metadataFH;
```

### sdist/kuzu-source/src/include/storage/storage_manager.h

```diff
@@ -13,23 +13,24 @@
 } // namespace main
 
 namespace storage {
 
 class StorageManager {
 public:
     StorageManager(const std::string& databasePath, bool readOnly, const catalog::Catalog& catalog,
-        MemoryManager& memoryManager, bool enableCompression, common::VirtualFileSystem* vfs);
+        MemoryManager& memoryManager, bool enableCompression, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
 
     static void recover(main::ClientContext& clientContext);
 
     void createTable(common::table_id_t tableID, catalog::Catalog* catalog,
-        transaction::Transaction* transaction);
-    void dropTable(common::table_id_t tableID);
+        main::ClientContext* context);
+    void dropTable(common::table_id_t tableID, common::VirtualFileSystem* vfs);
 
-    void prepareCommit(transaction::Transaction* transaction);
+    void prepareCommit(transaction::Transaction* transaction, common::VirtualFileSystem* vfs);
     void prepareRollback();
     void checkpointInMemory();
     void rollbackInMemory();
 
     PrimaryKeyIndex* getPKIndex(common::table_id_t tableID);
 
     Table* getTable(common::table_id_t tableID) const {
@@ -49,34 +50,36 @@
     }
     RelsStoreStats* getRelsStatistics() { return relsStatistics.get(); }
     std::string getDatabasePath() const { return databasePath; }
     bool isReadOnly() const { return readOnly; }
     bool compressionEnabled() const { return enableCompression; }
 
 private:
-    std::unique_ptr<BMFileHandle> initFileHandle(const std::string& filename);
+    std::unique_ptr<BMFileHandle> initFileHandle(const std::string& filename,
+        common::VirtualFileSystem* vfs, main::ClientContext* context);
 
-    void loadTables(const catalog::Catalog& catalog);
-    void createNodeTable(common::table_id_t tableID, catalog::NodeTableCatalogEntry* tableSchema);
+    void loadTables(const catalog::Catalog& catalog, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
+    void createNodeTable(common::table_id_t tableID, catalog::NodeTableCatalogEntry* tableSchema,
+        main::ClientContext* context);
     void createRelTable(common::table_id_t tableID, catalog::RelTableCatalogEntry* tableSchema,
         catalog::Catalog* catalog, transaction::Transaction* transaction);
     void createRelTableGroup(common::table_id_t tableID, catalog::RelGroupCatalogEntry* tableSchema,
         catalog::Catalog* catalog, transaction::Transaction* transaction);
     void createRdfGraph(common::table_id_t tableID, catalog::RDFGraphCatalogEntry* tableSchema,
-        catalog::Catalog* catalog, transaction::Transaction* transaction);
+        catalog::Catalog* catalog, main::ClientContext* context);
 
 private:
     std::string databasePath;
     bool readOnly;
     std::unique_ptr<BMFileHandle> dataFH;
     std::unique_ptr<BMFileHandle> metadataFH;
     std::unique_ptr<NodesStoreStatsAndDeletedIDs> nodesStatisticsAndDeletedIDs;
     std::unique_ptr<RelsStoreStats> relsStatistics;
     std::unordered_map<common::table_id_t, std::unique_ptr<Table>> tables;
     MemoryManager& memoryManager;
     std::unique_ptr<WAL> wal;
     bool enableCompression;
-    common::VirtualFileSystem* vfs;
 };
 
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h

```diff
@@ -84,18 +84,19 @@
 
 class OverflowFile {
     friend class OverflowFileHandle;
 
 public:
     // For reading an existing overflow file
     OverflowFile(const DBFileIDAndName& dbFileIdAndName, BufferManager* bufferManager, WAL* wal,
-        bool readOnly, common::VirtualFileSystem* vfs);
+        bool readOnly, common::VirtualFileSystem* vfs, main::ClientContext* context);
 
     // For creating an overflow file from scratch
-    static void createEmptyFiles(const std::string& fName, common::VirtualFileSystem* vfs);
+    static void createEmptyFiles(const std::string& fName, common::VirtualFileSystem* vfs,
+        main::ClientContext* context);
 
     // Handles contain a reference to the overflow file
     OverflowFile(OverflowFile&& other) = delete;
 
     void rollbackInMemory();
     void prepareCommit();
     void checkpointInMemory();
```

### sdist/kuzu-source/src/include/storage/store/column.h

```diff
@@ -75,15 +75,15 @@
         common::ValueVector* resultVector, uint64_t offsetInVector);
     // Scan from [startOffsetInGroup, endOffsetInGroup).
     virtual void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET);
 
     // Append column chunk in a new node group.
-    virtual void append(ColumnChunk* columnChunk, common::node_group_idx_t nodeGroupIdx);
+    virtual void append(ColumnChunk* columnChunk, ChunkState& state);
 
     common::LogicalType& getDataType() { return dataType; }
     const common::LogicalType& getDataType() const { return dataType; }
     uint32_t getNumBytesPerValue() const { return numBytesPerFixedSizedValue; }
     uint64_t getNumNodeGroups(transaction::Transaction* transaction) const {
         return metadataDA->getNumElements(transaction->getType());
     }
@@ -195,26 +195,24 @@
         common::offset_t srcOffset);
 
     virtual void commitLocalChunkInPlace(ChunkState& state,
         const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
         const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
         const offset_set_t& deleteInfo);
     virtual void commitLocalChunkOutOfPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, bool isNewNodeGroup,
-        const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
-        const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
-        const offset_set_t& deleteInfo);
+        ChunkState& state, bool isNewNodeGroup, const ChunkCollection& localInsertChunks,
+        const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
+        const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo);
 
     virtual void commitColumnChunkInPlace(ChunkState& state,
         const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
         common::offset_t srcOffset);
     virtual void commitColumnChunkOutOfPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, bool isNewNodeGroup,
-        const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
-        common::offset_t srcOffset);
+        ChunkState& state, bool isNewNodeGroup, const std::vector<common::offset_t>& dstOffsets,
+        ColumnChunk* chunk, common::offset_t srcOffset);
 
     void applyLocalChunkToColumn(ChunkState& state, const ChunkCollection& localChunks,
         const offset_to_row_idx_t& info);
 
     // check if val is in range [start, end)
     static bool isInRange(uint64_t val, uint64_t start, uint64_t end) {
         return val >= start && val < end;
```

### sdist/kuzu-source/src/include/storage/store/dictionary_column.h

```diff
@@ -14,15 +14,15 @@
     DictionaryColumn(const std::string& name, const MetadataDAHInfo& metaDAHeaderInfo,
         BMFileHandle* dataFH, BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal,
         transaction::Transaction* transaction, RWPropertyStats stats, bool enableCompression);
 
     void initChunkState(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, Column::ChunkState& columnReadState);
 
-    void append(common::node_group_idx_t nodeGroupIdx, const DictionaryChunk& dictChunk);
+    void append(Column::ChunkState& state, const DictionaryChunk& dictChunk);
 
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         DictionaryChunk& dictChunk);
     // Offsets to scan should be a sorted list of pairs mapping the index of the entry in the string
     // dictionary (as read from the index column) to the output index in the result vector to store
     // the string.
     void scan(transaction::Transaction* transaction, const Column::ChunkState& offsetState,
```

### sdist/kuzu-source/src/include/storage/store/list_column.h

```diff
@@ -69,15 +69,15 @@
     void scanInternal(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override;
 
     void lookupValue(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t nodeOffset, common::ValueVector* resultVector,
         uint32_t posInVector) override;
 
-    void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override;
+    void append(ColumnChunk* columnChunk, ChunkState& state) override;
 
 private:
     void scanUnfiltered(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* resultVector, const ListOffsetSizeInfo& listOffsetInfoInStorage);
     void scanFiltered(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* offsetVector, const ListOffsetSizeInfo& listOffsetInfoInStorage);
 
@@ -102,15 +102,15 @@
         const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
         common::offset_t startSrcOffset) override;
 
     void prepareCommitForOffsetChunk(transaction::Transaction* transaction, ChunkState& offsetState,
         const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
         common::offset_t startSrcOffset);
     void commitOffsetColumnChunkOutOfPlace(transaction::Transaction* transaction,
-        const ChunkState& offsetState, const std::vector<common::offset_t>& dstOffsets,
+        ChunkState& offsetState, const std::vector<common::offset_t>& dstOffsets,
         ColumnChunk* chunk, common::offset_t startSrcOffset);
 
 private:
     std::unique_ptr<Column> sizeColumn;
     std::unique_ptr<Column> dataColumn;
 };
```

### sdist/kuzu-source/src/include/storage/store/node_table.h

```diff
@@ -57,19 +57,19 @@
         : nodeIDVector{nodeIDVector}, pkVector{pkVector} {}
 };
 
 class StorageManager;
 class NodeTable final : public Table {
 public:
     NodeTable(StorageManager* storageManager, catalog::NodeTableCatalogEntry* nodeTableEntry,
-        MemoryManager* memoryManager, common::VirtualFileSystem* vfs);
+        MemoryManager* memoryManager, common::VirtualFileSystem* vfs, main::ClientContext* context);
 
     void initializePKIndex(const std::string& databasePath,
         catalog::NodeTableCatalogEntry* nodeTableEntry, bool readOnly,
-        common::VirtualFileSystem* vfs);
+        common::VirtualFileSystem* vfs, main::ClientContext* context);
 
     common::offset_t getMaxNodeOffset(transaction::Transaction* transaction) const {
         auto nodesStats = common::ku_dynamic_cast<TablesStatistics*, NodesStoreStatsAndDeletedIDs*>(
             tablesStatistics);
         return nodesStats->getMaxNodeOffset(transaction, tableID);
     }
     void setSelVectorForDeletedOffsets(transaction::Transaction* trx,
@@ -105,15 +105,17 @@
     NodesStoreStatsAndDeletedIDs* getNodeStatisticsAndDeletedIDs() const {
         return common::ku_dynamic_cast<TablesStatistics*, NodesStoreStatsAndDeletedIDs*>(
             tablesStatistics);
     }
     common::column_id_t getNumColumns() const { return tableData->getNumColumns(); }
     Column* getColumn(common::column_id_t columnID) { return tableData->getColumn(columnID); }
 
-    void append(ChunkedNodeGroup* nodeGroup) { tableData->append(nodeGroup); }
+    void append(transaction::Transaction* transaction, ChunkedNodeGroup* nodeGroup) {
+        tableData->append(transaction, nodeGroup);
+    }
 
     void prepareCommitNodeGroup(common::node_group_idx_t nodeGroupIdx,
         transaction::Transaction* transaction, storage::LocalNodeNG* localNodeGroup);
     void prepareCommit(transaction::Transaction* transaction, LocalTable* localTable) override;
     void prepareCommit() override;
     void prepareRollback(LocalTable* localTable) override;
     void checkpointInMemory() override;
```

### sdist/kuzu-source/src/include/storage/store/node_table_data.h

```diff
@@ -33,15 +33,15 @@
         std::vector<common::column_id_t> columnIDs, const common::ValueVector& inNodeIDVector,
         TableDataReadState& readState);
     void read(transaction::Transaction* transaction, TableDataReadState& readState,
         const common::ValueVector& nodeIDVector,
         const std::vector<common::ValueVector*>& outputVectors);
 
     // Flush the nodeGroup to disk and update metadataDAs.
-    void append(ChunkedNodeGroup* nodeGroup) override;
+    void append(transaction::Transaction* transaction, ChunkedNodeGroup* nodeGroup) override;
 
     void prepareLocalNodeGroupToCommit(common::node_group_idx_t nodeGroupIdx,
         transaction::Transaction* transaction, LocalNodeNG* localNodeGroup);
     void prepareLocalTableToCommit(transaction::Transaction* transaction,
         LocalTableData* localTable) override;
 
     common::node_group_idx_t getNumNodeGroups(
```

### sdist/kuzu-source/src/include/storage/store/null_column.h

```diff
@@ -28,15 +28,15 @@
     void scan(transaction::Transaction* transaction, node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
 
     void lookup(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
         ValueVector* resultVector) override;
 
-    void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override;
+    void append(ColumnChunk* columnChunk, ChunkState& state) override;
 
     bool isNull(Transaction* transaction, const ChunkState& state, offset_t offsetInChunk);
     void setNull(ChunkState& state, offset_t offsetInChunk, uint64_t value = true);
 
     void write(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
         uint32_t posInVectorToWriteFrom) override;
     void write(ChunkState& state, common::offset_t offsetInChunk, ColumnChunk* data,
```

### sdist/kuzu-source/src/include/storage/store/rel_table.h

```diff
@@ -111,17 +111,19 @@
     }
     const std::vector<std::unique_ptr<Column>>& getColumns(
         common::RelDataDirection direction) const {
         return direction == common::RelDataDirection::FWD ? fwdRelTableData->getColumns() :
                                                             bwdRelTableData->getColumns();
     }
 
-    void append(ChunkedNodeGroup* nodeGroup, common::RelDataDirection direction) {
-        direction == common::RelDataDirection::FWD ? fwdRelTableData->append(nodeGroup) :
-                                                     bwdRelTableData->append(nodeGroup);
+    void append(transaction::Transaction* transaction, ChunkedNodeGroup* nodeGroup,
+        common::RelDataDirection direction) {
+        direction == common::RelDataDirection::FWD ?
+            fwdRelTableData->append(transaction, nodeGroup) :
+            bwdRelTableData->append(transaction, nodeGroup);
     }
 
     bool isNewNodeGroup(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, common::RelDataDirection direction) {
         return direction == common::RelDataDirection::FWD ?
                    fwdRelTableData->isNewNodeGroup(transaction, nodeGroupIdx) :
                    bwdRelTableData->isNewNodeGroup(transaction, nodeGroupIdx);
```

### sdist/kuzu-source/src/include/storage/store/rel_table_data.h

```diff
@@ -48,18 +48,18 @@
     std::unique_ptr<Column> length;
 
     inline void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ChunkedCSRHeader& chunks) const {
         offset->scan(transaction, nodeGroupIdx, chunks.offset.get());
         length->scan(transaction, nodeGroupIdx, chunks.length.get());
     }
-    inline void append(const ChunkedCSRHeader& headerChunks,
-        common::node_group_idx_t nodeGroupIdx) const {
-        offset->append(headerChunks.offset.get(), nodeGroupIdx);
-        length->append(headerChunks.length.get(), nodeGroupIdx);
+    inline void append(const ChunkedCSRHeader& headerChunks, Column::ChunkState& offsetState,
+        Column::ChunkState& lengthState) const {
+        offset->append(headerChunks.offset.get(), offsetState);
+        length->append(headerChunks.length.get(), lengthState);
     }
 
     common::offset_t getNumNodes(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx) const;
 };
 
 // TODO(Guodong): Serialize the info to disk. This should be a config per node group.
@@ -151,15 +151,15 @@
     bool delete_(transaction::Transaction* transaction, common::ValueVector* srcNodeIDVector,
         common::ValueVector* relIDVector);
 
     void checkRelMultiplicityConstraint(transaction::Transaction* transaction,
         common::ValueVector* srcNodeIDVector) const;
     bool checkIfNodeHasRels(transaction::Transaction* transaction,
         common::offset_t nodeOffset) const;
-    void append(ChunkedNodeGroup* nodeGroup) override;
+    void append(transaction::Transaction* transaction, ChunkedNodeGroup* nodeGroup) override;
 
     inline Column* getNbrIDColumn() const { return columns[NBR_ID_COLUMN_ID].get(); }
     inline Column* getCSROffsetColumn() const { return csrHeaderColumns.offset.get(); }
     inline Column* getCSRLengthColumn() const { return csrHeaderColumns.length.get(); }
 
     bool isNewNodeGroup(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx) const;
```

### sdist/kuzu-source/src/include/storage/store/string_column.h

```diff
@@ -18,15 +18,15 @@
     void scan(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector = 0) override;
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
 
-    void append(ColumnChunk* columnChunk, common::node_group_idx_t nodeGroupIdx) override;
+    void append(ColumnChunk* columnChunk, ChunkState& state) override;
 
     void writeValue(ChunkState& state, common::offset_t offsetInChunk,
         common::ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) override;
 
     void write(ChunkState& state, common::offset_t offsetInChunk, ColumnChunk* data,
         common::offset_t dataOffset, common::length_t numValues) override;
```

### sdist/kuzu-source/src/include/storage/store/struct_column.h

```diff
@@ -17,15 +17,15 @@
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
     void scan(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector) override;
 
-    void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override;
+    void append(ColumnChunk* columnChunk, ChunkState& state) override;
 
     void checkpointInMemory() override;
     void rollbackInMemory() override;
     void prepareCommit() override;
 
     inline Column* getChild(common::vector_idx_t childIdx) {
         KU_ASSERT(childIdx < childColumns.size());
```

### sdist/kuzu-source/src/include/storage/store/table_data.h

```diff
@@ -27,15 +27,15 @@
     virtual void scan(transaction::Transaction* transaction, TableDataReadState& readState,
         const common::ValueVector& nodeIDVector,
         const std::vector<common::ValueVector*>& outputVectors) = 0;
     virtual void lookup(transaction::Transaction* transaction, TableDataReadState& readState,
         const common::ValueVector& nodeIDVector,
         const std::vector<common::ValueVector*>& outputVectors) = 0;
 
-    virtual void append(ChunkedNodeGroup* nodeGroup) = 0;
+    virtual void append(transaction::Transaction* transaction, ChunkedNodeGroup* nodeGroup) = 0;
 
     inline void dropColumn(common::column_id_t columnID) {
         columns.erase(columns.begin() + columnID);
     }
     void addColumn(transaction::Transaction* transaction, const std::string& colNamePrefix,
         DiskArray<ColumnChunkMetadata>* metadataDA, const MetadataDAHInfo& metadataDahInfo,
         const catalog::Property& property, common::ValueVector* defaultValueVector,
```

### sdist/kuzu-source/src/include/storage/wal/wal.h

```diff
@@ -21,15 +21,15 @@
 
 class WALReplayer;
 class WAL {
     friend class WALReplayer;
 
 public:
     WAL(const std::string& directory, bool readOnly, BufferManager& bufferManager,
-        common::VirtualFileSystem* vfs);
+        common::VirtualFileSystem* vfs, main::ClientContext* context);
 
     // Destructing WAL flushes any unwritten header page but not the other pages. The caller
     // which possibly has access to the buffer manager needs to ensure any unwritten pages
     // are also flushed to disk.
     ~WAL();
 
     common::page_idx_t logPageUpdateRecord(DBFileID dbFileID,
```

### sdist/kuzu-source/src/include/storage/wal_replayer_utils.h

```diff
@@ -19,12 +19,12 @@
 class WALReplayerUtils {
 public:
     static void removeHashIndexFile(common::VirtualFileSystem* vfs, common::table_id_t tableID,
         const std::string& directory);
 
     // Create empty hash index file for the new node table.
     static void createEmptyHashIndexFiles(catalog::NodeTableCatalogEntry* nodeTableEntry,
-        const std::string& directory, common::VirtualFileSystem* vfs);
+        const std::string& directory, common::VirtualFileSystem* vfs, main::ClientContext* context);
 };
 
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/main/attached_database.cpp

```diff
@@ -1,41 +1,56 @@
 #include "main/attached_database.h"
 
+#include "common/types/types.h"
 #include "main/db_config.h"
 #include "storage/storage_manager.h"
+#include "storage/storage_utils.h"
 #include "transaction/transaction_manager.h"
 
 namespace kuzu {
 namespace main {
 
 void AttachedDatabase::invalidateCache() {
     if (dbType != common::ATTACHED_KUZU_DB_TYPE) {
         auto catalogExtension = catalog->ptrCast<extension::CatalogExtension>();
         catalogExtension->invalidateCache();
     }
 }
 
-AttachedKuzuDatabase::AttachedKuzuDatabase(std::string dbPath, std::string dbName,
-    std::string dbType, ClientContext* clientContext)
-    : AttachedDatabase{std::move(dbName), std::move(dbType), nullptr /* catalog */} {
-    auto vfs = clientContext->getVFSUnsafe();
-    auto path = vfs->expandPath(clientContext, dbPath);
-    if (!vfs->fileOrPathExists(path, clientContext)) {
+void AttachedKuzuDatabase::initCatalog(const std::string& path, ClientContext* context) {
+    auto vfs = context->getVFSUnsafe();
+    auto catalogFilePath =
+        storage::StorageUtils::getCatalogFilePath(vfs, path, common::FileVersionType::ORIGINAL);
+    if (!vfs->fileOrPathExists(catalogFilePath, context)) {
         throw common::RuntimeException(common::stringFormat(
-            "Cannot attach a remote kuzu database due to invalid path: {}.", dbPath));
+            "Cannot attach a remote kuzu database due to invalid path: {}.", path));
     }
-    auto walFile = vfs->openFile(path + "/" + common::StorageConstants::WAL_FILE_SUFFIX, O_RDONLY,
-        clientContext);
+    catalog = std::make_unique<catalog::Catalog>();
+    catalog->readFromFile(path, vfs, common::FileVersionType::ORIGINAL, context);
+    catalog->registerBuiltInFunctions();
+}
+
+static void validateEmptyWAL(const std::string& path, ClientContext* context) {
+    auto walFile = context->getVFSUnsafe()->openFile(
+        path + "/" + common::StorageConstants::WAL_FILE_SUFFIX, O_RDONLY, context);
     if (walFile->getFileSize() > 0) {
         throw common::RuntimeException(
             common::stringFormat("Cannot attach a remote kuzu database with non-empty wal file."));
     }
-    catalog = std::make_unique<catalog::Catalog>(path, vfs);
+}
+
+AttachedKuzuDatabase::AttachedKuzuDatabase(std::string dbPath, std::string dbName,
+    std::string dbType, ClientContext* clientContext)
+    : AttachedDatabase{std::move(dbName), std::move(dbType), nullptr /* catalog */} {
+    auto vfs = clientContext->getVFSUnsafe();
+    auto path = vfs->expandPath(clientContext, dbPath);
+    initCatalog(path, clientContext);
+    validateEmptyWAL(path, clientContext);
     storageManager = std::make_unique<storage::StorageManager>(path, true /* isReadOnly */,
         *catalog, *clientContext->getMemoryManager(),
-        clientContext->getDBConfig()->enableCompression, vfs);
+        clientContext->getDBConfig()->enableCompression, vfs, clientContext);
     transactionManager =
         std::make_unique<transaction::TransactionManager>(storageManager->getWAL());
 }
 
 } // namespace main
 } // namespace kuzu
```

### sdist/kuzu-source/src/main/database.cpp

```diff
@@ -65,29 +65,29 @@
         flags |= O_CREAT;
     }
     lock = readOnly ? FileLockType::READ_LOCK : FileLockType::WRITE_LOCK;
 }
 
 Database::Database(std::string_view databasePath, SystemConfig systemConfig)
     : dbConfig{systemConfig} {
-    vfs = std::make_unique<VirtualFileSystem>(this);
+    vfs = std::make_unique<VirtualFileSystem>();
     // To expand a path with home directory(~), we have to pass in a dummy clientContext which
     // handles the home directory expansion.
     auto clientContext = ClientContext(this);
     auto dbPathStr = std::string(databasePath);
     this->databasePath = vfs->expandPath(&clientContext, dbPathStr);
     bufferManager =
         std::make_unique<BufferManager>(this->dbConfig.bufferPoolSize, this->dbConfig.maxDBSize);
-    memoryManager = std::make_unique<MemoryManager>(bufferManager.get(), vfs.get());
+    memoryManager = std::make_unique<MemoryManager>(bufferManager.get(), vfs.get(), nullptr);
     queryProcessor = std::make_unique<processor::QueryProcessor>(this->dbConfig.maxNumThreads);
     initAndLockDBDir();
     catalog = std::make_unique<Catalog>(this->databasePath, vfs.get());
     StorageManager::recover(clientContext);
     storageManager = std::make_unique<StorageManager>(this->databasePath, systemConfig.readOnly,
-        *catalog, *memoryManager, systemConfig.enableCompression, vfs.get());
+        *catalog, *memoryManager, systemConfig.enableCompression, vfs.get(), nullptr);
     transactionManager = std::make_unique<TransactionManager>(storageManager->getWAL());
     extensionOptions = std::make_unique<extension::ExtensionOptions>();
     databaseManager = std::make_unique<DatabaseManager>();
 }
 
 Database::~Database() {
     bufferManager->clearEvictionQueue();
```

### sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp

```diff
@@ -9,15 +9,15 @@
 namespace kuzu {
 namespace processor {
 
 void CreateTable::executeDDLInternal(ExecutionContext* context) {
     auto catalog = context->clientContext->getCatalog();
     auto newTableID = catalog->createTableSchema(context->clientContext->getTx(), info);
     auto storageManager = context->clientContext->getStorageManager();
-    storageManager->createTable(newTableID, catalog, context->clientContext->getTx());
+    storageManager->createTable(newTableID, catalog, context->clientContext);
 }
 
 std::string CreateTable::getOutputMsg() {
     return stringFormat("Table {} has been created.", info.tableName);
 }
 
 } // namespace processor
```

### sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp

```diff
@@ -33,28 +33,28 @@
         KU_ASSERT(distinctSharedState);
         numRows = distinctSharedState->getFactorizedTable()->getNumTuples();
     }
     pkIndex->bulkReserve(numRows);
     globalIndexBuilder = IndexBuilder(std::make_shared<IndexBuilderSharedState>(pkIndex));
 }
 
-void NodeBatchInsert::appendIncompleteNodeGroup(std::unique_ptr<ChunkedNodeGroup> localNodeGroup,
-    std::optional<IndexBuilder>& indexBuilder, ExecutionContext* context) {
+void NodeBatchInsert::appendIncompleteNodeGroup(transaction::Transaction* transaction,
+    std::unique_ptr<ChunkedNodeGroup> localNodeGroup, std::optional<IndexBuilder>& indexBuilder) {
     std::unique_lock xLck{sharedState->mtx};
     auto nodeSharedState =
         ku_dynamic_cast<BatchInsertSharedState*, NodeBatchInsertSharedState*>(sharedState.get());
     if (!nodeSharedState->sharedNodeGroup) {
         nodeSharedState->sharedNodeGroup = std::move(localNodeGroup);
         return;
     }
     auto numNodesAppended =
         nodeSharedState->sharedNodeGroup->append(localNodeGroup.get(), 0 /* offsetInNodeGroup */);
     if (nodeSharedState->sharedNodeGroup->isFull()) {
         node_group_idx_t nodeGroupIdx = nodeSharedState->getNextNodeGroupIdxWithoutLock();
-        writeAndResetNodeGroup(nodeGroupIdx, context, nodeSharedState->sharedNodeGroup,
+        writeAndResetNodeGroup(transaction, nodeGroupIdx, nodeSharedState->sharedNodeGroup,
             indexBuilder);
     }
     if (numNodesAppended < localNodeGroup->getNumRows()) {
         nodeSharedState->sharedNodeGroup->append(localNodeGroup.get(), numNodesAppended);
     }
 }
 
@@ -122,38 +122,38 @@
         ku_dynamic_cast<BatchInsertLocalState*, NodeBatchInsertLocalState*>(localState.get());
     if (nodeLocalState->localIndexBuilder) {
         token = nodeLocalState->localIndexBuilder->getProducerToken();
     }
 
     while (children[0]->getNextTuple(context)) {
         auto originalSelVector = nodeLocalState->columnState->getSelVectorShared();
-        copyToNodeGroup(context);
+        copyToNodeGroup(context->clientContext->getTx());
         nodeLocalState->columnState->setSelVector(originalSelVector);
     }
     if (nodeLocalState->nodeGroup->getNumRows() > 0) {
-        appendIncompleteNodeGroup(std::move(nodeLocalState->nodeGroup),
-            nodeLocalState->localIndexBuilder, context);
+        appendIncompleteNodeGroup(context->clientContext->getTx(),
+            std::move(nodeLocalState->nodeGroup), nodeLocalState->localIndexBuilder);
     }
     if (nodeLocalState->localIndexBuilder) {
         KU_ASSERT(token);
         token->quit();
         nodeLocalState->localIndexBuilder->finishedProducing();
     }
 }
 
-void NodeBatchInsert::writeAndResetNewNodeGroup(node_group_idx_t nodeGroupIdx,
-    std::optional<IndexBuilder>& indexBuilder, column_id_t pkColumnID, NodeTable* table,
-    ChunkedNodeGroup* nodeGroup) {
+void NodeBatchInsert::writeAndResetNewNodeGroup(transaction::Transaction* transaction,
+    node_group_idx_t nodeGroupIdx, std::optional<IndexBuilder>& indexBuilder,
+    column_id_t pkColumnID, NodeTable* table, ChunkedNodeGroup* nodeGroup) {
     nodeGroup->finalize(nodeGroupIdx);
     if (indexBuilder) {
         auto nodeOffset = StorageUtils::getStartOffsetOfNodeGroup(nodeGroupIdx);
         indexBuilder->insert(nodeGroup->getColumnChunkUnsafe(pkColumnID), nodeOffset,
             nodeGroup->getNumRows());
     }
-    table->append(nodeGroup);
+    table->append(transaction, nodeGroup);
     nodeGroup->resetToEmpty();
 }
 
 common::offset_t NodeBatchInsert::writeToExistingNodeGroup(transaction::Transaction* transaction,
     node_group_idx_t nodeGroupIdx, std::optional<IndexBuilder>& indexBuilder,
     column_id_t pkColumnID, NodeTable* table, ChunkedNodeGroup* nodeGroup) {
     auto numExistingTuplesInChunk = table->getNumTuplesInNodeGroup(transaction, nodeGroupIdx);
@@ -181,63 +181,64 @@
     auto oldNodeGroup = std::move(nodeGroup);
     auto nodeInfo = ku_dynamic_cast<BatchInsertInfo*, NodeBatchInsertInfo*>(info.get());
     nodeGroup = NodeGroupFactory::createNodeGroup(ColumnDataFormat::REGULAR, nodeInfo->columnTypes,
         info->compressionEnabled);
     nodeGroup->append(oldNodeGroup.get(), startIndexInGroup);
 }
 
-void NodeBatchInsert::copyToNodeGroup(ExecutionContext* context) {
+void NodeBatchInsert::copyToNodeGroup(transaction::Transaction* transaction) {
     auto numAppendedTuples = 0ul;
     auto nodeLocalState =
         ku_dynamic_cast<BatchInsertLocalState*, NodeBatchInsertLocalState*>(localState.get());
     auto numTuplesToAppend = nodeLocalState->columnState->getSelVector().getSelSize();
     auto nodeSharedState =
         ku_dynamic_cast<BatchInsertSharedState*, NodeBatchInsertSharedState*>(sharedState.get());
     while (numAppendedTuples < numTuplesToAppend) {
         auto numAppendedTuplesInNodeGroup = nodeLocalState->nodeGroup->append(
             nodeLocalState->columnVectors, nodeLocalState->columnState->getSelVectorUnsafe(),
             numTuplesToAppend - numAppendedTuples);
         numAppendedTuples += numAppendedTuplesInNodeGroup;
         if (nodeLocalState->nodeGroup->isFull()) {
-            writeAndResetNodeGroup(nodeSharedState->getNextNodeGroupIdx(), context,
+            writeAndResetNodeGroup(transaction, nodeSharedState->getNextNodeGroupIdx(),
                 nodeLocalState->nodeGroup, nodeLocalState->localIndexBuilder);
         }
         if (numAppendedTuples < numTuplesToAppend) {
             nodeLocalState->columnState->slice((offset_t)numAppendedTuplesInNodeGroup);
         }
     }
     sharedState->incrementNumRows(numAppendedTuples);
 }
 
-void NodeBatchInsert::writeAndResetNodeGroup(node_group_idx_t nodeGroupIdx,
-    ExecutionContext* context, std::unique_ptr<storage::ChunkedNodeGroup>& nodeGroup,
+void NodeBatchInsert::writeAndResetNodeGroup(transaction::Transaction* transaction,
+    node_group_idx_t nodeGroupIdx, std::unique_ptr<storage::ChunkedNodeGroup>& nodeGroup,
     std::optional<IndexBuilder>& indexBuilder) {
     auto nodeSharedState =
         ku_dynamic_cast<BatchInsertSharedState*, NodeBatchInsertSharedState*>(sharedState.get());
     auto nodeTable = ku_dynamic_cast<Table*, NodeTable*>(sharedState->table);
 
-    if (nodeGroupIdx >= nodeTable->getNumNodeGroups(context->clientContext->getTx())) {
-        writeAndResetNewNodeGroup(nodeGroupIdx, indexBuilder, nodeSharedState->pkColumnIdx,
-            nodeTable, nodeGroup.get());
+    if (nodeGroupIdx >= nodeTable->getNumNodeGroups(transaction)) {
+        writeAndResetNewNodeGroup(transaction, nodeGroupIdx, indexBuilder,
+            nodeSharedState->pkColumnIdx, nodeTable, nodeGroup.get());
     } else {
-        KU_ASSERT(nodeGroupIdx == nodeTable->getNumNodeGroups(context->clientContext->getTx()) - 1);
-        auto valuesWritten = writeToExistingNodeGroup(context->clientContext->getTx(), nodeGroupIdx,
-            indexBuilder, nodeSharedState->pkColumnIdx, nodeTable, nodeGroup.get());
+        KU_ASSERT(nodeGroupIdx == nodeTable->getNumNodeGroups(transaction) - 1);
+        auto valuesWritten = writeToExistingNodeGroup(transaction, nodeGroupIdx, indexBuilder,
+            nodeSharedState->pkColumnIdx, nodeTable, nodeGroup.get());
         clearToIndex(nodeGroup, valuesWritten);
     }
 }
 
 void NodeBatchInsert::finalize(ExecutionContext* context) {
     auto nodeSharedState =
         ku_dynamic_cast<BatchInsertSharedState*, NodeBatchInsertSharedState*>(sharedState.get());
     nodeSharedState->updateNumTuplesForTable();
     if (nodeSharedState->sharedNodeGroup) {
         while (nodeSharedState->sharedNodeGroup->getNumRows() > 0) {
-            writeAndResetNodeGroup(nodeSharedState->getNextNodeGroupIdx(), context,
-                nodeSharedState->sharedNodeGroup, nodeSharedState->globalIndexBuilder);
+            writeAndResetNodeGroup(context->clientContext->getTx(),
+                nodeSharedState->getNextNodeGroupIdx(), nodeSharedState->sharedNodeGroup,
+                nodeSharedState->globalIndexBuilder);
         }
     }
     if (nodeSharedState->globalIndexBuilder) {
         nodeSharedState->globalIndexBuilder->finalize(context);
     }
     sharedState->logBatchInsertWALRecord();
     auto outputMsg = stringFormat("{} tuples have been copied to the {} table.",
```

### sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp

```diff
@@ -36,17 +36,18 @@
             partitionerSharedState->getNextPartition(relInfo->partitioningIdx);
         if (relLocalState->nodeGroupIdx == INVALID_PARTITION_IDX) {
             // No more partitions left in the partitioning buffer.
             break;
         }
         if (relTable->isNewNodeGroup(context->clientContext->getTx(), relLocalState->nodeGroupIdx,
                 relInfo->direction)) {
-            appendNewNodeGroup(*relInfo, *relLocalState, *sharedState, *partitionerSharedState);
+            appendNewNodeGroup(context->clientContext->getTx(), *relInfo, *relLocalState,
+                *sharedState, *partitionerSharedState);
         } else {
-            mergeNodeGroup(context, *relInfo, *relLocalState, *sharedState,
+            mergeNodeGroup(context->clientContext->getTx(), *relInfo, *relLocalState, *sharedState,
                 *partitionerSharedState);
         }
     }
 }
 
 void RelBatchInsert::prepareCSRNodeGroup(const ChunkedNodeGroupCollection& partition,
     offset_t startNodeOffset, const RelBatchInsertInfo& relInfo,
@@ -72,17 +73,17 @@
     for (auto& chunkedGroup : partition.getChunkedGroups()) {
         auto& offsetChunk = chunkedGroup->getColumnChunkUnsafe(relInfo.offsetColumnID);
         setOffsetFromCSROffsets(offsetChunk, *csrHeader.offset);
     }
     populateEndCSROffsets(csrHeader, gaps);
 }
 
-void RelBatchInsert::mergeNodeGroup(ExecutionContext* context, const RelBatchInsertInfo& relInfo,
-    RelBatchInsertLocalState& localState, BatchInsertSharedState& sharedState,
-    const PartitionerSharedState& partitionerSharedState) {
+void RelBatchInsert::mergeNodeGroup(transaction::Transaction* transaction,
+    const RelBatchInsertInfo& relInfo, RelBatchInsertLocalState& localState,
+    BatchInsertSharedState& sharedState, const PartitionerSharedState& partitionerSharedState) {
     auto relTable = ku_dynamic_cast<Table*, RelTable*>(sharedState.table);
     auto nodeGroupStartOffset = StorageUtils::getStartOffsetOfNodeGroup(localState.nodeGroupIdx);
     auto localNG = std::make_unique<LocalRelNG>(nodeGroupStartOffset, relInfo.columnTypes);
     auto& partition =
         partitionerSharedState.getPartitionBuffer(relInfo.partitioningIdx, localState.nodeGroupIdx);
     auto& insertChunks = localNG->getInsertChunks();
     auto startNodeOffset = StorageUtils::getStartOffsetOfNodeGroup(localState.nodeGroupIdx);
@@ -99,16 +100,15 @@
             }
             chunksToAppend.push_back(std::move(chunkedGroup->getColumnChunksUnsafe()[i]));
         }
         auto chunkedGroupToAppend = std::make_unique<ChunkedNodeGroup>(std::move(chunksToAppend));
         insertChunks.appendChunkedGroup(&offsetChunk, std::move(chunkedGroupToAppend));
     }
     relTable->getDirectedTableData(relInfo.direction)
-        ->prepareCommitNodeGroup(context->clientContext->getTx(), localState.nodeGroupIdx,
-            localNG.get());
+        ->prepareCommitNodeGroup(transaction, localState.nodeGroupIdx, localNG.get());
     sharedState.incrementNumRows(numRels);
 }
 
 void RelBatchInsert::populateEndCSROffsets(ChunkedCSRHeader& csrHeader,
     std::vector<offset_t>& gaps) {
     auto csrOffsets = (offset_t*)csrHeader.offset->getData();
     for (auto i = 0u; i < csrHeader.offset->getNumValues(); i++) {
@@ -170,17 +170,17 @@
         auto nodeOffset = nodeOffsetChunk.getValue<offset_t>(i);
         auto csrOffset = csrOffsetChunk.getValue<offset_t>(nodeOffset);
         nodeOffsetChunk.setValue<offset_t>(csrOffset, i);
         csrOffsetChunk.setValue<offset_t>(csrOffset + 1, nodeOffset);
     }
 }
 
-void RelBatchInsert::appendNewNodeGroup(const RelBatchInsertInfo& relInfo,
-    RelBatchInsertLocalState& localState, BatchInsertSharedState& sharedState,
-    const PartitionerSharedState& partitionerSharedState) {
+void RelBatchInsert::appendNewNodeGroup(transaction::Transaction* transaction,
+    const RelBatchInsertInfo& relInfo, RelBatchInsertLocalState& localState,
+    BatchInsertSharedState& sharedState, const PartitionerSharedState& partitionerSharedState) {
     auto nodeGroupIdx = localState.nodeGroupIdx;
     auto& partitioningBuffer =
         partitionerSharedState.getPartitionBuffer(relInfo.partitioningIdx, localState.nodeGroupIdx);
     auto startNodeOffset = StorageUtils::getStartOffsetOfNodeGroup(nodeGroupIdx);
     for (auto& chunkedGroup : partitioningBuffer.getChunkedGroups()) {
         setOffsetToWithinNodeGroup(chunkedGroup->getColumnChunkUnsafe(relInfo.offsetColumnID),
             startNodeOffset);
@@ -192,15 +192,15 @@
     prepareCSRNodeGroup(partitioningBuffer, startNodeOffset, relInfo, localState, numNodes);
     for (auto& chunkedGroup : partitioningBuffer.getChunkedGroups()) {
         localState.nodeGroup->write(*chunkedGroup, relInfo.offsetColumnID);
     }
     localState.nodeGroup->finalize(nodeGroupIdx);
     // Flush node group to table.
     auto relTable = ku_dynamic_cast<Table*, RelTable*>(sharedState.table);
-    relTable->append(localState.nodeGroup.get(), relInfo.direction);
+    relTable->append(transaction, localState.nodeGroup.get(), relInfo.direction);
     sharedState.incrementNumRows(localState.nodeGroup->getNumRows());
     localState.nodeGroup->resetToEmpty();
 }
 
 std::optional<offset_t> RelBatchInsert::checkRelMultiplicityConstraint(
     const storage::ChunkedCSRHeader& csrHeader, const RelBatchInsertInfo& relInfo) {
     auto relTableEntry =
```

### sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp

```diff
@@ -14,16 +14,16 @@
     for (auto i = 0u; i < StorageConstants::PAGE_GROUP_SIZE; i++) {
         walPageIdxLocks[i] = std::make_unique<std::mutex>();
     }
 }
 
 BMFileHandle::BMFileHandle(const std::string& path, uint8_t flags, BufferManager* bm,
     PageSizeClass pageSizeClass, FileVersionedType fileVersionedType,
-    common::VirtualFileSystem* vfs)
-    : FileHandle{path, flags, vfs}, fileVersionedType{fileVersionedType}, bm{bm},
+    common::VirtualFileSystem* vfs, main::ClientContext* context)
+    : FileHandle{path, flags, vfs, context}, fileVersionedType{fileVersionedType}, bm{bm},
       pageSizeClass{pageSizeClass}, pageStates{numPages, pageCapacity},
       frameGroupIdxes{getNumPageGroups(), getNumPageGroups()} {
     for (auto i = 0u; i < frameGroupIdxes.size(); i++) {
         frameGroupIdxes[i] = bm->addNewFrameGroup(pageSizeClass);
     }
 }
```

### sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp

```diff
@@ -15,18 +15,20 @@
 
 MemoryBuffer::~MemoryBuffer() {
     if (buffer != nullptr) {
         allocator->freeBlock(pageIdx, buffer);
     }
 }
 
-MemoryAllocator::MemoryAllocator(BufferManager* bm, VirtualFileSystem* vfs) : bm{bm} {
+MemoryAllocator::MemoryAllocator(BufferManager* bm, VirtualFileSystem* vfs,
+    main::ClientContext* context)
+    : bm{bm} {
     pageSize = BufferPoolConstants::PAGE_256KB_SIZE;
     fh = bm->getBMFileHandle("mm-256KB", FileHandle::O_IN_MEM_TEMP_FILE,
-        BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs, PAGE_256KB);
+        BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs, context, PAGE_256KB);
 }
 
 MemoryAllocator::~MemoryAllocator() = default;
 
 std::unique_ptr<MemoryBuffer> MemoryAllocator::allocateBuffer(bool initializeToZero,
     uint64_t size) {
     if (size > BufferPoolConstants::PAGE_256KB_SIZE) [[unlikely]] {
```

### sdist/kuzu-source/src/storage/file_handle.cpp

```diff
@@ -8,45 +8,44 @@
 #include "common/file_system/virtual_file_system.h"
 
 using namespace kuzu::common;
 
 namespace kuzu {
 namespace storage {
 
-FileHandle::FileHandle(const std::string& path, uint8_t flags, VirtualFileSystem* vfs)
+FileHandle::FileHandle(const std::string& path, uint8_t flags, VirtualFileSystem* vfs,
+    main::ClientContext* context)
     : flags{flags} {
     if (!isNewTmpFile()) {
-        constructExistingFileHandle(path, vfs);
+        constructExistingFileHandle(path, vfs, context);
     } else {
-        constructNewFileHandle(path);
+        constructNewFileHandle(path, vfs, context);
     }
 }
 
-void FileHandle::constructExistingFileHandle(const std::string& path, VirtualFileSystem* vfs) {
+void FileHandle::constructExistingFileHandle(const std::string& path, VirtualFileSystem* vfs,
+    main::ClientContext* context) {
     int openFlags;
     if (isReadOnlyFile()) {
         openFlags = O_RDONLY;
     } else {
         openFlags = O_RDWR | ((createFileIfNotExists()) ? O_CREAT : 0x00000000);
     }
-    fileInfo = vfs->openFile(path, openFlags);
+    fileInfo = vfs->openFile(path, openFlags, context);
     auto fileLength = fileInfo->getFileSize();
     numPages = ceil((double)fileLength / (double)getPageSize());
     pageCapacity = 0;
     while (pageCapacity < numPages) {
         pageCapacity += StorageConstants::PAGE_GROUP_SIZE;
     }
 }
 
-void FileHandle::constructNewFileHandle(const std::string& path) {
-#ifdef _WIN32
-    fileInfo = make_unique<FileInfo>(path, nullptr /* fs */);
-#else
-    fileInfo = make_unique<FileInfo>(path, nullptr /* fs */);
-#endif
+void FileHandle::constructNewFileHandle(const std::string& path, VirtualFileSystem* vfs,
+    main::ClientContext* context) {
+    fileInfo = vfs->openFile(path, O_CREAT | O_RDWR, context);
     numPages = 0;
     pageCapacity = 0;
 }
 
 page_idx_t FileHandle::addNewPage() {
     return addNewPages(1 /* numNewPages */);
 }
```

### sdist/kuzu-source/src/storage/index/hash_index.cpp

```diff
@@ -627,23 +627,23 @@
 template class HashIndex<double>;
 template class HashIndex<float>;
 template class HashIndex<int128_t>;
 template class HashIndex<ku_string_t>;
 
 PrimaryKeyIndex::PrimaryKeyIndex(const DBFileIDAndName& dbFileIDAndName, bool readOnly,
     common::PhysicalTypeID keyDataType, BufferManager& bufferManager, WAL* wal,
-    VirtualFileSystem* vfs)
+    VirtualFileSystem* vfs, main::ClientContext* context)
     : hasRunPrepareCommit{false}, keyDataTypeID(keyDataType), bufferManager{bufferManager} {
     fileHandle = bufferManager.getBMFileHandle(dbFileIDAndName.fName,
         readOnly ? FileHandle::O_PERSISTENT_FILE_READ_ONLY :
                    FileHandle::O_PERSISTENT_FILE_NO_CREATE,
-        BMFileHandle::FileVersionedType::VERSIONED_FILE, vfs);
+        BMFileHandle::FileVersionedType::VERSIONED_FILE, vfs, context);
     if (keyDataTypeID == PhysicalTypeID::STRING) {
-        overflowFile =
-            std::make_unique<OverflowFile>(dbFileIDAndName, &bufferManager, wal, readOnly, vfs);
+        overflowFile = std::make_unique<OverflowFile>(dbFileIDAndName, &bufferManager, wal,
+            readOnly, vfs, context);
     }
 
     hashIndices.reserve(NUM_HASH_INDEXES);
     TypeUtils::visit(
         keyDataTypeID,
         [&](ku_string_t) {
             for (auto i = 0u; i < NUM_HASH_INDEXES; i++) {
@@ -746,22 +746,23 @@
         hashIndices[i]->prepareRollback();
     }
 }
 
 PrimaryKeyIndex::~PrimaryKeyIndex() = default;
 
 void PrimaryKeyIndex::createEmptyHashIndexFiles(PhysicalTypeID typeID, const std::string& fName,
-    VirtualFileSystem* vfs) {
-    FileHandle fileHandle(fName, FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS, vfs);
+    VirtualFileSystem* vfs, main::ClientContext* context) {
+    FileHandle fileHandle(fName, FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS, vfs, context);
     fileHandle.addNewPages(NUM_HEADER_PAGES * NUM_HASH_INDEXES);
     common::TypeUtils::visit(
         typeID,
         [&]<common::IndexHashable T>(T) {
             if constexpr (std::same_as<T, common::ku_string_t>) {
-                OverflowFile::createEmptyFiles(StorageUtils::getOverflowFileName(fName), vfs);
+                OverflowFile::createEmptyFiles(StorageUtils::getOverflowFileName(fName), vfs,
+                    context);
             }
             for (auto i = 0u; i < NUM_HASH_INDEXES; i++) {
                 InMemHashIndex<T>::createEmptyIndexFiles(i, fileHandle);
             }
         },
         [&](auto) { KU_UNREACHABLE; });
 }
```

### sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp

```diff
@@ -3,19 +3,21 @@
 using namespace kuzu::common;
 using namespace kuzu::transaction;
 
 namespace kuzu {
 namespace storage {
 
 NodesStoreStatsAndDeletedIDs::NodesStoreStatsAndDeletedIDs(const std::string& databasePath,
-    BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal, VirtualFileSystem* fs)
+    BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal, VirtualFileSystem* fs,
+    main::ClientContext* context)
     : TablesStatistics{metadataFH, bufferManager, wal} {
     if (fs->fileOrPathExists(StorageUtils::getNodesStatisticsAndDeletedIDsFilePath(fs, databasePath,
-            FileVersionType::ORIGINAL))) {
-        readFromFile(databasePath, FileVersionType::ORIGINAL, fs);
+                                 FileVersionType::ORIGINAL),
+            context)) {
+        readFromFile(databasePath, FileVersionType::ORIGINAL, fs, context);
     } else {
         saveToFile(databasePath, FileVersionType::ORIGINAL, TransactionType::READ_ONLY, fs);
     }
 }
 
 offset_t NodesStoreStatsAndDeletedIDs::getMaxNodeOffset(Transaction* transaction,
     table_id_t tableID) {
```

### sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp

```diff
@@ -7,19 +7,20 @@
 using namespace kuzu::common;
 using namespace kuzu::transaction;
 
 namespace kuzu {
 namespace storage {
 
 RelsStoreStats::RelsStoreStats(const std::string& databasePath, BMFileHandle* metadataFH,
-    BufferManager* bufferManager, WAL* wal, VirtualFileSystem* fs)
+    BufferManager* bufferManager, WAL* wal, VirtualFileSystem* fs, main::ClientContext* context)
     : TablesStatistics{metadataFH, bufferManager, wal} {
     if (fs->fileOrPathExists(
-            StorageUtils::getRelsStatisticsFilePath(fs, databasePath, FileVersionType::ORIGINAL))) {
-        readFromFile(databasePath, FileVersionType::ORIGINAL, fs);
+            StorageUtils::getRelsStatisticsFilePath(fs, databasePath, FileVersionType::ORIGINAL),
+            context)) {
+        readFromFile(databasePath, FileVersionType::ORIGINAL, fs, context);
     } else {
         saveToFile(databasePath, FileVersionType::ORIGINAL, TransactionType::READ_ONLY, fs);
     }
 }
 
 void RelsStoreStats::updateNumTuplesByValue(table_id_t relTableID, int64_t value) {
     std::unique_lock lck{mtx};
```

### sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp

```diff
@@ -16,18 +16,18 @@
 
 TablesStatistics::TablesStatistics(BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal)
     : metadataFH{metadataFH}, bufferManager{bufferManager}, wal{wal}, isUpdated{false} {
     readOnlyVersion = std::make_unique<TablesStatisticsContent>();
 }
 
 void TablesStatistics::readFromFile(const std::string& dbPath, FileVersionType fileVersionType,
-    VirtualFileSystem* fs) {
+    VirtualFileSystem* fs, main::ClientContext* context) {
     auto filePath = getTableStatisticsFilePath(dbPath, fileVersionType, fs);
-    auto deser =
-        Deserializer(std::make_unique<BufferedFileReader>(fs->openFile(filePath, O_RDONLY)));
+    auto deser = Deserializer(
+        std::make_unique<BufferedFileReader>(fs->openFile(filePath, O_RDONLY, context)));
     deser.deserializeUnorderedMap(readOnlyVersion->tableStatisticPerTable);
 }
 
 void TablesStatistics::saveToFile(const std::string& directory, FileVersionType fileVersionType,
     transaction::TransactionType transactionType, VirtualFileSystem* fs) {
     auto filePath = getTableStatisticsFilePath(directory, fileVersionType, fs);
     auto ser = Serializer(
```

### sdist/kuzu-source/src/storage/storage_manager.cpp

```diff
@@ -14,33 +14,36 @@
 using namespace kuzu::transaction;
 
 namespace kuzu {
 namespace storage {
 
 StorageManager::StorageManager(const std::string& databasePath, bool readOnly,
     const Catalog& catalog, MemoryManager& memoryManager, bool enableCompression,
-    VirtualFileSystem* vfs)
+    VirtualFileSystem* vfs, main::ClientContext* context)
     : databasePath{databasePath}, readOnly{readOnly}, memoryManager{memoryManager},
-      enableCompression{enableCompression}, vfs{vfs} {
-    dataFH = initFileHandle(StorageUtils::getDataFName(vfs, databasePath));
-    metadataFH = initFileHandle(StorageUtils::getMetadataFName(vfs, databasePath));
+      enableCompression{enableCompression} {
+    dataFH = initFileHandle(StorageUtils::getDataFName(vfs, databasePath), vfs, context);
+    metadataFH = initFileHandle(StorageUtils::getMetadataFName(vfs, databasePath), vfs, context);
     // TODO: Assert no wal file exists.
-    wal = std::make_unique<WAL>(databasePath, readOnly, *memoryManager.getBufferManager(), vfs);
+    // TODO: should we disable WAL in readonly mode?
+    wal = std::make_unique<WAL>(databasePath, readOnly, *memoryManager.getBufferManager(), vfs,
+        context);
     nodesStatisticsAndDeletedIDs = std::make_unique<NodesStoreStatsAndDeletedIDs>(databasePath,
-        metadataFH.get(), memoryManager.getBufferManager(), wal.get(), vfs);
+        metadataFH.get(), memoryManager.getBufferManager(), wal.get(), vfs, context);
     relsStatistics = std::make_unique<RelsStoreStats>(databasePath, metadataFH.get(),
-        memoryManager.getBufferManager(), wal.get(), vfs);
-    loadTables(catalog);
+        memoryManager.getBufferManager(), wal.get(), vfs, context);
+    loadTables(catalog, vfs, context);
 }
 
-std::unique_ptr<BMFileHandle> StorageManager::initFileHandle(const std::string& filename) {
+std::unique_ptr<BMFileHandle> StorageManager::initFileHandle(const std::string& filename,
+    VirtualFileSystem* vfs, main::ClientContext* context) {
     return memoryManager.getBufferManager()->getBMFileHandle(filename,
         readOnly ? FileHandle::O_PERSISTENT_FILE_READ_ONLY :
                    FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS,
-        BMFileHandle::FileVersionedType::VERSIONED_FILE, vfs);
+        BMFileHandle::FileVersionedType::VERSIONED_FILE, vfs, context);
 }
 
 static void setCommonTableIDToRdfRelTable(RelTable* relTable,
     std::vector<RDFGraphCatalogEntry*> rdfEntries) {
     for (auto rdfEntry : rdfEntries) {
         if (rdfEntry->isParent(relTable->getTableID())) {
             std::vector<Column*> columns;
@@ -52,19 +55,20 @@
                 ku_dynamic_cast<storage::Column*, storage::InternalIDColumn*>(column)
                     ->setCommonTableID(rdfEntry->getResourceTableID());
             }
         }
     }
 }
 
-void StorageManager::loadTables(const Catalog& catalog) {
+void StorageManager::loadTables(const Catalog& catalog, VirtualFileSystem* vfs,
+    main::ClientContext* context) {
     for (auto& nodeTableEntry : catalog.getNodeTableEntries(&DUMMY_READ_TRANSACTION)) {
         KU_ASSERT(!tables.contains(nodeTableEntry->getTableID()));
         tables[nodeTableEntry->getTableID()] =
-            std::make_unique<NodeTable>(this, nodeTableEntry, &memoryManager, vfs);
+            std::make_unique<NodeTable>(this, nodeTableEntry, &memoryManager, vfs, context);
     }
     auto rdfGraphSchemas = catalog.getRdfGraphEntries(&DUMMY_READ_TRANSACTION);
     for (auto relTableEntry : catalog.getRelTableEntries(&DUMMY_READ_TRANSACTION)) {
         KU_ASSERT(!tables.contains(relTableEntry->getTableID()));
         auto relTable = std::make_unique<RelTable>(dataFH.get(), metadataFH.get(),
             relsStatistics.get(), &memoryManager, relTableEntry, wal.get(), enableCompression);
         setCommonTableIDToRdfRelTable(relTable.get(), rdfGraphSchemas);
@@ -80,15 +84,15 @@
         return;
     }
     try {
         auto shadowFH = clientContext.getMemoryManager()->getBufferManager()->getBMFileHandle(
             vfs->joinPath(clientContext.getDatabasePath(),
                 std::string(StorageConstants::SHADOWING_SUFFIX)),
             FileHandle::O_PERSISTENT_FILE_NO_CREATE,
-            BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs);
+            BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs, &clientContext);
         auto walReplayer = std::make_unique<WALReplayer>(clientContext, *shadowFH,
             WALReplayMode::RECOVERY_CHECKPOINT);
         walReplayer->replay();
         // Truncate .wal and .shadow to empty. Remove catalog and stats wal files.
         auto walFileInfo = vfs->openFile(walFilePath, O_RDWR);
         if (walFileInfo->getFileSize() > 0) {
             walFileInfo->truncate(0);
@@ -98,18 +102,22 @@
         }
         StorageUtils::removeCatalogAndStatsWALFiles(clientContext.getDatabasePath(), vfs);
     } catch (std::exception& e) {
         throw Exception(stringFormat("Error during recovery: {}", e.what()));
     }
 }
 
-void StorageManager::createNodeTable(table_id_t tableID, NodeTableCatalogEntry* nodeTableEntry) {
+void StorageManager::createNodeTable(table_id_t tableID, NodeTableCatalogEntry* nodeTableEntry,
+    main::ClientContext* context) {
+    KU_ASSERT(context != nullptr);
     nodesStatisticsAndDeletedIDs->addNodeStatisticsAndDeletedIDs(nodeTableEntry);
-    WALReplayerUtils::createEmptyHashIndexFiles(nodeTableEntry, databasePath, vfs);
-    tables[tableID] = std::make_unique<NodeTable>(this, nodeTableEntry, &memoryManager, vfs);
+    WALReplayerUtils::createEmptyHashIndexFiles(nodeTableEntry, databasePath,
+        context->getVFSUnsafe(), context);
+    tables[tableID] = std::make_unique<NodeTable>(this, nodeTableEntry, &memoryManager,
+        context->getVFSUnsafe(), context);
 }
 
 void StorageManager::createRelTable(table_id_t tableID, RelTableCatalogEntry* relTableEntry,
     Catalog* catalog, Transaction* transaction) {
     relsStatistics->addTableStatistic(relTableEntry);
     auto relTable = std::make_unique<RelTable>(dataFH.get(), metadataFH.get(), relsStatistics.get(),
         &memoryManager, relTableEntry, wal.get(), enableCompression);
@@ -124,55 +132,54 @@
             ku_dynamic_cast<TableCatalogEntry*, RelTableCatalogEntry*>(
                 catalog->getTableCatalogEntry(transaction, relTableID)),
             catalog, transaction);
     }
 }
 
 void StorageManager::createRdfGraph(table_id_t, RDFGraphCatalogEntry* tableSchema, Catalog* catalog,
-    Transaction* transaction) {
+    main::ClientContext* context) {
+    KU_ASSERT(context != nullptr);
     auto rdfGraphSchema = ku_dynamic_cast<TableCatalogEntry*, RDFGraphCatalogEntry*>(tableSchema);
     auto resourceTableID = rdfGraphSchema->getResourceTableID();
     auto resourceTableEntry = ku_dynamic_cast<TableCatalogEntry*, NodeTableCatalogEntry*>(
-        catalog->getTableCatalogEntry(transaction, resourceTableID));
-    createNodeTable(resourceTableID, resourceTableEntry);
+        catalog->getTableCatalogEntry(context->getTx(), resourceTableID));
+    createNodeTable(resourceTableID, resourceTableEntry, context);
     auto literalTableID = rdfGraphSchema->getLiteralTableID();
-    auto literalTableEntry = ku_dynamic_cast<TableCatalogEntry*, NodeTableCatalogEntry*>(
-        catalog->getTableCatalogEntry(transaction, literalTableID));
-    createNodeTable(literalTableID, literalTableEntry);
+    auto literalTableEntry = catalog->getTableCatalogEntry(context->getTx(), literalTableID)
+                                 ->ptrCast<NodeTableCatalogEntry>();
+    createNodeTable(literalTableID, literalTableEntry, context);
     auto resourceTripleTableID = rdfGraphSchema->getResourceTripleTableID();
-    auto resourceTripleTableEntry = ku_dynamic_cast<TableCatalogEntry*, RelTableCatalogEntry*>(
-        catalog->getTableCatalogEntry(transaction, resourceTripleTableID));
-    createRelTable(resourceTripleTableID, resourceTripleTableEntry, catalog, transaction);
+    auto resourceTripleTableEntry =
+        catalog->getTableCatalogEntry(context->getTx(), resourceTripleTableID)
+            ->ptrCast<RelTableCatalogEntry>();
+    createRelTable(resourceTripleTableID, resourceTripleTableEntry, catalog, context->getTx());
     auto literalTripleTableID = rdfGraphSchema->getLiteralTripleTableID();
-    auto literalTripleTableEntry = ku_dynamic_cast<TableCatalogEntry*, RelTableCatalogEntry*>(
-        catalog->getTableCatalogEntry(transaction, literalTripleTableID));
-    createRelTable(literalTripleTableID, literalTripleTableEntry, catalog, transaction);
+    auto literalTripleTableEntry =
+        catalog->getTableCatalogEntry(context->getTx(), literalTripleTableID)
+            ->ptrCast<RelTableCatalogEntry>();
+    createRelTable(literalTripleTableID, literalTripleTableEntry, catalog, context->getTx());
 }
 
-void StorageManager::createTable(table_id_t tableID, Catalog* catalog, Transaction* transaction) {
-    auto tableEntry = catalog->getTableCatalogEntry(transaction, tableID);
+void StorageManager::createTable(table_id_t tableID, Catalog* catalog,
+    main::ClientContext* context) {
+    auto tableEntry = catalog->getTableCatalogEntry(context->getTx(), tableID);
     switch (tableEntry->getTableType()) {
     case TableType::NODE: {
-        createNodeTable(tableID,
-            ku_dynamic_cast<TableCatalogEntry*, NodeTableCatalogEntry*>(tableEntry));
+        createNodeTable(tableID, tableEntry->ptrCast<NodeTableCatalogEntry>(), context);
     } break;
     case TableType::REL: {
-        createRelTable(tableID,
-            ku_dynamic_cast<TableCatalogEntry*, RelTableCatalogEntry*>(tableEntry), catalog,
-            transaction);
+        createRelTable(tableID, tableEntry->ptrCast<RelTableCatalogEntry>(), catalog,
+            context->getTx());
     } break;
     case TableType::REL_GROUP: {
-        createRelTableGroup(tableID,
-            ku_dynamic_cast<TableCatalogEntry*, RelGroupCatalogEntry*>(tableEntry), catalog,
-            transaction);
+        createRelTableGroup(tableID, tableEntry->ptrCast<RelGroupCatalogEntry>(), catalog,
+            context->getTx());
     } break;
     case TableType::RDF: {
-        createRdfGraph(tableID,
-            ku_dynamic_cast<TableCatalogEntry*, RDFGraphCatalogEntry*>(tableEntry), catalog,
-            transaction);
+        createRdfGraph(tableID, tableEntry->ptrCast<RDFGraphCatalogEntry>(), catalog, context);
     } break;
     default: {
         KU_UNREACHABLE;
     }
     }
 }
 
@@ -184,15 +191,15 @@
 }
 
 WAL& StorageManager::getWAL() {
     KU_ASSERT(wal);
     return *wal;
 }
 
-void StorageManager::dropTable(table_id_t tableID) {
+void StorageManager::dropTable(table_id_t tableID, VirtualFileSystem* vfs) {
     KU_ASSERT(tables.contains(tableID));
     auto tableType = tables.at(tableID)->getTableType();
     switch (tableType) {
     case TableType::NODE: {
         nodesStatisticsAndDeletedIDs->removeTableStatistic(tableID);
         WALReplayerUtils::removeHashIndexFile(vfs, tableID, databasePath);
     } break;
@@ -202,15 +209,15 @@
     default: {
         KU_UNREACHABLE;
     }
     }
     tables.erase(tableID);
 }
 
-void StorageManager::prepareCommit(Transaction* transaction) {
+void StorageManager::prepareCommit(Transaction* transaction, common::VirtualFileSystem* vfs) {
     // Tables which are created but not inserted into may have pending writes
     // which need to be flushed (specifically, the metadata disk array header)
     // TODO(bmwinger): wal->getUpdatedTables isn't the ideal place to store this information
     for (auto tableID : wal->getUpdatedTables()) {
         if (transaction->getLocalStorage()->getLocalTable(tableID) == nullptr) {
             getTable(tableID)->prepareCommit();
         }
```

### sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp

```diff
@@ -155,34 +155,35 @@
     DBFileIDAndName copy = dbFileIdAndNameForMainDBFile;
     copy.dbFileID.isOverflow = true;
     copy.fName = StorageUtils::getOverflowFileName(dbFileIdAndNameForMainDBFile.fName);
     return copy;
 }
 
 OverflowFile::OverflowFile(const DBFileIDAndName& dbFileIdAndName, BufferManager* bufferManager,
-    WAL* wal, bool readOnly, common::VirtualFileSystem* vfs)
+    WAL* wal, bool readOnly, common::VirtualFileSystem* vfs, main::ClientContext* context)
     : bufferManager{bufferManager}, wal{wal}, headerChanged{false} {
     auto overflowFileIDAndName = constructDBFileIDAndName(dbFileIdAndName);
     dbFileID = overflowFileIDAndName.dbFileID;
     fileHandle = bufferManager->getBMFileHandle(overflowFileIDAndName.fName,
         readOnly ? FileHandle::O_PERSISTENT_FILE_READ_ONLY :
                    FileHandle::O_PERSISTENT_FILE_NO_CREATE,
-        BMFileHandle::FileVersionedType::VERSIONED_FILE, vfs);
+        BMFileHandle::FileVersionedType::VERSIONED_FILE, vfs, context);
     if (vfs->fileOrPathExists(overflowFileIDAndName.fName)) {
         readFromDisk(transaction::TransactionType::READ_ONLY, HEADER_PAGE_IDX,
             [&](auto* frame) { memcpy(&header, frame, sizeof(header)); });
         pageCounter = numPagesOnDisk = header.pages;
     } else {
         // Reserve a page for the header
         getNewPageIdx();
     }
 }
 
-void OverflowFile::createEmptyFiles(const std::string& fName, common::VirtualFileSystem* vfs) {
-    FileHandle fileHandle(fName, FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS, vfs);
+void OverflowFile::createEmptyFiles(const std::string& fName, common::VirtualFileSystem* vfs,
+    main::ClientContext* context) {
+    FileHandle fileHandle(fName, FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS, vfs, context);
     uint8_t page[common::BufferPoolConstants::PAGE_4KB_SIZE];
     StringOverflowFileHeader header;
     memcpy(page, &header, sizeof(StringOverflowFileHeader));
     // Zero free space at the end of the header page
     std::fill(page + sizeof(header), page + BufferPoolConstants::PAGE_4KB_SIZE, 0);
     fileHandle.addNewPage();
     fileHandle.writePage(page, HEADER_PAGE_IDX);
```

### sdist/kuzu-source/src/storage/store/column.cpp

```diff
@@ -155,55 +155,51 @@
         if (numValues > state.metadata.numValues) {
             state.metadata.numValues = numValues;
             // TODO: Avoid updating metadataDA.
             metadataDA->update(state.nodeGroupIdx, state.metadata);
         }
     }
 
-    void commitLocalChunkOutOfPlace(Transaction*, node_group_idx_t nodeGroupIdx,
-        bool isNewNodeGroup, const ChunkCollection&, const offset_to_row_idx_t& insertInfo,
-        const ChunkCollection&, const offset_to_row_idx_t& updateInfo,
-        const offset_set_t& deleteInfo) override {
+    void commitLocalChunkOutOfPlace(Transaction*, ChunkState& state, bool isNewNodeGroup,
+        const ChunkCollection&, const offset_to_row_idx_t& insertInfo, const ChunkCollection&,
+        const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) override {
         // Avoid unused parameter warnings during release build.
         (void)isNewNodeGroup;
         (void)updateInfo;
         (void)deleteInfo;
         KU_ASSERT(isNewNodeGroup && updateInfo.empty() && deleteInfo.empty());
         // Only when a new node group is created, we need to commit out of place.
         auto numValues = 0u;
         for (auto& [offsetInChunk, _] : insertInfo) {
             numValues = offsetInChunk >= numValues ? offsetInChunk + 1 : numValues;
         }
-        ColumnChunkMetadata chunkMeta;
-        chunkMeta.numValues = numValues;
-        metadataDA->resize(nodeGroupIdx + 1);
-        metadataDA->update(nodeGroupIdx, chunkMeta);
+        state.metadata.numValues = numValues;
+        metadataDA->resize(state.nodeGroupIdx + 1);
+        metadataDA->update(state.nodeGroupIdx, state.metadata);
     }
 
     void commitColumnChunkInPlace(ChunkState&, const std::vector<common::offset_t>&, ColumnChunk*,
         common::offset_t) override {
         // Note: only updates to rel table can trigger this code path. SERIAL is not supported in
         // rel table yet.
         KU_UNREACHABLE;
     }
 
-    void commitColumnChunkOutOfPlace(Transaction* /*transaction*/,
-        common::node_group_idx_t /*nodeGroupIdx*/, bool /*isNewNodeGroup*/,
-        const std::vector<common::offset_t>& /*dstOffset*/, ColumnChunk* /*chunk*/,
-        common::offset_t /*srcOffsetInChunk*/) override {
+    void commitColumnChunkOutOfPlace(Transaction*, ChunkState&, bool,
+        const std::vector<common::offset_t>&, ColumnChunk*, common::offset_t) override {
         // Note: only updates to rel table can trigger this code path. SERIAL is not supported in
         // rel table yet.
         KU_UNREACHABLE;
     }
 
-    void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override {
-        ColumnChunkMetadata metadata;
-        metadata.numValues = columnChunk->getNumValues();
-        metadataDA->resize(nodeGroupIdx + 1);
-        metadataDA->update(nodeGroupIdx, metadata);
+    void append(ColumnChunk* columnChunk, ChunkState& state) override {
+        KU_ASSERT(state.nodeGroupIdx != INVALID_NODE_GROUP_IDX);
+        state.metadata.numValues = columnChunk->getNumValues();
+        metadataDA->resize(state.nodeGroupIdx + 1);
+        metadataDA->update(state.nodeGroupIdx, state.metadata);
     }
 };
 
 InternalIDColumn::InternalIDColumn(std::string name, const MetadataDAHInfo& metaDAHeaderInfo,
     BMFileHandle* dataFH, BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal,
     transaction::Transaction* transaction, RWPropertyStats stats, bool enableCompression)
     : Column{name, *LogicalType::INTERNAL_ID(), metaDAHeaderInfo, dataFH, metadataFH, bufferManager,
@@ -273,23 +269,24 @@
     ChunkState& readState) {
     if (nullColumn) {
         if (!readState.nullState) {
             readState.nullState = std::make_unique<ChunkState>();
         }
         nullColumn->initChunkState(transaction, nodeGroupIdx, *readState.nullState);
     }
-    KU_ASSERT(nodeGroupIdx < metadataDA->getNumElements(transaction->getType()));
-    if (nodeGroupIdx != readState.nodeGroupIdx) {
+    if (readState.nodeGroupIdx != nodeGroupIdx) {
         // Only update metadata and numValuesPerPage if we're reading a different node group.
-        // This is an optimization to reduce accesses to metadataDA, which can lead to contention
-        // due to lock acquiring in DiskArray.
+        // This is an optimization to reduce accesses to metadataDA, which can lead to
+        // contention due to lock acquiring in DiskArray.
         readState.nodeGroupIdx = nodeGroupIdx;
-        readState.metadata = metadataDA->get(nodeGroupIdx, transaction->getType());
-        readState.numValuesPerPage =
-            readState.metadata.compMeta.numValues(BufferPoolConstants::PAGE_4KB_SIZE, dataType);
+        if (nodeGroupIdx < metadataDA->getNumElements(transaction->getType())) {
+            readState.metadata = metadataDA->get(nodeGroupIdx, transaction->getType());
+            readState.numValuesPerPage =
+                readState.metadata.compMeta.numValues(BufferPoolConstants::PAGE_4KB_SIZE, dataType);
+        }
     }
 }
 
 void Column::scan(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
     ValueVector* resultVector) {
     if (nullColumn) {
         KU_ASSERT(readState.nullState);
@@ -492,27 +489,29 @@
         } else {
             return std::ceil((double)metadata.numValues / (double)numValuesPerPage) <=
                    metadata.numPages;
         }
     }
 }
 
-void Column::append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) {
-    KU_ASSERT(enableCompression == columnChunk->isCompressionEnabled());
+void Column::append(ColumnChunk* columnChunk, ChunkState& state) {
+    KU_ASSERT(enableCompression == columnChunk->isCompressionEnabled() &&
+              state.nodeGroupIdx != INVALID_NODE_GROUP_IDX);
     KU_ASSERT(columnChunk->sanityCheck());
     // Main column chunk.
     auto preScanMetadata = columnChunk->getMetadataToFlush();
     auto startPageIdx = dataFH->addNewPages(preScanMetadata.numPages);
-    auto metadata = columnChunk->flushBuffer(dataFH, startPageIdx, preScanMetadata);
-    KU_ASSERT(sanityCheckForWrites(metadata, dataType));
-    metadataDA->resize(nodeGroupIdx + 1);
-    metadataDA->update(nodeGroupIdx, metadata);
+    state.metadata = columnChunk->flushBuffer(dataFH, startPageIdx, preScanMetadata);
+    KU_ASSERT(sanityCheckForWrites(state.metadata, dataType));
+    metadataDA->resize(state.nodeGroupIdx + 1);
+    metadataDA->update(state.nodeGroupIdx, state.metadata);
     if (nullColumn) {
         // Null column chunk.
-        nullColumn->append(columnChunk->getNullChunk(), nodeGroupIdx);
+        KU_ASSERT(state.nullState);
+        nullColumn->append(columnChunk->getNullChunk(), *state.nullState);
     }
 }
 
 void Column::write(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
     uint32_t posInVectorToWriteFrom) {
     bool isNull = vectorToWriteFrom->isNull(posInVectorToWriteFrom);
     if (!isNull) {
@@ -603,38 +602,38 @@
     }
 }
 
 void Column::prepareCommitForChunk(Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
     bool isNewNodeGroup, const ChunkCollection& localInsertChunks,
     const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
     const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) {
+    ChunkState state;
+    initChunkState(transaction, nodeGroupIdx, state);
     if (isNewNodeGroup) {
         // If this is a new node group, updateInfo should be empty. We should perform out-of-place
         // commit with a new column chunk.
-        commitLocalChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, localInsertChunks,
+        commitLocalChunkOutOfPlace(transaction, state, isNewNodeGroup, localInsertChunks,
             insertInfo, localUpdateChunks, updateInfo, deleteInfo);
     } else {
-        ChunkState state;
-        initChunkState(transaction, nodeGroupIdx, state);
         prepareCommitForExistingChunk(transaction, state, localInsertChunks, insertInfo,
             localUpdateChunks, updateInfo, deleteInfo);
     }
 }
 
 void Column::prepareCommitForChunk(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     bool isNewNodeGroup, const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
     offset_t startSrcOffset) {
     metadataDA->prepareCommit();
+    ChunkState state;
+    initChunkState(transaction, nodeGroupIdx, state);
     if (isNewNodeGroup) {
-        commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets, chunk,
+        commitColumnChunkOutOfPlace(transaction, state, isNewNodeGroup, dstOffsets, chunk,
             startSrcOffset);
     } else {
         // If this is not a new node group, we should first check if we can perform in-place commit.
-        ChunkState state;
-        initChunkState(transaction, nodeGroupIdx, state);
         prepareCommitForExistingChunk(transaction, state, dstOffsets, chunk, startSrcOffset);
     }
 }
 
 void Column::prepareCommitForExistingChunk(Transaction* transaction, Column::ChunkState& state,
     const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
     const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
@@ -649,32 +648,32 @@
             KU_ASSERT(state.nullState);
             auto nullInsertChunks = getNullChunkCollection(localInsertChunks);
             auto nullUpdateChunks = getNullChunkCollection(localUpdateChunks);
             nullColumn->prepareCommitForExistingChunk(transaction, *state.nullState,
                 nullInsertChunks, insertInfo, nullUpdateChunks, updateInfo, deleteInfo);
         }
     } else {
-        commitLocalChunkOutOfPlace(transaction, state.nodeGroupIdx, false /*isNewNodeGroup*/,
-            localInsertChunks, insertInfo, localUpdateChunks, updateInfo, deleteInfo);
+        commitLocalChunkOutOfPlace(transaction, state, false /*isNewNodeGroup*/, localInsertChunks,
+            insertInfo, localUpdateChunks, updateInfo, deleteInfo);
     }
 }
 
 void Column::prepareCommitForExistingChunk(Transaction* transaction, ChunkState& state,
     const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk, offset_t startSrcOffset) {
     if (canCommitInPlace(state, dstOffsets, chunk, startSrcOffset)) {
         commitColumnChunkInPlace(state, dstOffsets, chunk, startSrcOffset);
         KU_ASSERT(sanityCheckForWrites(state.metadata, dataType));
         metadataDA->update(state.nodeGroupIdx, state.metadata);
         if (nullColumn) {
             nullColumn->prepareCommitForExistingChunk(transaction, *state.nullState, dstOffsets,
                 chunk->getNullChunk(), startSrcOffset);
         }
     } else {
-        commitColumnChunkOutOfPlace(transaction, state.nodeGroupIdx, false /*isNewNodeGroup*/,
-            dstOffsets, chunk, startSrcOffset);
+        commitColumnChunkOutOfPlace(transaction, state, false /*isNewNodeGroup*/, dstOffsets, chunk,
+            startSrcOffset);
     }
 }
 
 bool Column::isInsertionsOutOfPagesCapacity(const ColumnChunkMetadata& metadata,
     const offset_to_row_idx_t& insertInfo) {
     auto maxOffset = 0u;
     for (auto& [offset, rowIdx] : insertInfo) {
@@ -759,71 +758,70 @@
 }
 
 std::unique_ptr<ColumnChunk> Column::getEmptyChunkForCommit(uint64_t capacity) {
     return ColumnChunkFactory::createColumnChunk(*dataType.copy(), enableCompression, capacity);
 }
 
 // TODO: Pass state in to avoid access metadata.
-void Column::commitLocalChunkOutOfPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+void Column::commitLocalChunkOutOfPlace(Transaction* transaction, ChunkState& state,
     bool isNewNodeGroup, const ChunkCollection& localInsertChunks,
     const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
     const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) {
     std::unique_ptr<ColumnChunk> columnChunk;
     if (isNewNodeGroup) {
         KU_ASSERT(updateInfo.empty() && deleteInfo.empty());
         columnChunk = getEmptyChunkForCommit(getMaxOffset(insertInfo) + 1);
         // Apply inserts from the local chunk.
         applyLocalChunkToColumnChunk(localInsertChunks, columnChunk.get(), insertInfo);
     } else {
         auto maxNodeOffset = std::max(getMaxOffset(insertInfo), getMaxOffset(updateInfo));
-        auto chunkMeta = getMetadata(nodeGroupIdx, transaction->getType());
+        auto chunkMeta = getMetadata(state.nodeGroupIdx, transaction->getType());
         maxNodeOffset = std::max(maxNodeOffset, chunkMeta.numValues);
         columnChunk = getEmptyChunkForCommit(maxNodeOffset + 1);
         // First, scan the whole column chunk from persistent storage.
-        scan(transaction, nodeGroupIdx, columnChunk.get());
+        scan(transaction, state.nodeGroupIdx, columnChunk.get());
         // Then, apply updates from the local chunk.
         applyLocalChunkToColumnChunk(localUpdateChunks, columnChunk.get(), updateInfo);
         // Lastly, apply inserts from the local chunk.
         applyLocalChunkToColumnChunk(localInsertChunks, columnChunk.get(), insertInfo);
         if (columnChunk->getNullChunk()) {
             // Set nulls based on deleteInfo.
             for (auto offsetInChunk : deleteInfo) {
                 columnChunk->getNullChunk()->setNull(offsetInChunk, true /* isNull */);
             }
         }
     }
     columnChunk->finalize();
     KU_ASSERT(columnChunk->sanityCheck());
-    append(columnChunk.get(), nodeGroupIdx);
+    append(columnChunk.get(), state);
 }
 
 void Column::commitColumnChunkInPlace(ChunkState& state, const std::vector<offset_t>& dstOffsets,
     ColumnChunk* chunk, offset_t srcOffset) {
     // TODO: Should always sort dstOffsets, and group writes to the same page.
     for (auto i = 0u; i < dstOffsets.size(); i++) {
         write(state, dstOffsets[i], chunk, srcOffset + i, 1 /* numValues */);
     }
 }
 
-void Column::commitColumnChunkOutOfPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+void Column::commitColumnChunkOutOfPlace(Transaction* transaction, ChunkState& state,
     bool isNewNodeGroup, const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk,
     offset_t srcOffset) {
     if (isNewNodeGroup) {
         chunk->finalize();
-        append(chunk, nodeGroupIdx);
+        append(chunk, state);
     } else {
-        auto chunkMeta = getMetadata(nodeGroupIdx, transaction->getType());
         auto columnChunk = getEmptyChunkForCommit(
-            std::max(std::bit_ceil(chunkMeta.numValues), getMaxOffset(dstOffsets) + 1));
-        scan(transaction, nodeGroupIdx, columnChunk.get());
+            std::max(std::bit_ceil(state.metadata.numValues), getMaxOffset(dstOffsets) + 1));
+        scan(transaction, state.nodeGroupIdx, columnChunk.get());
         for (auto i = 0u; i < dstOffsets.size(); i++) {
             columnChunk->write(chunk, srcOffset + i, dstOffsets[i], 1 /* numValues */);
         }
         columnChunk->finalize();
-        append(columnChunk.get(), nodeGroupIdx);
+        append(columnChunk.get(), state);
     }
 }
 
 void Column::applyLocalChunkToColumnChunk(const ChunkCollection& localChunks,
     ColumnChunk* columnChunk, const offset_to_row_idx_t& updateInfo) {
     for (auto& [offsetInDstChunk, rowIdx] : updateInfo) {
         auto [chunkIdx, offsetInLocalChunk] =
@@ -865,29 +863,31 @@
 
 void Column::populateWithDefaultVal(Transaction* transaction,
     DiskArray<ColumnChunkMetadata>* metadataDA_, ValueVector* defaultValueVector) {
     KU_ASSERT(metadataDA_ != nullptr);
     auto numNodeGroups = metadataDA_->getNumElements(transaction->getType());
     auto columnChunk = ColumnChunkFactory::createColumnChunk(*dataType.copy(), enableCompression);
     columnChunk->populateWithDefaultVal(defaultValueVector);
-    for (auto i = 0u; i < numNodeGroups; i++) {
-        auto chunkMeta = metadataDA_->get(i, transaction->getType());
+    ChunkState state;
+    for (auto nodeGroupIdx = 0u; nodeGroupIdx < numNodeGroups; nodeGroupIdx++) {
+        initChunkState(transaction, nodeGroupIdx, state);
+        auto chunkMeta = metadataDA_->get(nodeGroupIdx, transaction->getType());
         auto capacity = columnChunk->getCapacity();
         while (capacity < chunkMeta.numValues) {
             capacity *= CHUNK_RESIZE_RATIO;
         }
         if (capacity > columnChunk->getCapacity()) {
             auto newColumnChunk = ColumnChunkFactory::createColumnChunk(*dataType.copy(),
                 enableCompression, capacity);
             newColumnChunk->populateWithDefaultVal(defaultValueVector);
             newColumnChunk->setNumValues(chunkMeta.numValues);
-            append(newColumnChunk.get(), i);
+            append(newColumnChunk.get(), state);
         } else {
             columnChunk->setNumValues(chunkMeta.numValues);
-            append(columnChunk.get(), i);
+            append(columnChunk.get(), state);
         }
     }
 }
 
 ChunkCollection Column::getNullChunkCollection(const ChunkCollection& chunkCollection) {
     ChunkCollection nullChunkCollection;
     for (const auto& chunk : chunkCollection) {
```

### sdist/kuzu-source/src/storage/store/dictionary_column.cpp

```diff
@@ -30,18 +30,20 @@
     readState.childrenStates.resize(2);
     dataColumn->initChunkState(transaction, nodeGroupIdx,
         readState.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX]);
     offsetColumn->initChunkState(transaction, nodeGroupIdx,
         readState.childrenStates[OFFSET_COLUMN_CHILD_READ_STATE_IDX]);
 }
 
-void DictionaryColumn::append(node_group_idx_t nodeGroupIdx, const DictionaryChunk& dictChunk) {
+void DictionaryColumn::append(Column::ChunkState& state, const DictionaryChunk& dictChunk) {
     KU_ASSERT(dictChunk.sanityCheck());
-    dataColumn->append(dictChunk.getStringDataChunk(), nodeGroupIdx);
-    offsetColumn->append(dictChunk.getOffsetChunk(), nodeGroupIdx);
+    dataColumn->append(dictChunk.getStringDataChunk(),
+        state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX]);
+    offsetColumn->append(dictChunk.getOffsetChunk(),
+        state.childrenStates[OFFSET_COLUMN_CHILD_READ_STATE_IDX]);
 }
 
 void DictionaryColumn::scan(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     DictionaryChunk& dictChunk) {
     auto dataMetadata = dataColumn->getMetadata(nodeGroupIdx, transaction->getType());
     // Make sure that the chunk is large enough
     auto stringDataChunk = dictChunk.getStringDataChunk();
```

### sdist/kuzu-source/src/storage/store/list_column.cpp

```diff
@@ -114,16 +114,16 @@
 }
 
 void ListColumn::scan(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     ColumnChunk* columnChunk, offset_t startOffset, offset_t endOffset) {
     if (nodeGroupIdx >= metadataDA->getNumElements(transaction->getType())) {
         columnChunk->setNumValues(0);
     } else {
-        auto listColumnChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(columnChunk);
         Column::scan(transaction, nodeGroupIdx, columnChunk, startOffset, endOffset);
+        auto listColumnChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(columnChunk);
         auto sizeColumnChunk = listColumnChunk->getSizeColumnChunk();
         // TODO: Should use readState here too.
         sizeColumn->scan(transaction, nodeGroupIdx, sizeColumnChunk, startOffset, endOffset);
         auto resizeNumValues = listColumnChunk->getDataColumnChunk()->getNumValues();
         bool isOffsetSortedAscending = true;
         offset_t prevOffset = listColumnChunk->getListStartOffset(0);
         for (auto i = 0u; i < columnChunk->getNumValues(); i++) {
@@ -194,22 +194,22 @@
     resultVector->setValue(posInVector, list_entry_t{offsetInVector, size});
     ListVector::resizeDataVector(resultVector, offsetInVector + size);
     auto dataVector = ListVector::getDataVector(resultVector);
     dataColumn->scan(transaction, readState.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX],
         listStartOffset, listEndOffset, dataVector, offsetInVector);
 }
 
-void ListColumn::append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) {
+void ListColumn::append(ColumnChunk* columnChunk, ChunkState& state) {
     KU_ASSERT(columnChunk->getDataType().getPhysicalType() == dataType.getPhysicalType());
     auto listColumnChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(columnChunk);
-    Column::append(listColumnChunk, nodeGroupIdx);
+    Column::append(listColumnChunk, state);
     auto sizeColumnChunk = listColumnChunk->getSizeColumnChunk();
-    sizeColumn->append(sizeColumnChunk, nodeGroupIdx);
+    sizeColumn->append(sizeColumnChunk, state.childrenStates[SIZE_COLUMN_CHILD_READ_STATE_IDX]);
     auto dataColumnChunk = listColumnChunk->getDataColumnChunk();
-    dataColumn->append(dataColumnChunk, nodeGroupIdx);
+    dataColumn->append(dataColumnChunk, state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX]);
 }
 
 void ListColumn::scanUnfiltered(Transaction* transaction, ChunkState& readState,
     ValueVector* resultVector, const ListOffsetSizeInfo& listOffsetInfoInStorage) {
     auto numValuesToScan = resultVector->state->getSelVector().getSelSize();
     numValuesToScan = std::min((uint64_t)numValuesToScan, listOffsetInfoInStorage.numTotal);
     offset_t offsetInVector = 0;
@@ -363,20 +363,21 @@
             dstOffsetsInDataColumn.push_back(dataColumnSize + dataSize++);
         }
     }
     bool dataColumnCanCommitInPlace =
         dataColumn->canCommitInPlace(state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX],
             dstOffsetsInDataColumn, dataColumnChunk, startListOffset);
     if (!dataColumnCanCommitInPlace) {
-        commitColumnChunkOutOfPlace(transaction, state.nodeGroupIdx, false /*isNewNodeGroup*/,
-            dstOffsets, chunk, startSrcOffset);
+        commitColumnChunkOutOfPlace(transaction, state, false /*isNewNodeGroup*/, dstOffsets, chunk,
+            startSrcOffset);
     } else {
         // TODO: Shouldn't here be in place commit?
-        dataColumn->commitColumnChunkOutOfPlace(transaction, state.nodeGroupIdx,
-            false /*isNewNodeGroup*/, dstOffsetsInDataColumn, dataColumnChunk, startListOffset);
+        dataColumn->commitColumnChunkOutOfPlace(transaction,
+            state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX], false /*isNewNodeGroup*/,
+            dstOffsetsInDataColumn, dataColumnChunk, startListOffset);
         sizeColumn->prepareCommitForExistingChunk(transaction,
             state.childrenStates[SIZE_COLUMN_CHILD_READ_STATE_IDX], dstOffsets,
             listChunk->getSizeColumnChunk(), startSrcOffset);
         for (auto i = 0u; i < numListsToAppend; i++) {
             auto listEndOffset = listChunk->getListEndOffset(startSrcOffset + i);
             chunk->setValue<offset_t>(dataColumnSize + listEndOffset, startSrcOffset + i);
         }
@@ -397,27 +398,27 @@
     } else {
         commitOffsetColumnChunkOutOfPlace(transaction, offsetState, dstOffsets, chunk,
             startSrcOffset);
     }
 }
 
 void ListColumn::commitOffsetColumnChunkOutOfPlace(Transaction* transaction,
-    const ChunkState& offsetState, const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk,
+    ChunkState& offsetState, const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk,
     offset_t startSrcOffset) {
     auto listChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(chunk);
     auto offsetColumnChunk = ColumnChunkFactory::createColumnChunk(*dataType.copy(),
         enableCompression, 1.5 * std::bit_ceil(offsetState.metadata.numValues + dstOffsets.size()));
     Column::scan(transaction, offsetState.nodeGroupIdx, offsetColumnChunk.get());
     auto numListsToAppend = std::min(chunk->getNumValues(), (uint64_t)dstOffsets.size());
     for (auto i = 0u; i < numListsToAppend; i++) {
         auto listEndOffset = listChunk->getListEndOffset(startSrcOffset + i);
         auto isNull = listChunk->getNullChunk()->isNull(startSrcOffset + i);
         offsetColumnChunk->setValue<offset_t>(listEndOffset, dstOffsets[i]);
         offsetColumnChunk->getNullChunk()->setNull(dstOffsets[i], isNull);
     }
     auto offsetListChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(offsetColumnChunk.get());
     offsetListChunk->getSizeColumnChunk()->setNumValues(offsetColumnChunk->getNumValues());
-    Column::append(offsetColumnChunk.get(), offsetState.nodeGroupIdx);
+    Column::append(offsetColumnChunk.get(), offsetState);
 }
 
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/storage/store/node_table.cpp

```diff
@@ -14,34 +14,35 @@
 using namespace kuzu::common;
 using namespace kuzu::transaction;
 
 namespace kuzu {
 namespace storage {
 
 NodeTable::NodeTable(StorageManager* storageManager, NodeTableCatalogEntry* nodeTableEntry,
-    MemoryManager* memoryManager, VirtualFileSystem* vfs)
+    MemoryManager* memoryManager, VirtualFileSystem* vfs, main::ClientContext* context)
     : Table{nodeTableEntry, storageManager->getNodesStatisticsAndDeletedIDs(), memoryManager,
           &storageManager->getWAL()},
       pkColumnID{nodeTableEntry->getColumnID(nodeTableEntry->getPrimaryKeyPID())} {
     tableData = std::make_unique<NodeTableData>(storageManager->getDataFH(),
         storageManager->getMetadataFH(), nodeTableEntry, bufferManager, wal,
         nodeTableEntry->getPropertiesRef(), storageManager->getNodesStatisticsAndDeletedIDs(),
         storageManager->compressionEnabled());
     initializePKIndex(storageManager->getDatabasePath(), nodeTableEntry,
-        storageManager->isReadOnly(), vfs);
+        storageManager->isReadOnly(), vfs, context);
 }
 
 void NodeTable::initializePKIndex(const std::string& databasePath,
-    NodeTableCatalogEntry* nodeTableEntry, bool readOnly, VirtualFileSystem* vfs) {
+    NodeTableCatalogEntry* nodeTableEntry, bool readOnly, VirtualFileSystem* vfs,
+    main::ClientContext* context) {
     if (nodeTableEntry->getPrimaryKey()->getDataType()->getLogicalTypeID() !=
         LogicalTypeID::SERIAL) {
         pkIndex = std::make_unique<PrimaryKeyIndex>(
             StorageUtils::getNodeIndexIDAndFName(vfs, databasePath, tableID), readOnly,
             nodeTableEntry->getPrimaryKey()->getDataType()->getPhysicalType(), *bufferManager, wal,
-            vfs);
+            vfs, context);
     }
 }
 
 void NodeTable::readInternal(Transaction* transaction, TableReadState& readState) {
     tableData->read(transaction, *readState.dataReadState, *readState.nodeIDVector,
         readState.outputVectors);
     auto& dataReadState = ku_dynamic_cast<const TableDataReadState&, const NodeDataReadState&>(
```

### sdist/kuzu-source/src/storage/store/node_table_data.cpp

```diff
@@ -84,17 +84,15 @@
     auto& dataReadState = ku_dynamic_cast<TableDataReadState&, NodeDataReadState&>(readState);
     for (auto i = 0u; i < readState.columnIDs.size(); i++) {
         if (readState.columnIDs[i] != INVALID_COLUMN_ID) {
             getColumn(readState.columnIDs[i])
                 ->initChunkState(transaction, nodeGroupIdx, dataReadState.columnReadStates[i]);
         }
     }
-    if (nodeGroupIdx != dataReadState.nodeGroupIdx) {
-        KU_ASSERT(sanityCheckOnColumnNumValues(dataReadState));
-    }
+    KU_ASSERT(sanityCheckOnColumnNumValues(dataReadState));
 }
 
 bool NodeTableData::sanityCheckOnColumnNumValues(
     const kuzu::storage::NodeDataReadState& readState) {
     // Sanity check on that all valid columns should have the same numValues in the node
     // group.
     auto validColumn = std::find_if(readState.columnIDs.begin(), readState.columnIDs.end(),
@@ -182,19 +180,22 @@
             columns[readState.columnIDs[columnIdx]]->lookup(transaction,
                 nodeDataReadState.columnReadStates[columnIdx],
                 const_cast<ValueVector*>(&nodeIDVector), outputVectors[columnIdx]);
         }
     }
 }
 
-void NodeTableData::append(ChunkedNodeGroup* nodeGroup) {
+void NodeTableData::append(Transaction* transaction, ChunkedNodeGroup* nodeGroup) {
     for (auto columnID = 0u; columnID < columns.size(); columnID++) {
         auto& columnChunk = nodeGroup->getColumnChunkUnsafe(columnID);
         KU_ASSERT(columnID < columns.size());
-        columns[columnID]->append(&columnChunk, nodeGroup->getNodeGroupIdx());
+        auto column = columns[columnID].get();
+        Column::ChunkState state;
+        column->initChunkState(transaction, nodeGroup->getNodeGroupIdx(), state);
+        columns[columnID]->append(&columnChunk, state);
     }
 }
 
 void NodeTableData::prepareLocalNodeGroupToCommit(node_group_idx_t nodeGroupIdx,
     Transaction* transaction, LocalNodeNG* localNodeGroup) {
     auto numNodeGroups = columns[0]->getNumNodeGroups(transaction);
     auto isNewNodeGroup = nodeGroupIdx >= numNodeGroups;
```

### sdist/kuzu-source/src/storage/store/null_column.cpp

```diff
@@ -92,20 +92,20 @@
         for (auto i = 0ul; i < nodeIDVector->state->getSelVector().getSelSize(); i++) {
             auto pos = nodeIDVector->state->getSelVector()[i];
             resultVector->setNull(pos, false);
         }
     }
 }
 
-void NullColumn::append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) {
+void NullColumn::append(ColumnChunk* columnChunk, ChunkState& state) {
     auto preScanMetadata = columnChunk->getMetadataToFlush();
     auto startPageIdx = dataFH->addNewPages(preScanMetadata.numPages);
-    auto metadata = columnChunk->flushBuffer(dataFH, startPageIdx, preScanMetadata);
-    metadataDA->resize(nodeGroupIdx + 1);
-    metadataDA->update(nodeGroupIdx, metadata);
+    state.metadata = columnChunk->flushBuffer(dataFH, startPageIdx, preScanMetadata);
+    metadataDA->resize(state.nodeGroupIdx + 1);
+    metadataDA->update(state.nodeGroupIdx, state.metadata);
     if (static_cast<NullColumnChunk*>(columnChunk)->mayHaveNull()) {
         propertyStatistics.setHasNull(DUMMY_WRITE_TRANSACTION);
     }
 }
 
 bool NullColumn::isNull(Transaction* transaction, const ChunkState& state, offset_t offsetInChunk) {
     uint64_t result = false;
```

### sdist/kuzu-source/src/storage/store/rel_table_data.cpp

```diff
@@ -300,20 +300,27 @@
     }
     length_t length;
     csrHeaderColumns.length->scan(transaction, readState, offsetInChunk, offsetInChunk + 1,
         reinterpret_cast<uint8_t*>(&length));
     return length > 0;
 }
 
-void RelTableData::append(ChunkedNodeGroup* nodeGroup) {
+void RelTableData::append(Transaction* transaction, ChunkedNodeGroup* nodeGroup) {
     auto csrNodeGroup = ku_dynamic_cast<ChunkedNodeGroup*, ChunkedCSRNodeGroup*>(nodeGroup);
-    csrHeaderColumns.append(csrNodeGroup->getCSRHeader(), nodeGroup->getNodeGroupIdx());
+    Column::ChunkState csrOffsetState, csrLengthState;
+    csrHeaderColumns.offset->initChunkState(transaction, csrNodeGroup->getNodeGroupIdx(),
+        csrOffsetState);
+    csrHeaderColumns.length->initChunkState(transaction, csrNodeGroup->getNodeGroupIdx(),
+        csrLengthState);
+    csrHeaderColumns.append(csrNodeGroup->getCSRHeader(), csrOffsetState, csrLengthState);
     for (auto columnID = 0u; columnID < columns.size(); columnID++) {
-        getColumn(columnID)->append(&nodeGroup->getColumnChunkUnsafe(columnID),
-            nodeGroup->getNodeGroupIdx());
+        auto column = getColumn(columnID);
+        Column::ChunkState state;
+        column->initChunkState(&DUMMY_WRITE_TRANSACTION, csrNodeGroup->getNodeGroupIdx(), state);
+        getColumn(columnID)->append(&nodeGroup->getColumnChunkUnsafe(columnID), state);
     }
 }
 
 static length_t getGapSizeForNode(const ChunkedCSRHeader& header, offset_t nodeOffset) {
     return header.getEndCSROffset(nodeOffset) - header.getStartCSROffset(nodeOffset) -
            header.getCSRLength(nodeOffset);
 }
@@ -935,27 +942,27 @@
     commitCSRHeaderChunk(transaction, isNewNodeGroup, nodeGroupIdx, csrHeaderColumns.length.get(),
         newHeader.length.get(), localState, dstOffsets);
 }
 
 void RelTableData::commitCSRHeaderChunk(Transaction* transaction, bool isNewNodeGroup,
     node_group_idx_t nodeGroupIdx, Column* column, ColumnChunk* chunk, LocalState& localState,
     const std::vector<common::offset_t>& dstOffsets) {
+    Column::ChunkState state;
+    column->initChunkState(transaction, nodeGroupIdx, state);
     if (!isNewNodeGroup) {
-        Column::ChunkState state;
-        column->initChunkState(transaction, nodeGroupIdx, state);
         if (column->canCommitInPlace(state, dstOffsets, chunk, localState.region.leftBoundary)) {
             // TODO: We're assuming dstOffsets are consecutive here. This is a bad interface.
             column->write(state, dstOffsets[0], chunk, localState.region.leftBoundary,
                 dstOffsets.size());
             column->getMetadataDA()->update(nodeGroupIdx, state.metadata);
             return;
         }
     }
-    column->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets,
-        chunk, localState.region.leftBoundary);
+    column->commitColumnChunkOutOfPlace(transaction, state, isNewNodeGroup, dstOffsets, chunk,
+        localState.region.leftBoundary);
 }
 
 void RelTableData::distributeOffsets(const ChunkedCSRHeader& header, LocalState& localState,
     offset_t leftBoundary, offset_t rightBoundary) {
     if (localState.region.level > packedCSRInfo.calibratorTreeHeight) {
         // Need to resize the capacity and reset regionToDistribute to the top level one.
         localState.region =
```

### sdist/kuzu-source/src/storage/store/string_column.cpp

```diff
@@ -46,18 +46,18 @@
     if (columnChunk->getNumValues() == 0) {
         return;
     }
     auto stringColumnChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(columnChunk);
     dictionary.scan(transaction, nodeGroupIdx, stringColumnChunk->getDictionaryChunk());
 }
 
-void StringColumn::append(ColumnChunk* columnChunk, node_group_idx_t nodeGroupIdx) {
-    Column::append(columnChunk, nodeGroupIdx);
+void StringColumn::append(ColumnChunk* columnChunk, ChunkState& state) {
+    Column::append(columnChunk, state);
     auto stringColumnChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(columnChunk);
-    dictionary.append(nodeGroupIdx, stringColumnChunk->getDictionaryChunk());
+    dictionary.append(state, stringColumnChunk->getDictionaryChunk());
 }
 
 void StringColumn::writeValue(ChunkState& state, offset_t offsetInChunk,
     ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
     auto& kuStr = vectorToWriteFrom->getValue<ku_string_t>(posInVectorToWriteFrom);
     auto index = dictionary.append(state, kuStr.getAsStringView());
     // Write index to main column
```

### sdist/kuzu-source/src/storage/store/struct_column.cpp

```diff
@@ -110,20 +110,20 @@
     for (auto i = 0u; i < childColumns.size(); i++) {
         auto childData = structData->getChild(i);
         childColumns[i]->write(state.childrenStates[i], offsetInChunk, childData, dataOffset,
             numValues);
     }
 }
 
-void StructColumn::append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) {
-    Column::append(columnChunk, nodeGroupIdx);
+void StructColumn::append(ColumnChunk* columnChunk, ChunkState& state) {
+    Column::append(columnChunk, state);
     KU_ASSERT(columnChunk->getDataType().getPhysicalType() == PhysicalTypeID::STRUCT);
     auto structColumnChunk = static_cast<StructColumnChunk*>(columnChunk);
     for (auto i = 0u; i < childColumns.size(); i++) {
-        childColumns[i]->append(structColumnChunk->getChild(i), nodeGroupIdx);
+        childColumns[i]->append(structColumnChunk->getChild(i), state.childrenStates[i]);
     }
 }
 
 void StructColumn::checkpointInMemory() {
     Column::checkpointInMemory();
     for (const auto& childColumn : childColumns) {
         childColumn->checkpointInMemory();
```

### sdist/kuzu-source/src/storage/wal/wal.cpp

```diff
@@ -11,25 +11,25 @@
 using namespace kuzu::catalog;
 using namespace kuzu::common;
 
 namespace kuzu {
 namespace storage {
 
 WAL::WAL(const std::string& directory, bool readOnly, BufferManager& bufferManager,
-    VirtualFileSystem* vfs)
+    VirtualFileSystem* vfs, main::ClientContext* context)
     : directory{directory}, bufferManager{bufferManager}, vfs{vfs} {
     auto fileInfo =
         vfs->openFile(vfs->joinPath(directory, std::string(StorageConstants::WAL_FILE_SUFFIX)),
-            readOnly ? O_RDONLY : O_CREAT | O_RDWR);
+            readOnly ? O_RDONLY : O_CREAT | O_RDWR, context);
     bufferedWriter = std::make_shared<BufferedFileWriter>(std::move(fileInfo));
     shadowingFH = bufferManager.getBMFileHandle(
         vfs->joinPath(directory, std::string(StorageConstants::SHADOWING_SUFFIX)),
         readOnly ? FileHandle::O_PERSISTENT_FILE_READ_ONLY :
                    FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS,
-        BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs);
+        BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs, context);
 }
 
 WAL::~WAL() {}
 
 page_idx_t WAL::logPageUpdateRecord(DBFileID dbFileID, page_idx_t pageIdxInOriginalFile) {
     lock_t lck{mtx};
     auto pageIdxInWAL = shadowingFH->addNewPage();
```

### sdist/kuzu-source/src/storage/wal_replayer.cpp

```diff
@@ -228,15 +228,15 @@
     case CatalogEntryType::NODE_TABLE_ENTRY:
     case CatalogEntryType::REL_TABLE_ENTRY:
     case CatalogEntryType::REL_GROUP_ENTRY:
     case CatalogEntryType::RDF_GRAPH_ENTRY: {
         clientContext.getCatalog()->dropTableSchema(&DUMMY_WRITE_TRANSACTION, entryID);
         // During recovery, storageManager does not exist.
         if (clientContext.getStorageManager()) {
-            clientContext.getStorageManager()->dropTable(entryID);
+            clientContext.getStorageManager()->dropTable(entryID, clientContext.getVFSUnsafe());
         }
     } break;
     case CatalogEntryType::SEQUENCE_ENTRY: {
         clientContext.getCatalog()->dropSequence(&DUMMY_WRITE_TRANSACTION, entryID);
     } break;
     default: {
         KU_UNREACHABLE;
```

### sdist/kuzu-source/src/storage/wal_replayer_utils.cpp

```diff
@@ -12,20 +12,20 @@
 void WALReplayerUtils::removeHashIndexFile(common::VirtualFileSystem* vfs, table_id_t tableID,
     const std::string& directory) {
     vfs->removeFileIfExists(
         StorageUtils::getNodeIndexFName(vfs, directory, tableID, FileVersionType::ORIGINAL));
 }
 
 void WALReplayerUtils::createEmptyHashIndexFiles(catalog::NodeTableCatalogEntry* nodeTableEntry,
-    const std::string& directory, VirtualFileSystem* vfs) {
+    const std::string& directory, VirtualFileSystem* vfs, main::ClientContext* context) {
     auto pk = nodeTableEntry->getPrimaryKey();
     auto dt = pk->getDataType();
     if (dt->getLogicalTypeID() != LogicalTypeID::SERIAL) {
         PrimaryKeyIndex::createEmptyHashIndexFiles(pk->getDataType()->getPhysicalType(),
             StorageUtils::getNodeIndexFName(vfs, directory, nodeTableEntry->getTableID(),
                 FileVersionType::ORIGINAL),
-            vfs);
+            vfs, context);
     }
 }
 
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/transaction/transaction_manager.cpp

```diff
@@ -40,15 +40,15 @@
     if (transaction->isReadOnly()) {
         activeReadOnlyTransactionIDs.erase(transaction->getID());
         return;
     }
     lastTimestamp++;
     transaction->commitTS = lastTimestamp;
     transaction->commit(&wal);
-    clientContext.getStorageManager()->prepareCommit(transaction);
+    clientContext.getStorageManager()->prepareCommit(transaction, clientContext.getVFSUnsafe());
     wal.flushAllPages();
     clearActiveWriteTransactionIfWriteTransactionNoLock(transaction);
     if (!skipCheckPointing) {
         checkpointNoLock(clientContext);
     }
 }
```

### sdist/kuzu.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuzu
-Version: 0.4.3.dev8
+Version: 0.4.3.dev9
 Summary: An in-process property graph database management system built for query speed and scalability.
 Home-page: https://github.com/kuzudb/kuzu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kuzu Version: 0.4.3.dev8 Summary: An in-process
+Metadata-Version: 2.1 Name: kuzu Version: 0.4.3.dev9 Summary: An in-process
 property graph database management system built for query speed and
 scalability. Home-page: https://github.com/kuzudb/kuzu License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE
                     [https://kuzudb.com/img/kuzu-logo.png]
 
   _[_G_i_t_h_u_b_ _A_c_t_i_o_n_s_ _B_a_d_g_e_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_k_u_z_u_d_b_/_k_u_z_u_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
               _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_N_1_A_T_6_H_7_9_L_M_]_[_d_i_s_c_o_r_d_]_[_t_w_i_t_t_e_r_]
```

### sdist/pyproject.toml

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "kuzu"
 description = "Highly scalable, extremely fast, easy-to-use embeddable graph database"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["graph", "database"]
-version = "0.4.3.dev8"
+version = "0.4.3.dev9"
 
 [project.urls]
 Homepage = "https://kuzudb.com/"
 Documentation = "https://docs.kuzudb.com/"
 Repository = "https://github.com/kuzudb/kuzu"
 Changelog = "https://github.com/kuzudb/kuzu/releases"
```

