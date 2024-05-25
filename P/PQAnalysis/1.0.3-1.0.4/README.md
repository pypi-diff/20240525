# Comparing `tmp/pqanalysis-1.0.3.tar.gz` & `tmp/pqanalysis-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqanalysis-1.0.3.tar", last modified: Thu May 23 15:29:03 2024, max compression
+gzip compressed data, was "pqanalysis-1.0.4.tar", last modified: Sat May 25 11:28:18 2024, max compression
```

## Comparing `pqanalysis-1.0.3.tar` & `pqanalysis-1.0.4.tar`

### file list

```diff
@@ -1,457 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.564074 pqanalysis-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.docstr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.480074 pqanalysis-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/.pylint_cache/
--rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/.pylint_cache/PQAnalysis_1.stats
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/scripts/parse_pylint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 15:29:03.564074 pqanalysis-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.496074 pqanalysis-1.0.3/PQAnalysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.496074 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.496074 pqanalysis-1.0.3/PQAnalysis/atomic_system/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/build_nep_traj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/gen2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/xyz2gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/core/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/atom/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/atom/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/core/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/cell/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/cell/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/residue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/PQ_inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/rules.lark
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/selection.lark
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/terminals.lark
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/box_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/conversion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/energy_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/gen_file/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/info_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/input_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/moldescriptor_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/nep/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/nep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/nep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/nep/nep_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/restart_file/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/topology_file/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/traj_file/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/frame_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/virial/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/virial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/virial/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/virial/virial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/physical_data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/physical_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/physical_data/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/physical_data/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/tools/add_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/topology/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/_topology_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bonded_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/shake_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/traj/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/type_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/PQAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/benchmarks/core/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/benchmarks/core/benchmark_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/benchmarks/core/benchmark_traj_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/benchmarks/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/autodoc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.484073 pqanalysis-1.0.3/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/_templates/package.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.532074 pqanalysis-1.0.3/docs/source/code/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.add_molecules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.continue_input.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.gen2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.rst2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.traj2box.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.xyz2gen.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.atom.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.atom.element.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.cell.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.residue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.box_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.conversion_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.energy_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.info_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.nep.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.virial.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.virial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.write_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.physical_data.energy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.physical_data.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.physical_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.add_molecule.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.shake_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.trajectory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.custom_logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.random.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.units.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.532074 pqanalysis-1.0.3/docs/source/developerGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.532074 pqanalysis-1.0.3/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.536074 pqanalysis-1.0.3/docs/source/userGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/userGuide/inputFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/userGuide/userGuide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.484073 pqanalysis-1.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.536074 pqanalysis-1.0.3/examples/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2box/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.536074 pqanalysis-1.0.3/examples/traj2comtraj/
--rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/pytest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 15:29:03.564074 pqanalysis-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.540074 pqanalysis-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.540074 pqanalysis-1.0.3/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_rdfInputFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_rdfOutputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/atomicSystem/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24372 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/test_atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/test_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/atom/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/atom/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/test_residue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.488074 pqanalysis-1.0.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/data/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_output_files.in
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_start_file.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/input.in
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/input_PQ.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/rdf/input.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/rdf/required_keys_not_given.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readEnergyFile/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readInfoFile/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readMoldescriptor/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readRestartFile/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readRestartFile/md-01.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readRestartFile/moldescriptor.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/rst2xyz/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2box/box.dat
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2box/box.vmd.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2box/test.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.552074 pqanalysis-1.0.3/tests/data/traj2qmcfc/
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.556074 pqanalysis-1.0.3/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.556074 pqanalysis-1.0.3/tests/io/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.556074 pqanalysis-1.0.3/tests/io/inputFileReader/PQ/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_inputDictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_inputFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_boxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_energyFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_frameReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_infoFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_restartReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_restartWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_trajectoryReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_trajectoryWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/physicalData/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/physicalData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/physicalData/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/test_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/topology/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_bondedTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_selectionTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_shakeTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/traj/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/traj/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/traj/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/utils/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/utils/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.816900 pqanalysis-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.docstr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.736901 pqanalysis-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.744901 pqanalysis-1.0.4/.github/.pylint_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/.pylint_cache/PQAnalysis_1.stats
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.744901 pqanalysis-1.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.744901 pqanalysis-1.0.4/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/scripts/parse_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.744901 pqanalysis-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-25 11:28:18.816900 pqanalysis-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.748901 pqanalysis-1.0.4/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.748901 pqanalysis-1.0.4/PQAnalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.748901 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.748901 pqanalysis-1.0.4/PQAnalysis/atomic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/atomic_system/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.752901 pqanalysis-1.0.4/PQAnalysis/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/build_nep_traj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/gen2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/cli/xyz2gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.752901 pqanalysis-1.0.4/PQAnalysis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.752901 pqanalysis-1.0.4/PQAnalysis/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/atom/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.752901 pqanalysis-1.0.4/PQAnalysis/core/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/cell/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/cell/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/core/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.756901 pqanalysis-1.0.4/PQAnalysis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/grammar/PQ_inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/grammar/inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/grammar/rules.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/grammar/selection.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/grammar/terminals.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.756901 pqanalysis-1.0.4/PQAnalysis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/box_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/conversion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/energy_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.756901 pqanalysis-1.0.4/PQAnalysis/io/gen_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/gen_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/gen_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/gen_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/gen_file/gen_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/gen_file/gen_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/info_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.756901 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/input_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.756901 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq/output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.760901 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/moldescriptor_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.760901 pqanalysis-1.0.4/PQAnalysis/io/nep/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/nep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/nep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/nep/nep_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.760901 pqanalysis-1.0.4/PQAnalysis/io/restart_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/restart_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/restart_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/restart_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/restart_file/restart_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/restart_file/restart_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.760901 pqanalysis-1.0.4/PQAnalysis/io/topology_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/topology_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/topology_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/topology_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/topology_file/topology_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/topology_file/topology_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.760901 pqanalysis-1.0.4/PQAnalysis/io/traj_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/traj_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/traj_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/traj_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/traj_file/frame_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/traj_file/trajectory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/traj_file/trajectory_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.760901 pqanalysis-1.0.4/PQAnalysis/io/virial/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/virial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/virial/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/virial/virial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/io/write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.764901 pqanalysis-1.0.4/PQAnalysis/physical_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/physical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/physical_data/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/physical_data/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.764901 pqanalysis-1.0.4/PQAnalysis/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/tools/add_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.764901 pqanalysis-1.0.4/PQAnalysis/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.764901 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/_topology_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/bonded_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/shake_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.764901 pqanalysis-1.0.4/PQAnalysis/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/traj/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/traj/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/PQAnalysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/PQAnalysis/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.816900 pqanalysis-1.0.4/PQAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 11:28:18.000000 pqanalysis-1.0.4/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/benchmarks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/benchmarks/core/benchmark_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/benchmarks/core/benchmark_traj_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/benchmarks/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/autodoc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.740901 pqanalysis-1.0.4/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.768900 pqanalysis-1.0.4/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/_templates/package.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.784901 pqanalysis-1.0.4/docs/source/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rdf.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.add_molecules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.continue_input.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.gen2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.rst2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.traj2box.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.cli.xyz2gen.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.atom.element.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.cell.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.residue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.box_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.conversion_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.energy_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.gen_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.gen_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.info_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.nep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.restart_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.restart_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.topology_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.topology_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.virial.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.virial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.write_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.physical_data.energy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.physical_data.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.physical_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.tools.add_molecule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.shake_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.traj.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.traj.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.traj.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.traj.trajectory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.custom_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.random.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/code/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.784901 pqanalysis-1.0.4/docs/source/developerGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.784901 pqanalysis-1.0.4/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.788900 pqanalysis-1.0.4/docs/source/userGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/userGuide/inputFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/docs/source/userGuide/userGuide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.740901 pqanalysis-1.0.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.788900 pqanalysis-1.0.4/examples/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/examples/traj2box/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.788900 pqanalysis-1.0.4/examples/traj2comtraj/
+-rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-25 11:28:18.816900 pqanalysis-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.792900 pqanalysis-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.792900 pqanalysis-1.0.4/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.796900 pqanalysis-1.0.4/tests/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/analysis/rdf/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/analysis/rdf/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/analysis/rdf/test_rdfInputFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/analysis/rdf/test_rdfOutputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.796900 pqanalysis-1.0.4/tests/atomicSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/atomicSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24372 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/atomicSystem/test_atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/atomicSystem/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/atomicSystem/test_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.796900 pqanalysis-1.0.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/cli/test_continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/cli/test_traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.796900 pqanalysis-1.0.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.796900 pqanalysis-1.0.4/tests/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/core/atom/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/core/atom/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/core/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/core/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.740901 pqanalysis-1.0.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.796900 pqanalysis-1.0.4/tests/data/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/n_not_matching.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/no_output_files.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/no_start_file.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-09.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-10.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/inputFileReader/input_PQ.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/rdf/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/rdf/required_keys_not_given.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/readEnergyFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/readInfoFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/readMoldescriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/readRestartFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readRestartFile/md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/readRestartFile/moldescriptor.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/rst2xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.800900 pqanalysis-1.0.4/tests/data/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/traj2box/box.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/traj2box/box.vmd.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/traj2box/test.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.804901 pqanalysis-1.0.4/tests/data/traj2qmcfc/
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.808900 pqanalysis-1.0.4/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.808900 pqanalysis-1.0.4/tests/io/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/io/inputFileReader/PQ/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/PQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/io/inputFileReader/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/PQAnalysis/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/test_inputDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/test_inputFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/inputFileReader/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_boxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_energyFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_frameReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_infoFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_restartReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_restartWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_trajectoryWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/io/test_write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/physicalData/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/physicalData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/physicalData/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/test_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/bonded_topology/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/bonded_topology/test_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/bonded_topology/test_bondedTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/bonded_topology/test_dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/test_selectionTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/test_shakeTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/topology/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/traj/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/traj/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:28:18.812900 pqanalysis-1.0.4/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-25 11:28:07.000000 pqanalysis-1.0.4/tests/utils/test_decorators.py
```

### Comparing `pqanalysis-1.0.3/.codecov.yml` & `pqanalysis-1.0.4/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/.pylint_cache/PQAnalysis_1.stats` & `pqanalysis-1.0.4/.github/.pylint_cache/PQAnalysis_1.stats`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `pqanalysis-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/scripts/parse_pylint.py` & `pqanalysis-1.0.4/.github/scripts/parse_pylint.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/workflows/ci.yml` & `pqanalysis-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/workflows/docs.yml` & `pqanalysis-1.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/workflows/pylint.yml` & `pqanalysis-1.0.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.github/workflows/release.yml` & `pqanalysis-1.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/.pylintrc` & `pqanalysis-1.0.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/CODE_OF_CONDUCT.md` & `pqanalysis-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/LICENSE` & `pqanalysis-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PKG-INFO` & `pqanalysis-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.3
+Version: 1.0.4
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/__init__.py` & `pqanalysis-1.0.4/PQAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/__init__.py` & `pqanalysis-1.0.4/PQAnalysis/analysis/rdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/api.py` & `pqanalysis-1.0.4/PQAnalysis/analysis/rdf/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/analysis/rdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf.py` & `pqanalysis-1.0.4/PQAnalysis/analysis/rdf/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_input_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/analysis/rdf/rdf_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_output_file_writer.py` & `pqanalysis-1.0.4/PQAnalysis/analysis/rdf/rdf_output_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/atomic_system/_decorators.py` & `pqanalysis-1.0.4/PQAnalysis/atomic_system/_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/atomic_system/_positions.py` & `pqanalysis-1.0.4/PQAnalysis/atomic_system/_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/atomic_system/_properties.py` & `pqanalysis-1.0.4/PQAnalysis/atomic_system/_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/atomic_system/_standard_properties.py` & `pqanalysis-1.0.4/PQAnalysis/atomic_system/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/atomic_system/atomic_system.py` & `pqanalysis-1.0.4/PQAnalysis/atomic_system/atomic_system.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/atomic_system/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/atomic_system/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/_argument_parser.py` & `pqanalysis-1.0.4/PQAnalysis/cli/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/_cli_base.py` & `pqanalysis-1.0.4/PQAnalysis/cli/_cli_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/add_molecules.py` & `pqanalysis-1.0.4/PQAnalysis/cli/add_molecules.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/build_nep_traj.py` & `pqanalysis-1.0.4/PQAnalysis/cli/build_nep_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/continue_input.py` & `pqanalysis-1.0.4/PQAnalysis/cli/continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/gen2xyz.py` & `pqanalysis-1.0.4/PQAnalysis/cli/gen2xyz.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,17 +55,15 @@
 
         Parameters
         ----------
         parser : _ArgumentParser
             The parser to which the arguments should be added.
         """
         parser.add_argument(
-            'gen_file',
-            type=str,
-            help='The gen file to be converted.'
+            'gen_file', type=str, help='The gen file to be converted.'
         )
 
         parser.parse_output_file()
 
         parser.add_argument(
             '--nobox',
             action='store_true',
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/main.py` & `pqanalysis-1.0.4/PQAnalysis/cli/main.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/rdf.py` & `pqanalysis-1.0.4/PQAnalysis/cli/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/rst2xyz.py` & `pqanalysis-1.0.4/PQAnalysis/cli/rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/traj2box.py` & `pqanalysis-1.0.4/PQAnalysis/cli/traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/traj2qmcfc.py` & `pqanalysis-1.0.4/PQAnalysis/cli/traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/cli/xyz2gen.py` & `pqanalysis-1.0.4/PQAnalysis/cli/xyz2gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,31 +51,29 @@
         Adds the arguments to the parser.
 
         Parameters
         ----------
         parser : _ArgumentParser
             The parser to which the arguments should be added.
         """
+        parser.parse_output_file()
+
         parser.add_argument(
             'xyz_file',
             type=str,
-            help='The gen file to be converted.'
+            help='The gen file to be converted.',
         )
 
-        parser.parse_output_file()
-
         parser.add_argument(
-            'periodic',
-            choices=[True,
-            False,
-            None],
+            '--periodic',
+            choices=[True, False, None],
             default=None,
             help=(
-            'If True, the box is printed. If False, the box is not printed. '
-            'If None, the box is printed if it is present in the xyz file.'
+                'If True, the box is printed. If False, the box is not printed. '
+                'If None, the box is printed if it is present in the xyz file.'
             )
         )
 
         parser.parse_engine()
         parser.parse_mode()
 
     @classmethod
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/__init__.py` & `pqanalysis-1.0.4/PQAnalysis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/api.py` & `pqanalysis-1.0.4/PQAnalysis/core/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/atom/atom.py` & `pqanalysis-1.0.4/PQAnalysis/core/atom/atom.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,16 +124,16 @@
             If the name of the atom_type is an integer and the id is given.
         """
 
         if isinstance(name, Element):
             if element_id is not None:
                 self.logger.error(
                     (
-                    "The element of the atom_type cannot be an "
-                    "Element object if the id is given."
+                        "The element of the atom_type cannot be an "
+                        "Element object if the id is given."
                     ),
                     exception=PQValueError
                 )
 
             self._name = name.symbol
             self._element = name
             return
@@ -241,8 +241,8 @@
     @element.setter
     def element(self, element: Element) -> None:
         self._element = element
 
     @property
     def element_name(self) -> str:
         """str: The name of the element (e.g. 'Carbon')"""
-        return self._element.name
+        return self._element.symbol
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/atom/element.py` & `pqanalysis-1.0.4/PQAnalysis/core/atom/element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/cell/_standard_properties.py` & `pqanalysis-1.0.4/PQAnalysis/core/cell/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/cell/cell.py` & `pqanalysis-1.0.4/PQAnalysis/core/cell/cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/core/residue.py` & `pqanalysis-1.0.4/PQAnalysis/core/residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/formats.py` & `pqanalysis-1.0.4/PQAnalysis/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/grammar/inputGrammar.lark` & `pqanalysis-1.0.4/PQAnalysis/grammar/inputGrammar.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/grammar/rules.lark` & `pqanalysis-1.0.4/PQAnalysis/grammar/rules.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/grammar/selection.lark` & `pqanalysis-1.0.4/PQAnalysis/grammar/selection.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/__init__.py` & `pqanalysis-1.0.4/PQAnalysis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/api.py` & `pqanalysis-1.0.4/PQAnalysis/io/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/base.py` & `pqanalysis-1.0.4/PQAnalysis/io/base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/box_writer.py` & `pqanalysis-1.0.4/PQAnalysis/io/box_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/conversion_api.py` & `pqanalysis-1.0.4/PQAnalysis/io/conversion_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         system.cell = Cell()
 
     write_trajectory(
         system,
         output,
         engine_format=md_format,
         traj_type="xyz",
-        mode=mode
+        mode=mode,
     )
 
 
 
 @runtime_type_checking
 def xyz2gen(
     xyz_file: str,
@@ -95,18 +95,23 @@
     md_format : MDEngineFormat | str, optional
         The format of the md engine for the output file. The default is MDEngineFormat.PQ.
     """
 
     system = TrajectoryReader(
         xyz_file,
         md_format=md_format,
-        traj_format="xyz"
+        traj_format="xyz",
     ).read()
 
-    write_gen_file(output, system, periodic, mode)
+    write_gen_file(
+        filename=output,
+        system=system[0],
+        periodic=periodic,
+        mode=mode,
+    )
 
 
 
 @runtime_type_checking
 def rst2xyz(
     restart_file: str,
     output: str | None = None,
@@ -139,19 +144,15 @@
     """
     system = read_restart_file(restart_file)
 
     if not print_box:
         system.cell = Cell()
 
     write_trajectory(
-        system,
-        output,
-        engine_format=md_format,
-        traj_type="xyz",
-        mode=mode
+        system, output, engine_format=md_format, traj_type="xyz", mode=mode
     )
 
 
 
 @runtime_type_checking
 def traj2box(
     trajectory_files: List[str],
@@ -221,17 +222,15 @@
         The writing mode, by default "w". The following modes are available:
         - "w": write
         - "a": append
         - "o": overwrite
     """
 
     writer = TrajectoryWriter(
-        filename=output,
-        engine_format="qmcfc",
-        mode=mode
+        filename=output, engine_format="qmcfc", mode=mode
     )
 
     for filename in trajectory_files:
         reader = TrajectoryReader(filename)
         trajectory = reader.read()
 
         writer.write(trajectory)
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/energy_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/energy_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/formats.py` & `pqanalysis-1.0.4/PQAnalysis/io/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/gen_file/api.py` & `pqanalysis-1.0.4/PQAnalysis/io/gen_file/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,28 +29,29 @@
 
     return GenFileReader(filename).read()
 
 
 
 @runtime_type_checking
 def write_gen_file(
-    filename: str,
     system: AtomicSystem,
+    filename: str | None = None,
     periodic: bool | None = None,
     mode: FileWritingMode | str = "w"
 ) -> None:
     """
     Function to write a gen file.
 
     Parameters
     ----------
-    filename : str
-        The filename of the gen file.
     system : AtomicSystem
         The system to write.
+    filename : str | None, optional
+        The filename of the gen file. If None, the file is not opened, 
+        by default None.
     periodic : bool, optional
         The periodicity of the system. If True, the system is considered periodic. 
         If False, the system is considered non-periodic. If None, the periodicity
         is inferred from the system, by default None.
     mode : FileWritingMode | str, optional
         The writing mode, by default "w". The following modes are available:
         - "w": write
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/gen_file/gen_file_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,32 +48,30 @@
 
         Returns
         -------
         AtomicSystem
             The AtomicSystem including the Cell object.
         """
         with open(self.filename, 'r', encoding='utf-8') as file:
-            lines = file.read_lines()
+            lines = file.readlines()
 
             self.n_atoms, is_periodic, atom_names = self._read_header(lines[:2])
 
             coords, ids = self._read_coords(lines[2:2 + self.n_atoms])
 
             cell = self._read_cell(
                 lines[2 + self.n_atoms:2 + self.n_atoms + 3]
             ) if is_periodic else Cell()
 
             atoms = [Atom(atom_names[id - 1]) for id in ids]
 
             return AtomicSystem(atoms=atoms, pos=coords, cell=cell)
 
     def _read_header(self,
-        header: List[str]) -> Tuple[PositiveInt,
-        bool,
-        List[str]]:
+                     header: List[str]) -> Tuple[PositiveInt, bool, List[str]]:
         """
         Reads the header of the gen file.
 
         The header consists of two lines. The first line contains the number 
         of atoms and the periodicity of the system. The second line contains
         the atom names from which the indices of the atoms in the coordinates 
         block can be derived.
@@ -107,16 +105,15 @@
             )
 
         atom_names = [name.lower() for name in header[1].split()]
 
         return n_atoms, is_periodic, atom_names
 
     def _read_coords(self,
-        lines: List[str]) -> Tuple[Np2DNumberArray,
-        Np1DIntArray]:
+                     lines: List[str]) -> Tuple[Np2DNumberArray, Np1DIntArray]:
         """
         Reads the coordinates block of the gen file.
 
         One line corresponds to one atom and contains a counter index, 
         the atom index and the x, y and z coordinates.
 
         Parameters
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_writer.py` & `pqanalysis-1.0.4/PQAnalysis/io/gen_file/gen_file_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,22 +24,23 @@
 
     logger = logging.getLogger(__package_name__).getChild(__qualname__)
     logger = setup_logger(logger)
 
     @runtime_type_checking
     def __init__(
         self,
-        filename: str,
+        filename: str | None = None,
         mode: FileWritingMode | str = "w",
     ) -> None:
         """
         Parameters
         ----------
-        filename : str
-            The filename of the gen file.
+        filename : str | None, optional
+            The filename of the gen file. If None, the file is not opened,
+            by default None.
         mode : FileWritingMode | str, optional
             The writing mode, by default "w". The following modes are available:
             - "w": write
             - "a": append
             - "o": overwrite
         """
 
@@ -101,15 +102,15 @@
         """
         Writes the header of the gen file.
 
         The header consists of two lines. The first line contains the number of atoms and 
         the periodicity of the system. The second line contains the atom names from which 
         the indices of the atoms in the coordinates block can be derived.
         """
-        print({self.system.n_atoms}, {periodicity}, file=self.file)
+        print(self.system.n_atoms, periodicity, file=self.file)
 
         element_names = self.system.unique_element_names
 
         print(" ".join(element_names), file=self.file)
 
     def _write_coords(self) -> None:
         """
@@ -124,20 +125,17 @@
         """
         element_names = self.system.unique_element_names
         for i in range(self.system.n_atoms):
             print(
                 "\t",
                 i + 1,
                 element_names.index(self.system.atoms[i].element_name) + 1,
-                self.system.pos[i,
-                0],
-                self.system.pos[i,
-                1],
-                self.system.pos[i,
-                2],
+                self.system.pos[i, 0],
+                self.system.pos[i, 1],
+                self.system.pos[i, 2],
                 file=self.file
             )
 
     def _write_box_matrix(self) -> None:
         """
         Writes the box matrix of the system.
 
@@ -149,15 +147,12 @@
         - The z-coordinate of the first box vector
         """
         box_matrix = np.transpose(self.system.cell.box_matrix)
 
         print(0.0, 0.0, 0.0, file=self.file)
         for i in range(3):
             print(
-                box_matrix[i,
-                0],
-                box_matrix[i,
-                1],
-                box_matrix[i,
-                2],
+                box_matrix[i, 0],
+                box_matrix[i, 1],
+                box_matrix[i, 2],
                 file=self.file
             )
```

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/info_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/info_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/formats.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/input_file_parser.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/input_file_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/output_files.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq/output_files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/moldescriptor_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/moldescriptor_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/nep/nep_writer.py` & `pqanalysis-1.0.4/PQAnalysis/io/nep/nep_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/restart_file/api.py` & `pqanalysis-1.0.4/PQAnalysis/io/restart_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/restart_file/restart_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_writer.py` & `pqanalysis-1.0.4/PQAnalysis/io/restart_file/restart_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/topology_file/api.py` & `pqanalysis-1.0.4/PQAnalysis/io/topology_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/topology_file/topology_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_writer.py` & `pqanalysis-1.0.4/PQAnalysis/io/topology_file/topology_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/traj_file/api.py` & `pqanalysis-1.0.4/PQAnalysis/io/traj_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/traj_file/frame_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/traj_file/frame_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/traj_file/trajectory_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_writer.py` & `pqanalysis-1.0.4/PQAnalysis/io/traj_file/trajectory_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/virial/api.py` & `pqanalysis-1.0.4/PQAnalysis/io/virial/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/virial/virial_reader.py` & `pqanalysis-1.0.4/PQAnalysis/io/virial/virial_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/io/write_api.py` & `pqanalysis-1.0.4/PQAnalysis/io/write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/physical_data/energy.py` & `pqanalysis-1.0.4/PQAnalysis/physical_data/energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/tools/add_molecule.py` & `pqanalysis-1.0.4/PQAnalysis/tools/add_molecule.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-1.0.4/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/__init__.py` & `pqanalysis-1.0.4/PQAnalysis/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/api.py` & `pqanalysis-1.0.4/PQAnalysis/topology/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/_topology_properties.py` & `pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/_topology_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/angle.py` & `pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bond.py` & `pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bonded_topology.py` & `pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/bonded_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/dihedral.py` & `pqanalysis-1.0.4/PQAnalysis/topology/bonded_topology/dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/selection.py` & `pqanalysis-1.0.4/PQAnalysis/topology/selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/shake_topology.py` & `pqanalysis-1.0.4/PQAnalysis/topology/shake_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/topology/topology.py` & `pqanalysis-1.0.4/PQAnalysis/topology/topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/traj/api.py` & `pqanalysis-1.0.4/PQAnalysis/traj/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/traj/exceptions.py` & `pqanalysis-1.0.4/PQAnalysis/traj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/traj/formats.py` & `pqanalysis-1.0.4/PQAnalysis/traj/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/traj/trajectory.py` & `pqanalysis-1.0.4/PQAnalysis/traj/trajectory.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/type_checking.py` & `pqanalysis-1.0.4/PQAnalysis/type_checking.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/types.py` & `pqanalysis-1.0.4/PQAnalysis/types.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/utils/common.py` & `pqanalysis-1.0.4/PQAnalysis/utils/common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/utils/custom_logging.py` & `pqanalysis-1.0.4/PQAnalysis/utils/custom_logging.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/utils/decorators.py` & `pqanalysis-1.0.4/PQAnalysis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/utils/files.py` & `pqanalysis-1.0.4/PQAnalysis/utils/files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis/utils/random.py` & `pqanalysis-1.0.4/PQAnalysis/utils/random.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/PQAnalysis.egg-info/PKG-INFO` & `pqanalysis-1.0.4/PQAnalysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.3
+Version: 1.0.4
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pqanalysis-1.0.3/PQAnalysis.egg-info/SOURCES.txt` & `pqanalysis-1.0.4/PQAnalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/README.md` & `pqanalysis-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/benchmarks/core/benchmark_traj_reader.py` & `pqanalysis-1.0.4/benchmarks/core/benchmark_traj_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/Makefile` & `pqanalysis-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/make.bat` & `pqanalysis-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/_templates/module.rst` & `pqanalysis-1.0.4/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/_templates/package.rst` & `pqanalysis-1.0.4/docs/source/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.exceptions.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.atomic_system.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.exceptions.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.api.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.io.traj_file.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.add_molecule.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.tools.add_molecule.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.api.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.topology.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.custom_logging.rst` & `pqanalysis-1.0.4/docs/source/code/PQAnalysis.utils.custom_logging.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/conf.py` & `pqanalysis-1.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/developerGuide/developerGuide.rst` & `pqanalysis-1.0.4/docs/source/developerGuide/developerGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/logo/PQAnalysis.png` & `pqanalysis-1.0.4/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/userGuide/inputFile.rst` & `pqanalysis-1.0.4/docs/source/userGuide/inputFile.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/docs/source/userGuide/userGuide.rst` & `pqanalysis-1.0.4/docs/source/userGuide/userGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0.4/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0.4/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-1.0.4/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/pyproject.toml` & `pqanalysis-1.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -62,11 +62,13 @@
 traj2qmcfc = "PQAnalysis.cli.traj2qmcfc:main"
 rst2xyz = "PQAnalysis.cli.rst2xyz:main"
 continue_input = "PQAnalysis.cli.continue_input:main"
 rdf = "PQAnalysis.cli.rdf:main"
 add_molecules = "PQAnalysis.cli.add_molecules:main"
 activate_argcomplete = "PQAnalysis.cli.activate_argcomplete:main"
 build_nep_traj = "PQAnalysis.cli.build_nep_traj:main"
+xyz2gen = "PQAnalysis.cli.xyz2gen:main"
+gen2xyz = "PQAnalysis.cli.gen2xyz:main"
 
 [project.urls]
 "Homepage" = "https://github.com/MolarVerse/PQAnalysis"
 "PQ" = "https://github.com/MolarVerse/PQ"
```

### Comparing `pqanalysis-1.0.3/tests/analysis/rdf/test_api.py` & `pqanalysis-1.0.4/tests/analysis/rdf/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/analysis/rdf/test_rdf.py` & `pqanalysis-1.0.4/tests/analysis/rdf/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/analysis/rdf/test_rdfInputFileReader.py` & `pqanalysis-1.0.4/tests/analysis/rdf/test_rdfInputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/analysis/rdf/test_rdfOutputFileReader.py` & `pqanalysis-1.0.4/tests/analysis/rdf/test_rdfOutputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/atomicSystem/test_atomic_system.py` & `pqanalysis-1.0.4/tests/atomicSystem/test_atomic_system.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/atomicSystem/test_decorators.py` & `pqanalysis-1.0.4/tests/atomicSystem/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/atomicSystem/test_positions.py` & `pqanalysis-1.0.4/tests/atomicSystem/test_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/cli/test_continue_input.py` & `pqanalysis-1.0.4/tests/cli/test_continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/cli/test_rst2xyz.py` & `pqanalysis-1.0.4/tests/cli/test_rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/cli/test_traj2box.py` & `pqanalysis-1.0.4/tests/cli/test_traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/cli/test_traj2qmcfc.py` & `pqanalysis-1.0.4/tests/cli/test_traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/conftest.py` & `pqanalysis-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/core/atom/test_atom.py` & `pqanalysis-1.0.4/tests/core/atom/test_atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/core/atom/test_element.py` & `pqanalysis-1.0.4/tests/core/atom/test_element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/core/test_cell.py` & `pqanalysis-1.0.4/tests/core/test_cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/core/test_residue.py` & `pqanalysis-1.0.4/tests/core/test_residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/n_not_matching.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_output_files.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/no_output_files.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_start_file.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/no_start_file.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.rpmd.in` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-08.rpmd.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.in.ref` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-09.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.in.ref` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-10.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref` & `pqanalysis-1.0.4/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/readEnergyFile/md-01.info` & `pqanalysis-1.0.4/tests/data/readEnergyFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/readInfoFile/md-01.info` & `pqanalysis-1.0.4/tests/data/readInfoFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-1.0.4/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic.xyz` & `pqanalysis-1.0.4/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic_2.xyz` & `pqanalysis-1.0.4/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/data/traj2qmcfc/traj.qmcfc.xyz` & `pqanalysis-1.0.4/tests/data/traj2qmcfc/traj.qmcfc.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py` & `pqanalysis-1.0.4/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/test_parse.py` & `pqanalysis-1.0.4/tests/io/inputFileReader/PQAnalysis/test_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/inputFileReader/test_inputDictionary.py` & `pqanalysis-1.0.4/tests/io/inputFileReader/test_inputDictionary.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/inputFileReader/test_inputFileParser.py` & `pqanalysis-1.0.4/tests/io/inputFileReader/test_inputFileParser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/inputFileReader/test_transformers.py` & `pqanalysis-1.0.4/tests/io/inputFileReader/test_transformers.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/inputFileReader/test_visitors.py` & `pqanalysis-1.0.4/tests/io/inputFileReader/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_base.py` & `pqanalysis-1.0.4/tests/io/test_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_boxWriter.py` & `pqanalysis-1.0.4/tests/io/test_boxWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_energyFileReader.py` & `pqanalysis-1.0.4/tests/io/test_energyFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_frameReader.py` & `pqanalysis-1.0.4/tests/io/test_frameReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_infoFileReader.py` & `pqanalysis-1.0.4/tests/io/test_infoFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_moldescriptorReader.py` & `pqanalysis-1.0.4/tests/io/test_moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_restartReader.py` & `pqanalysis-1.0.4/tests/io/test_restartReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_restartWriter.py` & `pqanalysis-1.0.4/tests/io/test_restartWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_trajectoryReader.py` & `pqanalysis-1.0.4/tests/io/test_trajectoryReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_trajectoryWriter.py` & `pqanalysis-1.0.4/tests/io/test_trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/io/test_write_api.py` & `pqanalysis-1.0.4/tests/io/test_write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/physicalData/test_energy.py` & `pqanalysis-1.0.4/tests/physicalData/test_energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-1.0.4/tests/tools/test_traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/bonded_topology/test_angle.py` & `pqanalysis-1.0.4/tests/topology/bonded_topology/test_angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/bonded_topology/test_bond.py` & `pqanalysis-1.0.4/tests/topology/bonded_topology/test_bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/bonded_topology/test_bondedTopology.py` & `pqanalysis-1.0.4/tests/topology/bonded_topology/test_bondedTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/bonded_topology/test_dihedral.py` & `pqanalysis-1.0.4/tests/topology/bonded_topology/test_dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/test_selection.py` & `pqanalysis-1.0.4/tests/topology/test_selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/test_selectionTransformer.py` & `pqanalysis-1.0.4/tests/topology/test_selectionTransformer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/test_shakeTopology.py` & `pqanalysis-1.0.4/tests/topology/test_shakeTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/topology/test_topology.py` & `pqanalysis-1.0.4/tests/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/traj/test_api.py` & `pqanalysis-1.0.4/tests/traj/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/traj/test_trajectory.py` & `pqanalysis-1.0.4/tests/traj/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/utils/test_common.py` & `pqanalysis-1.0.4/tests/utils/test_common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.3/tests/utils/test_decorators.py` & `pqanalysis-1.0.4/tests/utils/test_decorators.py`

 * *Files identical despite different names*

