# Comparing `tmp/wfl-0.2.7.tar.gz` & `tmp/wfl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfl-0.2.7.tar", last modified: Sun May 19 00:32:42 2024, max compression
+gzip compressed data, was "wfl-0.3.0.tar", last modified: Fri May 24 23:17:02 2024, max compression
```

## Comparing `wfl-0.2.7.tar` & `wfl-0.3.0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.790441 wfl-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-19 00:32:36.000000 wfl-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23587 2024-05-19 00:32:42.790441 wfl-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 00:32:36.000000 wfl-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.762441 wfl-0.2.7/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/cli_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.758441 wfl-0.2.7/deprecated/devtools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/devtools/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8092 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/devtools/scripts/pretty_pca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.758441 wfl-0.2.7/deprecated/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/examples/DFT-calculations/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/examples/DFT-calculations/castep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/examples/DFT-calculations/quantum_espresso.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/examples/DFT-calculations/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/plotting/maxveit_plottools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/plotting/normal_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/plotting/plot_2b.py
--rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/plotting/plot_ef_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/plotting/reactions_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.762441 wfl-0.2.7/deprecated/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/user/reactions/
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/cli_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/cli_reactions_iter_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/user/reactions/generate/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/generate/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/generate/irc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/generate/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/generate/radicals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/generate/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/user/reactions/reactions_processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/reactions_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/reactions_processing/trajectory_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.766441 wfl-0.2.7/deprecated/user/reactions/select/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/select/simple_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/select/weighted_cur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.770441 wfl-0.2.7/deprecated/user/reactions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 00:32:36.000000 wfl-0.2.7/deprecated/user/reactions/tests/test_molecules_radicals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.762441 wfl-0.2.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.770441 wfl-0.2.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-19 00:32:36.000000 wfl-0.2.7/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.762441 wfl-0.2.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.770441 wfl-0.2.7/examples/iterative_gap_fit/
--rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-05-19 00:32:36.000000 wfl-0.2.7/examples/iterative_gap_fit/batch_gap_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-19 00:32:36.000000 wfl-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:32:42.790441 wfl-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.774441 wfl-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_ace_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_atoms_and_dimers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_autoparallelize.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_batch_gap_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_buildcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_calc_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_cli_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_configset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_descriptor_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_doc_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_flat_histo_to_nearby.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_gap_fitting_multistage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_gap_fitting_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_kspacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_mace_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_minimahopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_ndim_neigh_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_neb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_normal_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_outputspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_point_defects.py
--rw-r--r--   0 runner    (1001) docker     (127)    17757 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_remote_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_rng_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_select_greedy_fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_select_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-19 00:32:36.000000 wfl-0.2.7/tests/test_version_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.774441 wfl-0.2.7/wfl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.778441 wfl-0.2.7/wfl/autoparallelize/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/autoparainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/mpipool_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/remoteinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/autoparallelize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.778441 wfl-0.2.7/wfl/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/aims.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/castep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/committee.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/espresso.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/mopac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.778441 wfl-0.2.7/wfl/calculators/orca/
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/orca/basinhopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/calculators/wfl_fileio_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.778441 wfl-0.2.7/wfl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/cli_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.782441 wfl-0.2.7/wfl/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/commands/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/commands/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/commands/select.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5598 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/dft_convergence_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    60870 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/cli/gap_rss_iter_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/configset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/descriptor_heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.782441 wfl-0.2.7/wfl/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/descriptors/quippy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.782441 wfl-0.2.7/wfl/fit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20665 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/ace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21419 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.782441 wfl-0.2.7/wfl/fit/gap/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/gap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/gap/glue_2b.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22213 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/gap/multistage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/gap/relocate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/gap/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/mace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.782441 wfl-0.2.7/wfl/fit/modify_database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/modify_database/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7599 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/modify_database/scale_orig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/modify_database/simple_factor_nonperiodic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5832 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/fit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.786441 wfl-0.2.7/wfl/generate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/atoms_and_dimers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/buildcell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.786441 wfl-0.2.7/wfl/generate/md/
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/md/abort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/md/abort_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/minimahopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/normal_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21142 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/generate/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.786441 wfl-0.2.7/wfl/select/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/select/by_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/select/convex_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/select/flat_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/select/selection_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/select/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.790441 wfl-0.2.7/wfl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/at_copy_save_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/convex_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/find_voids.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/gap_xml_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/julia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/ndim_neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/quip_cli_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/replace_eval_in_strs.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/round_sig_figs.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 00:32:36.000000 wfl-0.2.7/wfl/utils/vol_composition_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:32:42.790441 wfl-0.2.7/wfl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23587 2024-05-19 00:32:42.000000 wfl-0.2.7/wfl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-19 00:32:42.000000 wfl-0.2.7/wfl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:32:42.000000 wfl-0.2.7/wfl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-19 00:32:42.000000 wfl-0.2.7/wfl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 00:32:42.000000 wfl-0.2.7/wfl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 00:32:42.000000 wfl-0.2.7/wfl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.351093 wfl-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-24 23:16:58.000000 wfl-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23587 2024-05-24 23:17:02.351093 wfl-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-24 23:16:58.000000 wfl-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/cli_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.315093 wfl-0.3.0/deprecated/devtools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/devtools/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8092 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/devtools/scripts/pretty_pca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.315093 wfl-0.3.0/deprecated/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/examples/DFT-calculations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/examples/DFT-calculations/castep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/examples/DFT-calculations/quantum_espresso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/examples/DFT-calculations/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/plotting/maxveit_plottools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/plotting/normal_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/plotting/plot_2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/plotting/plot_ef_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/plotting/reactions_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.319093 wfl-0.3.0/deprecated/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/user/reactions/
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/cli_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/cli_reactions_iter_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/user/reactions/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/generate/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/generate/irc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/generate/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/generate/radicals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/generate/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.323093 wfl-0.3.0/deprecated/user/reactions/reactions_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/reactions_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/reactions_processing/trajectory_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.327093 wfl-0.3.0/deprecated/user/reactions/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/select/simple_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/select/weighted_cur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.327093 wfl-0.3.0/deprecated/user/reactions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-24 23:16:58.000000 wfl-0.3.0/deprecated/user/reactions/tests/test_molecules_radicals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.319093 wfl-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.327093 wfl-0.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-24 23:16:58.000000 wfl-0.3.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.319093 wfl-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.327093 wfl-0.3.0/examples/iterative_gap_fit/
+-rw-r--r--   0 runner    (1001) docker     (127)    14955 2024-05-24 23:16:58.000000 wfl-0.3.0/examples/iterative_gap_fit/batch_gap_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-24 23:16:58.000000 wfl-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 23:17:02.351093 wfl-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.331093 wfl-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_ace_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_atoms_and_dimers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_autoparallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_batch_gap_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_buildcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_calc_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_cli_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_configset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_descriptor_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_doc_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_flat_histo_to_nearby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_gap_fitting_multistage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_gap_fitting_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_kspacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_mace_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_minimahopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_ndim_neigh_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_normal_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_outputspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_point_defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17811 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_remote_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_rng_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_select_greedy_fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_select_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-24 23:16:58.000000 wfl-0.3.0/tests/test_version_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.331093 wfl-0.3.0/wfl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.335093 wfl-0.3.0/wfl/autoparallelize/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/autoparainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/mpipool_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/remoteinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/autoparallelize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.339093 wfl-0.3.0/wfl/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/aims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/castep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/committee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/espresso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/mopac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.339093 wfl-0.3.0/wfl/calculators/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/orca/basinhopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/calculators/wfl_fileio_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.339093 wfl-0.3.0/wfl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/cli_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.339093 wfl-0.3.0/wfl/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/commands/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/commands/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/commands/select.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5598 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/dft_convergence_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60906 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/cli/gap_rss_iter_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/configset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/descriptor_heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.339093 wfl-0.3.0/wfl/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/descriptors/quippy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.343093 wfl-0.3.0/wfl/fit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20665 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/ace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21419 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.343093 wfl-0.3.0/wfl/fit/gap/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/gap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/gap/glue_2b.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22213 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/gap/multistage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/gap/relocate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/gap/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/mace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.343093 wfl-0.3.0/wfl/fit/modify_database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/modify_database/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7599 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/modify_database/scale_orig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/modify_database/simple_factor_nonperiodic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5832 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/fit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.347093 wfl-0.3.0/wfl/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/atoms_and_dimers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/buildcell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.347093 wfl-0.3.0/wfl/generate/md/
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/md/abort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/md/abort_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/minimahopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/normal_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21142 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/generate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.347093 wfl-0.3.0/wfl/select/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/select/by_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/select/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/select/flat_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/select/selection_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/select/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.351093 wfl-0.3.0/wfl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/find_voids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/gap_xml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/julia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/ndim_neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/quip_cli_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/replace_eval_in_strs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/round_sig_figs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/save_calc_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-24 23:16:58.000000 wfl-0.3.0/wfl/utils/vol_composition_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:17:02.351093 wfl-0.3.0/wfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23587 2024-05-24 23:17:02.000000 wfl-0.3.0/wfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-24 23:17:02.000000 wfl-0.3.0/wfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:17:02.000000 wfl-0.3.0/wfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 23:17:02.000000 wfl-0.3.0/wfl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 23:17:02.000000 wfl-0.3.0/wfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 23:17:02.000000 wfl-0.3.0/wfl.egg-info/top_level.txt
```

### Comparing `wfl-0.2.7/LICENSE` & `wfl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/PKG-INFO` & `wfl-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfl
-Version: 0.2.7
+Version: 0.3.0
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `wfl-0.2.7/README.md` & `wfl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/cli_plotting.py` & `wfl-0.3.0/deprecated/cli_plotting.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/devtools/scripts/pretty_pca.py` & `wfl-0.3.0/deprecated/devtools/scripts/pretty_pca.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/examples/DFT-calculations/castep.py` & `wfl-0.3.0/deprecated/examples/DFT-calculations/castep.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/examples/DFT-calculations/quantum_espresso.py` & `wfl-0.3.0/deprecated/examples/DFT-calculations/quantum_espresso.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/examples/DFT-calculations/vasp.py` & `wfl-0.3.0/deprecated/examples/DFT-calculations/vasp.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/plotting/maxveit_plottools.py` & `wfl-0.3.0/deprecated/plotting/maxveit_plottools.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/plotting/normal_modes.py` & `wfl-0.3.0/deprecated/plotting/normal_modes.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/plotting/plot_2b.py` & `wfl-0.3.0/deprecated/plotting/plot_2b.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/plotting/plot_ef_correlation.py` & `wfl-0.3.0/deprecated/plotting/plot_ef_correlation.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/plotting/reactions_plotting.py` & `wfl-0.3.0/deprecated/plotting/reactions_plotting.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/cli_cli.py` & `wfl-0.3.0/deprecated/user/reactions/cli_cli.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/cli_reactions_iter_fit.py` & `wfl-0.3.0/deprecated/user/reactions/cli_reactions_iter_fit.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/generate/collision.py` & `wfl-0.3.0/deprecated/user/reactions/generate/collision.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/generate/irc.py` & `wfl-0.3.0/deprecated/user/reactions/generate/irc.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/generate/neb.py` & `wfl-0.3.0/deprecated/user/reactions/generate/neb.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/generate/radicals.py` & `wfl-0.3.0/deprecated/user/reactions/generate/radicals.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/generate/ts.py` & `wfl-0.3.0/deprecated/user/reactions/generate/ts.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/reactions_processing/trajectory_processing.py` & `wfl-0.3.0/deprecated/user/reactions/reactions_processing/trajectory_processing.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/select/simple_filters.py` & `wfl-0.3.0/deprecated/user/reactions/select/simple_filters.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/select/weighted_cur.py` & `wfl-0.3.0/deprecated/user/reactions/select/weighted_cur.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/deprecated/user/reactions/tests/test_molecules_radicals.py` & `wfl-0.3.0/deprecated/user/reactions/tests/test_molecules_radicals.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/docs/source/conf.py` & `wfl-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/examples/iterative_gap_fit/batch_gap_fit.py` & `wfl-0.3.0/examples/iterative_gap_fit/batch_gap_fit.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/pyproject.toml` & `wfl-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "wfl"
-version = "0.2.7"
+version = "0.3.0"
 requires-python = ">=3.9"
 dependencies = [ "click>=7.0", "numpy", "ase>=3.22.1", "pyyaml", "spglib",
                  "docstring_parser", "expyre-wfl", "universalSOAP" ]
 readme = "README.md"
 license = { file = "LICENSE" }
 
 [project.scripts]
```

### Comparing `wfl-0.2.7/tests/test_ace_fitting.py` & `wfl-0.3.0/tests/test_ace_fitting.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_atoms_and_dimers.py` & `wfl-0.3.0/tests/test_atoms_and_dimers.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_autoparallelize.py` & `wfl-0.3.0/tests/test_autoparallelize.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_batch_gap_fit.py` & `wfl-0.3.0/tests/test_batch_gap_fit.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_buildcell.py` & `wfl-0.3.0/tests/test_buildcell.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_calc_descriptor.py` & `wfl-0.3.0/tests/test_calc_descriptor.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_cli_rss.py` & `wfl-0.3.0/tests/test_cli_rss.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_configset.py` & `wfl-0.3.0/tests/test_configset.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_descriptor_heuristics.py` & `wfl-0.3.0/tests/test_descriptor_heuristics.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_doc_examples.py` & `wfl-0.3.0/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_error.py` & `wfl-0.3.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_flat_histo_to_nearby.py` & `wfl-0.3.0/tests/test_flat_histo_to_nearby.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_gap_fitting_multistage.py` & `wfl-0.3.0/tests/test_gap_fitting_multistage.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_gap_fitting_simple.py` & `wfl-0.3.0/tests/test_gap_fitting_simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_kspacing.py` & `wfl-0.3.0/tests/test_kspacing.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_mace_fitting.py` & `wfl-0.3.0/tests/test_mace_fitting.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_map.py` & `wfl-0.3.0/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_md.py` & `wfl-0.3.0/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_minimahopping.py` & `wfl-0.3.0/tests/test_minimahopping.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_molecules.py` & `wfl-0.3.0/tests/test_molecules.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_ndim_neigh_list.py` & `wfl-0.3.0/tests/test_ndim_neigh_list.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_neb.py` & `wfl-0.3.0/tests/test_neb.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_normal_modes.py` & `wfl-0.3.0/tests/test_normal_modes.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_optimize.py` & `wfl-0.3.0/tests/test_optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     print("optimised positions:", atoms_opt.positions)
 
     assert atoms_opt.positions == approx(
         expected_relaxed_positions_constant_pressure, abs=3e-3
     )
 
-    assert atoms_opt.info["config_type"] == "cu_slab_optimize_last_converged"
+    assert atoms_opt.info["config_type"] == "cu_slab:optimize_last_converged"
 
 
 def test_relax_fixed_vol(cu_slab):
 
     calc = EMT()
 
     inputs = ConfigSet(cu_slab)
@@ -172,15 +172,15 @@
         ]
     )
 
     print("optimised positions:", atoms_opt.positions)
 
     assert atoms_opt.positions == approx(expected_positions, abs=3e-3)
 
-    assert atoms_opt.info["config_type"] == "cu_slab_optimize_last_converged"
+    assert atoms_opt.info["config_type"] == "cu_slab:optimize_last_converged"
 
 
 def test_subselect_from_traj(cu_slab):
 
     calc = (EMT, [], {})
 
     cu_slab_optimised = cu_slab.copy()
```

### Comparing `wfl-0.2.7/tests/test_outputspec.py` & `wfl-0.3.0/tests/test_outputspec.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_phonopy.py` & `wfl-0.3.0/tests/test_phonopy.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_point_defects.py` & `wfl-0.3.0/tests/test_point_defects.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_remote_run.py` & `wfl-0.3.0/tests/test_remote_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,19 +270,19 @@
     dt = time.time() - t0
     print('remote parallel calc_time', dt)
 
     # check consistency with local calc
     for at_local, at in zip(ase.io.read(tmp_path / f'ats_o_local_{sys_name}_1.xyz', ':'), ase.io.read(tmp_path / f'ats_o_{sys_name}_1.xyz', ':')):
         assert at_local.info['orig_file'] == at.info['orig_file']
         assert at_local.info['orig_file_seq_no'] == at.info['orig_file_seq_no']
-        assert np.abs((at_local.info['optimize_energy'] - at.info['optimize_energy']) / at_local.info['optimize_energy']) < 1.0e-8
+        assert np.abs((at_local.info['last_op__optimize_energy'] - at.info['last_op__optimize_energy']) / at_local.info['last_op__optimize_energy']) < 1.0e-8
     for at_local, at in zip(ase.io.read(tmp_path / f'ats_o_local_{sys_name}_2.xyz', ':'), ase.io.read(tmp_path / f'ats_o_{sys_name}_2.xyz', ':')):
         assert at_local.info['orig_file'] == at.info['orig_file']
         assert at_local.info['orig_file_seq_no'] == at.info['orig_file_seq_no']
-        assert np.abs((at_local.info['optimize_energy'] - at.info['optimize_energy']) / at_local.info['optimize_energy']) < 1.0e-8
+        assert np.abs((at_local.info['last_op__optimize_energy'] - at.info['last_op__optimize_energy']) / at_local.info['last_op__optimize_energy']) < 1.0e-8
 
 
 def test_fail_immediately(tmp_path, expyre_systems, monkeypatch, remoteinfo_env):
     for sys_name in expyre_systems:
         if sys_name.startswith('_'):
             continue
```

### Comparing `wfl-0.2.7/tests/test_rng_determinism.py` & `wfl-0.3.0/tests/test_rng_determinism.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_select_greedy_fps.py` & `wfl-0.3.0/tests/test_select_greedy_fps.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/tests/test_select_simple.py` & `wfl-0.3.0/tests/test_select_simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/autoparainfo.py` & `wfl-0.3.0/wfl/autoparallelize/autoparainfo.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/base.py` & `wfl-0.3.0/wfl/autoparallelize/base.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/mpipool_support.py` & `wfl-0.3.0/wfl/autoparallelize/mpipool_support.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/pool.py` & `wfl-0.3.0/wfl/autoparallelize/pool.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/remote.py` & `wfl-0.3.0/wfl/autoparallelize/remote.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/remoteinfo.py` & `wfl-0.3.0/wfl/autoparallelize/remoteinfo.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/autoparallelize/utils.py` & `wfl-0.3.0/wfl/autoparallelize/utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/calculators/aims.py` & `wfl-0.3.0/wfl/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/calculators/castep.py` & `wfl-0.3.0/wfl/calculators/castep.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         except Exception as exc:
             atoms.info['DFT_FAILED_CASTEP'] = True
             calculation_succeeded = False
             raise exc
         finally:
             # ASE castep calculator does not ever raise an exception when
             # it fails.  Instead, you get things like stress being None,
-            # which lead to TypeError when save_results calls get_stress().
+            # which lead to TypeError when save_calc_results calls get_stress().
             for property in properties:
                 result = self.get_property(property)
                 if result is None:
                     calculation_succeeded = False
                     atoms.info["DFT_FAILED_CASTEP"] = True
 
             # from WFLFileIOCalculator
```

### Comparing `wfl-0.2.7/wfl/calculators/committee.py` & `wfl-0.3.0/wfl/calculators/committee.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Committee of Models
 
 Calculated properties with a list of models and saves them into info/arrays.
 Further operations (eg. mean, variance, etc.) with these are up to the user.
 """
 from ase import Atoms
 
-from .utils import per_atom_properties, per_config_properties
-from ..utils.misc import atoms_to_list
-from ..utils.parallel import construct_calculator_picklesafe
+from wfl.utils.save_calc_results import per_atom_properties, per_config_properties
+from wfl.utils.misc import atoms_to_list
+from wfl.utils.parallel import construct_calculator_picklesafe
 
 __default_properties = ['energy', 'forces', 'stress']
 
 
 def calculate_committee(atoms, calculator_list, properties=None, output_prefix="committee_{}_"):
     """Calculate energy and forces with a committee of models
```

### Comparing `wfl-0.2.7/wfl/calculators/espresso.py` & `wfl-0.3.0/wfl/calculators/espresso.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 try:
     from ase.calculators.espresso import EspressoProfile
 except ImportError:
     EspressoProfile = None
 from ase.io.espresso import kspacing_to_grid
 
 from .wfl_fileio_calculator import WFLFileIOCalculator
-from .utils import save_results, parse_genericfileio_profile_argv
+from wfl.utils.save_calc_results import save_calc_results
+from .utils import parse_genericfileio_profile_argv
 
 # NOMAD compatible, see https://nomad-lab.eu/prod/rae/gui/uploads
 _default_keep_files = ["*.pwo"]
 _default_properties = ["energy", "forces", "stress"]           # done as "implemented_propertie"
 
 
 class Espresso(WFLFileIOCalculator, ASE_Espresso):
@@ -135,17 +136,17 @@
         self.setup_rundir()
 
         try:
             super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
             calculation_succeeded = True
             if 'DFT_FAILED_ESPRESSO' in atoms.info:
                 del atoms.info['DFT_FAILED_ESPRESSO']
-            if "_output_prefix" in atoms.info:
-                save_results(atoms, properties, atoms.info["_output_prefix"])
-                atoms.info["_results_saved"] = True
+            if "__calculator_output_prefix" in atoms.info:
+                save_calc_results(atoms, prefix=atoms.info["__calculator_output_prefix"], properties=properties)
+                atoms.info["__calculator_results_saved"] = True
         except Exception as exc:
             atoms.info['DFT_FAILED_ESPRESSO'] = True
             calculation_succeeded = False
             raise exc
         finally:
             # from WFLFileIOCalculator
             self.clean_rundir(_default_keep_files, calculation_succeeded)
```

### Comparing `wfl-0.2.7/wfl/calculators/generic.py` & `wfl-0.3.0/wfl/calculators/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ase import Atoms
 from ase.calculators.calculator import all_changes
 
 from wfl.autoparallelize import autoparallelize, autoparallelize_docstring
 from wfl.utils.misc import atoms_to_list
 from wfl.utils.parallel import construct_calculator_picklesafe
-from .utils import save_results
+from wfl.utils.save_calc_results import save_calc_results
 
 
 def _run_autopara_wrappable(atoms, calculator, properties=None, output_prefix='_auto_', verbose=False, raise_calc_exceptions=False):
     """evaluates configs using an arbitrary calculator and store results in info/arrays entries
     or `SinglePointCalculator`.
 
     Defaults to wfl_num_inputs_per_python_subprocess=10, to avoid recreating the calculator for
@@ -128,15 +128,15 @@
 
         # clean up invalid properties, will be fixed in quip Potential soon?
         if hasattr(at.calc, "results") and 'virial' in at.calc.results:
             del at.calc.results['virial']
 
         if calculation_succeeded:
             # this will skip saving if calculator already saved
-            save_results(at, properties_use, output_prefix)
+            save_calc_results(at, prefix=output_prefix, properties=properties_use)
         else:
             # avoid maintaining the reference to the calculator
             at.calc = None
 
         at_out.append(at)
 
     if isinstance(atoms, Atoms):
```

### Comparing `wfl-0.2.7/wfl/calculators/kpts.py` & `wfl-0.3.0/wfl/calculators/kpts.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/calculators/mopac.py` & `wfl-0.3.0/wfl/calculators/mopac.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/calculators/orca/__init__.py` & `wfl-0.3.0/wfl/calculators/orca/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         else:
             self.command = kwargs["command"]
 
         super().__init__(keep_files=keep_files, rundir_prefix=rundir_prefix,
                          workdir=workdir, scratchdir=scratchdir, **kwargs)
 
         self.extra_results = dict()
-        # to make use of wfl.calculators.utils.save_results()
+        # to make use of wfl.utils.save_calc_results.save_calc_results()
         self.extra_results["atoms"] = {}
         self.extra_results["config"] = {}
 
         self.post_process = post_process
 
 
     def calculate(self, atoms=None, properties=["energy", "forces"], system_changes=all_changes):
```

### Comparing `wfl-0.2.7/wfl/calculators/orca/basinhopping.py` & `wfl-0.3.0/wfl/calculators/orca/basinhopping.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/calculators/vasp.py` & `wfl-0.3.0/wfl/calculators/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import numpy as np
 
 from ase.calculators.calculator import all_changes
 from ase.calculators.vasp.vasp import Vasp as ASE_Vasp
 
 from .wfl_fileio_calculator import WFLFileIOCalculator
-from .utils import save_results
+from wfl.utils.save_calc_results import save_calc_results
 from .kpts import universal_kspacing_n_k
 
 from ase.calculators.vasp.create_input import float_keys, exp_keys, string_keys, int_keys, bool_keys
 from ase.calculators.vasp.create_input import list_int_keys, list_bool_keys, list_float_keys, special_keys, dict_keys
 
 
 # NOMAD compatible, see https://nomad-lab.eu/prod/rae/gui/uploads
@@ -251,18 +251,18 @@
                 super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
                 if self.debug: shutil.copy(self._cur_rundir / "OUTCAR", self._cur_rundir / f"OUTCAR.{multi_i}")
                 # restore previous values
                 for k, v in multi_calculation_kwargs_set.items():
                     if self.debug: print("  multi_calculation restoring from prev val", k, prev_vals[k])
                     prev_dicts[k][k] = prev_vals[k]
             calculation_succeeded = True
-            # save results here (if possible) so that save_results() called by calculators.generic
+            # save results here (if possible) so that save_calc_results() called by calculators.generic
             # won't trigger additional calculations due to the ASE caching noticing the change in pbc
             if "__calculator_output_prefix" in atoms.info:
-                save_results(atoms, properties, atoms.info["__calculator_output_prefix"])
+                save_calc_results(atoms, prefix=atoms.info["__calculator_output_prefix"], properties=properties)
                 atoms.info["__calculator_results_saved"] = True
         except Exception as exc:
             atoms.info['DFT_FAILED_VASP'] = True
             raise exc
         finally:
             # from WFLFileIOCalculator
             self.clean_rundir(_default_keep_files, calculation_succeeded)
```

### Comparing `wfl-0.2.7/wfl/calculators/wfl_fileio_calculator.py` & `wfl-0.3.0/wfl/calculators/wfl_fileio_calculator.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/cli.py` & `wfl-0.3.0/wfl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/cli_options.py` & `wfl-0.3.0/wfl/cli/cli_options.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/commands/descriptor.py` & `wfl-0.3.0/wfl/cli/commands/descriptor.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/commands/error.py` & `wfl-0.3.0/wfl/cli/commands/error.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/commands/eval.py` & `wfl-0.3.0/wfl/cli/commands/eval.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/commands/generate.py` & `wfl-0.3.0/wfl/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/commands/select.py` & `wfl-0.3.0/wfl/cli/commands/select.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/dft_convergence_test.py` & `wfl-0.3.0/wfl/cli/dft_convergence_test.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/cli/gap_rss_iter_fit.py` & `wfl-0.3.0/wfl/cli/gap_rss_iter_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
                        traj_select_by_desc_method, descriptor_strs,
                        params.get('global/config_selection_descriptor_local', default=False),
                        prev_GAP, select_convex_hull=params.get('rss_step/select_convex_hull'),
                        get_entire_trajectories=True, optimize_kwargs=params.get('rss_step/optimize_kwargs', {}),
                        rng=ctx.obj['rng'], verbose=verbose)
 
     select_fitting_and_testing_for_groups(run_dir, cur_iter, groups, Params(params.get('rss_step'), cur_iter), Zs,
-                                          'optimize_energy', select_by_desc_method, descriptor_strs,
+                                          'last_op__optimize_energy', select_by_desc_method, descriptor_strs,
                                           params.get('global/config_selection_descriptor_local', default=False),
                                           rng=ctx.obj['rng'], verbose=verbose)
 
     _ = evaluate_iter_and_fit_all(cur_iter, run_dir, params, Params(params.get('rss_step'), cur_iter),
                                   [grp['cur_confs'] for grp in groups.values()],
                                   [grp['testing_confs'] for grp in groups.values()],
                                   params.get('fit/database_modify_mod'),
@@ -799,15 +799,15 @@
                                 temperature=defect_MD_T_range, temperature_tau=10.0 * MD_dt,
                                 pressure=MD_pressure, traj_step_interval=50, rng=ctx.obj['rng'])
 
         groups[grp_label]['cur_confs'] = ConfigSet([bulk_traj, defect_traj])
 
     print_log('selecting by flat histogram + by-descriptor from MD trajectories')
     select_fitting_and_testing_for_groups(
-        run_dir, cur_iter, groups, Params(params.get('MD_bulk_defect_step'), cur_iter), Zs, 'md_energy', select_by_desc_method,
+        run_dir, cur_iter, groups, Params(params.get('MD_bulk_defect_step'), cur_iter), Zs, 'last_op__md_energy', select_by_desc_method,
         descriptor_strs, params.get('global/config_selection_descriptor_local', default=False), rng=ctx.obj['rng'], verbose=verbose)
 
     _ = evaluate_iter_and_fit_all(cur_iter, run_dir, params, Params(params.get('MD_bulk_defect_step'), cur_iter),
                                   [grp['cur_confs'] for grp in groups.values()],
                                   [grp['testing_confs'] for grp in groups.values()],
                                   params.get('fit/database_modify_mod'),
                                   params.get('fit/calc_fitting_error', default=True),
@@ -925,24 +925,24 @@
                                                 lambda at: at.info["optimize_config_type"].startswith("optimize_last"))
 
         if select_convex_hull:
             print_log('selecting convex hull of minima')
             groups[grp_label]['convex_hull'] = wfl.select.convex_hull.select(
                 minima,
                 OutputSpec(f'minima_convex_hull.{grp_label}.xyz', file_root=run_dir),
-                info_field='optimize_energy')
+                info_field='last_op__optimize_energy')
         else:
             groups[grp_label]['convex_hull'] = None
 
         exclude_list = groups[grp_label]['convex_hull']
 
         grp_frac = groups[grp_label]['frac']
         minima_flat_histo_kT = step_params.get('minima_flat_histo_kT', step_params.get('flat_histo_kT'))
         minima_config_by_desc, _ = flat_histo_then_by_desc(
-            run_dir, minima, 'minima', grp_label, Zs, 'optimize_energy', minima_flat_histo_kT,
+            run_dir, minima, 'minima', grp_label, Zs, 'last_op__optimize_energy', minima_flat_histo_kT,
             int(step_params.get('minima_flat_histo_N') * grp_frac), select_by_desc_method,
             config_selection_descriptor_strs, config_selection_descriptor_local,
             int(step_params.get('minima_by_desc_select_N') * grp_frac), testing_N=0,
             vol_range=step_params.get('vol_range', 0.25), compos_range=step_params.get('composition_range', 0.01),
             by_desc_exclude_list=exclude_list, flat_histo_by_bin=step_params.get('flat_histo_by_bin', True),
             flat_histo_replacement=step_params.get('flat_histo_with_replacement', False),
             rng=rng, verbose=verbose)
```

### Comparing `wfl-0.2.7/wfl/configset.py` & `wfl-0.3.0/wfl/configset.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/descriptor_heuristics.py` & `wfl-0.3.0/wfl/descriptor_heuristics.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/descriptors/quippy.py` & `wfl-0.3.0/wfl/descriptors/quippy.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/ace.py` & `wfl-0.3.0/wfl/fit/ace.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/error.py` & `wfl-0.3.0/wfl/fit/error.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/gap/glue_2b.py` & `wfl-0.3.0/wfl/fit/gap/glue_2b.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/gap/multistage.py` & `wfl-0.3.0/wfl/fit/gap/multistage.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/gap/relocate.py` & `wfl-0.3.0/wfl/fit/gap/relocate.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/gap/simple.py` & `wfl-0.3.0/wfl/fit/gap/simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/mace.py` & `wfl-0.3.0/wfl/fit/mace.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,27 +133,27 @@
         xpr.mark_processed()
 
         return results
 
     run_dir.mkdir(parents=True, exist_ok=True)
 
     if valid_configs is not None:
-        valid_configs_scratch_filename = _prep_configs_file(valid_configs, mace_fit_params, "valid_file")
+        valid_configs_scratch_filename = _prep_configs_file(valid_configs, mace_fit_params, "valid_file", workdir=run_dir)
     if test_configs is not None:
-        test_configs_scratch_filename = _prep_configs_file(test_configs, mace_fit_params, "test_file")
+        test_configs_scratch_filename = _prep_configs_file(test_configs, mace_fit_params, "test_file", workdir=run_dir)
 
     if mace_fit_cmd is None:
         if os.environ.get("WFL_MACE_FIT_COMMAND") is not None:
             mace_fit_cmd = os.environ.get("WFL_MACE_FIT_COMMAND")
         elif shutil.which("mace_run_train") is not None:
             mace_fit_cmd = shutil.which("mace_run_train")
         else:
             raise Exception("Path for run_train.py not found.")
 
-    fitting_configs_scratch_filename = _prep_configs_file(fitting_configs, mace_fit_params, "train_file")
+    fitting_configs_scratch_filename = _prep_configs_file(fitting_configs, mace_fit_params, "train_file", workdir=run_dir)
 
     if mace_fit_params.get("foundation_model", None) is not None and Path(mace_fit_params["foundation_model"]).is_file():
         mace_fit_params["foundation_model"] = str(Path(mace_fit_params["foundation_model"]).absolute())
 
     for key, val in mace_fit_params.items():
         if isinstance(val, int) or isinstance(val, float):
             mace_fit_cmd += f" --{key}={val}"
@@ -202,15 +202,15 @@
         print("Failure in calling MACE fitting with error code:", exc.returncode)
         raise exc
 
     if orig_omp_n is not None:
         os.environ["OMP_NUM_THREADS"] = orig_omp_n
 
 
-def _prep_configs_file(configs, use_params, key):
+def _prep_configs_file(configs, use_params, key, workdir=Path()):
     """
     Writes configs to file and updates MACE fitting parameters.
     Configurations and filename handled by Workflow overwrite any filename
     specified in parameters.
 
     Parameters:
     -----------
@@ -224,23 +224,25 @@
     filename
         temporary file name or None if already file is written beforehand
     """
 
     configs_filename = configs.one_file()
 
     if not configs_filename:
-        fd_scratch, filename = tempfile.mkstemp(prefix=f"_MACE_{key}_configs.", suffix=".xyz", dir=".")
+        fd_scratch, filename = tempfile.mkstemp(prefix=str(workdir / f"_MACE_{key}_configs."), suffix=".xyz", dir=".")
         os.close(fd_scratch)
 
         if key in use_params.keys():
             warnings.warn(f"Ignoring configs file '{use_params[key]}' in mace_fit_params, "
                           f"instead using configs passed in and saved to '{filename}'.")
 
         use_params[key] = filename
         ase.io.write(filename, configs)
 
         return filename
 
     else:
-        use_params[key] = configs_filename
+        # make sure this isn't a relative pathname, because the chdir that surrounds actually
+        # running the fit will break it
+        use_params[key] = str(Path(configs_filename).absolute())
 
         return None
```

### Comparing `wfl-0.2.7/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py` & `wfl-0.3.0/wfl/fit/modify_database/gap_rss_set_config_sigmas_from_convex_hull.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/modify_database/scale_orig.py` & `wfl-0.3.0/wfl/fit/modify_database/scale_orig.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/modify_database/simple_factor_nonperiodic.py` & `wfl-0.3.0/wfl/fit/modify_database/simple_factor_nonperiodic.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/fit/utils.py` & `wfl-0.3.0/wfl/fit/utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/atoms_and_dimers.py` & `wfl-0.3.0/wfl/generate/atoms_and_dimers.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/buildcell.py` & `wfl-0.3.0/wfl/generate/buildcell.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/md/__init__.py` & `wfl-0.3.0/wfl/generate/md/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 from ase.md.nvtberendsen import NVTBerendsen
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution, Stationary
 from ase.md.verlet import VelocityVerlet
 from ase.md.langevin import Langevin
 from ase.units import GPa, fs
 
 from wfl.autoparallelize import autoparallelize, autoparallelize_docstring
-from wfl.utils.at_copy_save_results import at_copy_save_results
+from wfl.utils.save_calc_results import at_copy_save_calc_results
 from wfl.utils.misc import atoms_to_list
 from wfl.utils.parallel import construct_calculator_picklesafe
 from wfl.utils.pressure import sample_pressure
-from ..utils import config_type_append
+from ..utils import save_config_type
 
 bar = 1.0e-4 * GPa
 
 
 def _sample_autopara_wrappable(atoms, calculator, steps, dt, integrator="NVTBerendsen", temperature=None, temperature_tau=None,
               pressure=None, pressure_tau=None, compressibility_fd_displ=0.01,
-              traj_step_interval=1, skip_failures=True, results_prefix='md_', verbose=False, update_config_type=True,
+              traj_step_interval=1, skip_failures=True, results_prefix='last_op__md_', verbose=False, update_config_type="append",
               traj_select_during_func=lambda at: True, traj_select_after_func=None, abort_check=None, rng=None,
               _autopara_per_item_info=None):
     """runs an MD trajectory with aggresive, not necessarily physical, integrators for
-    sampling configs
+    sampling configs. By default calculator properties for each frame stored in
+    keys prefixed with "last_op__md_", which may be overwritten by next operation.
 
     Parameters
     ----------
     atoms: list(Atoms)
         input configs
     calculator: Calculator / (initializer, args, kwargs)
         ASE calculator or routine to call to create calculator
@@ -54,19 +55,23 @@
         ignored if pressure is None, defaults to 3*temperature_tau
     compressibility_fd_displ: float, default 0.01
         finite difference in strain to use when computing compressibility for NPTBerendsen
     traj_step_interval: int, default 1
         interval between trajectory snapshots
     skip_failures: bool, default True
         just skip minimizations that raise an exception
+    results_prefix: str, default "last_op__md_"
+        prefix to info/arrays keys where calculator properties will be stored
+        Will overwrite any other properties that start with same "<str>__", so that by
+        default only last op's properties will be stored.
     verbose: bool, default False
         verbose output
         MD logs are not printed unless this is True
-    update_config_type: bool, default True
-        append "MD" to at.info['config_type']
+    update_config_type: ["append" | "overwrite" | False], default "append"
+        whether/how to add 'MD' to at.info['config_type']
     traj_select_during_func: func(Atoms), default func(Atoms) -> bool=True
         Function to sub-select configs from the first trajectory.
         Used during MD loop with one config at a time, returning True/False
     traj_select_after_func: func(list(Atoms)), default None
         Function to sub-select configs from the first trajectory.
         Used at end of MD loop with entire trajectory as list, returns subset
     abort_check: default None,
@@ -201,15 +206,15 @@
 
         def process_step(interval):
             nonlocal cur_step, first_step_of_later_stage
 
             if not first_step_of_later_stage and cur_step % interval == 0:
                 at.info['MD_time_fs'] = cur_step * dt
                 at.info['MD_step'] = cur_step
-                at_save = at_copy_save_results(at, results_prefix=results_prefix)
+                at_save = at_copy_save_calc_results(at, prefix=results_prefix)
 
                 if traj_select_during_func(at):
                     traj.append(at_save)
 
                 if abort_check is not None:
                     if abort_check.stop(at):
                         raise RuntimeError(f"MD was stopped by the MD checker function {abort_check.__class__.__name__}")
@@ -242,23 +247,21 @@
                     break
                 else:
                     raise
 
         if len(traj) == 0 or traj[-1] != at:
             if traj_select_during_func(at):
                 at.info['MD_time_fs'] = cur_step * dt
-                traj.append(at_copy_save_results(at, results_prefix=results_prefix))
+                traj.append(at_copy_save_calc_results(at, prefix=results_prefix))
 
         if traj_select_after_func is not None:
             traj = traj_select_after_func(traj)
 
-        if update_config_type:
-            # save config_type
-            for at in traj:
-                config_type_append(at, 'MD')
+        for at in traj:
+            save_config_type(at, update_config_type, 'MD')
 
         all_trajs.append(traj)
 
     return all_trajs
 
 
 def md(*args, **kwargs):
```

### Comparing `wfl-0.2.7/wfl/generate/md/abort.py` & `wfl-0.3.0/wfl/generate/md/abort.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/md/abort_base.py` & `wfl-0.3.0/wfl/generate/md/abort_base.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/minimahopping.py` & `wfl-0.3.0/wfl/generate/minimahopping.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 import numpy as np
 from ase.optimize.minimahopping import MinimaHopping
 from ase.io.trajectory import Trajectory
 import ase.io
 
 from wfl.autoparallelize import autoparallelize, autoparallelize_docstring
 from wfl.utils.misc import atoms_to_list
-from wfl.generate.utils import config_type_append
+from .utils import save_config_type
 from wfl.utils.parallel import construct_calculator_picklesafe
 
 
-
-def _get_MD_trajectory(rundir):
+def _get_MD_trajectory(rundir, update_config_type):
 
     md_traj = []
     mdtrajfiles = sorted([file for file in Path(rundir).glob("md*.traj")])
     for mdtraj in mdtrajfiles:
         for at in ase.io.read(f"{mdtraj}", ":"):
-            config_type_append(at, 'traj')
+            save_config_type(at, update_config_type, 'minimahop_traj')
             md_traj.append(at)
 
     return md_traj
 
 
 # perform MinimaHopping on one ASE.atoms object
 def _atom_opt_hopping(atom, calculator, Ediff0, T0, minima_threshold, mdmin,
-                     fmax, timestep, totalsteps, skip_failures, workdir=None, **opt_kwargs):
+                     fmax, timestep, totalsteps, skip_failures, update_config_type,
+                     workdir=None, **opt_kwargs):
     save_tmpdir = opt_kwargs.pop("save_tmpdir", False)
     return_all_traj = opt_kwargs.pop("return_all_traj", False)
     origdir = Path.cwd()
     if workdir is None:
         workdir = Path.cwd()
     else:
         workdir = Path(workdir)
@@ -57,31 +57,31 @@
             os.chdir(origdir)
             return None
         else:
             raise
     else:
         traj = []
         if return_all_traj:
-            traj += _get_MD_trajectory(rundir)
+            traj += _get_MD_trajectory(rundir, update_config_type)
 
         for hop_traj in Trajectory('minima.traj'):
-            config_type_append(hop_traj, 'minima')
+            save_config_type(hop_traj, update_config_type, 'minimahop_min')
             traj.append(hop_traj)
         if not save_tmpdir:
             os.chdir(workdir)
             shutil.rmtree(rundir)
         os.chdir(origdir)
         return traj
 
     os.chdir(origdir)
 
 
 def _run_autopara_wrappable(atoms, calculator, Ediff0=1, T0=1000, minima_threshold=0.5, mdmin=2,
-                           fmax=1, timestep=1, totalsteps=10, skip_failures=True, workdir=None,
-                           rng=None, _autopara_per_item_info=None,
+                           fmax=1, timestep=1, totalsteps=10, skip_failures=True, update_config_type="append",
+                           workdir=None, rng=None, _autopara_per_item_info=None,
                            **opt_kwargs):
     """runs a structure optimization
 
     Parameters
     ----------
     atoms: list(Atoms)
         input configs
@@ -99,14 +99,16 @@
         max force for optimizations
     timestep: float, default 1 (fs)
         timestep for MD simulations
     totalsteps: int, default 10
         number of steps
     skip_failures: bool, default True
         just skip optimizations that raise an exception
+    update_config_type: ["append" | "overwrite" | False], default "append"
+        whether/how to add at.info['optimize_config_type'] to at.info['config_type']
     workdir: str/Path default None
         workdir for saving files
     opt_kwargs
         keyword arguments for MinimaHopping
     rng: numpy.random.Generator, default None
         random number generator to use (needed for pressure sampling, initial temperature, or Langevin dynamics)
     _autopara_per_item_info: dict
@@ -125,15 +127,16 @@
         if _autopara_per_item_info is not None:
             # minima hopping doesn't let you pass in a np.random.Generator, so set a global seed using
             # current generator
             np.random.seed(_autopara_per_item_info[at_i]["rng"].integers(2 ** 32))
 
         traj = _atom_opt_hopping(atom=at, calculator=calculator, Ediff0=Ediff0, T0=T0, minima_threshold=minima_threshold,
                                  mdmin=mdmin, fmax=fmax, timestep=timestep, totalsteps=totalsteps,
-                                 skip_failures=skip_failures, workdir=workdir, **opt_kwargs)
+                                 skip_failures=skip_failures, update_config_type=update_config_type,
+                                 workdir=workdir, **opt_kwargs)
         all_trajs.append(traj)
 
     return all_trajs
 
 
 # run that operation on ConfigSet, for multiprocessing
 def minimahopping(*args, **kwargs):
```

### Comparing `wfl-0.2.7/wfl/generate/neb.py` & `wfl-0.3.0/wfl/generate/neb.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import numpy as np
 from ase.optimize import FIRE
 from ase.mep.dyneb import DyNEB
 from ase.atoms import Atoms
 
 from wfl.autoparallelize import autoparallelize, autoparallelize_docstring
-from wfl.utils.at_copy_save_results import at_copy_save_results
+from wfl.utils.save_calc_results import at_copy_save_calc_results
 from wfl.utils.misc import atoms_to_list
 from wfl.utils.parallel import construct_calculator_picklesafe
-from .utils import config_type_append
+from .utils import save_config_type
 
 
 def _run_autopara_wrappable(list_of_images, calculator, fmax=5e-2, steps=1000,
            traj_step_interval=1, traj_subselect=None, skip_failures=True,
-           results_prefix='neb_', verbose=False, logfile=None, update_config_type=True,
+           results_prefix='last_op__neb_', verbose=False, logfile=None, update_config_type="append",
            **neb_kwargs):
-    """runs a structure optimization
+    """runs a structure optimization. By default calculator properties will be stored
+    in keys prefixed with "last_op__neb_", which may be overwritten by next operation.
 
     Parameters
     ----------
     list_of_images: list(iterable(Atoms))
         input list of images, with each is an itereable of Atoms
         (i.e. [images1, images2, images3])
     calculator: Calculator / (initializer, args, kwargs)
@@ -32,19 +33,23 @@
     traj_step_interval: int, default 1
         if present, interval between trajectory snapshots
     traj_subselect: "last_converged", default None
         rule for sub-selecting configs from the full trajectory.
         Currently implemented: "last_converged", which takes the last config, if converged.
     skip_failures: bool, default True
         just skip optimizations that raise an exception
+    results_prefix: str, default "last_op__neb_"
+        prefix to info/arrays keys where calculator properties will be stored
+        Will overwrite any other properties that start with same "<str>__", so that by
+        default only last op's properties will be stored.
     verbose: bool, default False
         verbose output
         optimisation logs are not printed unless this is True
-    update_config_type: bool, default True
-        append at.info['optimize_config_type'] at.info['config_type']
+    update_config_type: ["append" | "overwrite" | False], default "append"
+        whether/how to add at.info['neb_config_type'] to at.info['config_type']
     neb_kwargs
         keyword arguments for DyNEB and FIRE 
 
     Returns
     -------
         list(Atoms) trajectories
     """
@@ -69,15 +74,15 @@
         opt = FIRE(neb, logfile=logfile)
 
         traj = []
         def process_step():
 
             cur_images = []
             for at, constraints in zip(images, orig_constraints):
-                new_config = at_copy_save_results(at, results_prefix=results_prefix)
+                new_config = at_copy_save_calc_results(at, prefix=results_prefix)
                 new_config.set_constraint(constraints)
                 new_config.info['neb_iter_i'] = opt.get_number_of_steps()
                 cur_images.append(new_config)
 
             traj.append(cur_images)
 
         opt.attach(process_step, interval=traj_step_interval)
@@ -111,19 +116,17 @@
             for at in intermed_images:
                 at.info['neb_config_type'] = 'neb_intermediate'
 
         for at in traj[-1]:
             at.info['neb_config_type'] = f'neb_last_{final_status}'
             at.info['neb_n_steps'] = opt.get_number_of_steps()
 
-        if update_config_type:
-            # save config_type
-            for all_images in traj:
-                for at in all_images:
-                    config_type_append(at, at.info['neb_config_type'])
+        for all_images in traj:
+            for at in all_images:
+                save_config_type(at, update_config_type, at.info['neb_config_type'])
 
         traj = subselect_from_traj(traj, subselect=traj_subselect)
 
         all_trajs.append(traj)
 
     return all_trajs
```

### Comparing `wfl-0.2.7/wfl/generate/normal_modes.py` & `wfl-0.3.0/wfl/generate/normal_modes.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/optimize.py` & `wfl-0.3.0/wfl/generate/optimize.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import ase.units
 import numpy as np
 import spglib
 from ase.filters import FrechetCellFilter
 from ase.optimize.precon import PreconLBFGS
 
 from wfl.autoparallelize import autoparallelize, autoparallelize_docstring
-from wfl.utils.at_copy_save_results import at_copy_save_results
+from wfl.utils.save_calc_results import at_copy_save_calc_results
 from wfl.utils.misc import atoms_to_list
 from wfl.utils.parallel import construct_calculator_picklesafe
 from wfl.utils.pressure import sample_pressure
-from .utils import config_type_append
+from .utils import save_config_type
 
 orig_log = PreconLBFGS.log
 
 
 def _new_log(self, forces=None):
     if 'buildcell_config_i' in self.atoms.info:
         if self.logfile is not None:
@@ -29,18 +29,19 @@
 
 
 PreconLBFGS.log = _new_log
 
 
 def _run_autopara_wrappable(atoms, calculator, fmax=1.0e-3, smax=None, steps=1000, pressure=None,
            stress_mask=None, keep_symmetry=True, traj_step_interval=1, traj_subselect=None,
-           skip_failures=True, results_prefix='optimize_', verbose=False, update_config_type=True,
+           skip_failures=True, results_prefix='last_op__optimize_', verbose=False, update_config_type="append",
            rng=None, _autopara_per_item_info=None,
            **opt_kwargs):
-    """runs a structure optimization
+    """runs a structure optimization. By default calculator properties will be stored in keys
+    prefixed with "last_op__optimize_", which may be overwritten by next operation.
 
     Parameters
     ----------
     atoms: list(Atoms)
         input configs
     calculator: Calculator / (initializer, args, kwargs)
         ASE calculator or routine to call to create calculator
@@ -59,19 +60,23 @@
     traj_step_interval: int, default 1
         if present, interval between trajectory snapshots
     traj_subselect: "last_converged", default None
         rule for sub-selecting configs from the full trajectory.
         Currently implemented: "last_converged", which takes the last config, if converged.
     skip_failures: bool, default True
         just skip optimizations that raise an exception
+    results_prefix: str, default "last_op__optimize_"
+        prefix to info/arrays keys where calculator properties will be stored.
+        Will overwrite any other properties that start with same "<str>__", so that by
+        default only last op's properties will be stored.
     verbose: bool, default False
         verbose output
         optimisation logs are not printed unless this is True
-    update_config_type: bool, default True
-        append at.info['optimize_config_type'] at.info['config_type']
+    update_config_type: ["append" | "overwrite" | False], default "append"
+        whether/how to add at.info['optimize_config_type'] to at.info['config_type']
     opt_kwargs
         keyword arguments for PreconLBFGS
     rng: numpy.random.Generator, default None
         random number generator to use (needed for pressure sampling, initial temperature, or Langevin dynamics)
     _autopara_per_item_info: dict
         INTERNALLY used by autoparallelization framework to make runs reproducible (see
         wfl.autoparallelize.autoparallelize() docs)
@@ -142,15 +147,15 @@
 
             if len(traj) > 0 and traj[-1] == at:
                 # Some optimization algorithms sometimes seem to repeat, perhaps
                 # only in weird circumstances, e.g. bad gradients near breakdown.
                 # Do not store those duplicate configs.
                 return
 
-            new_config = at_copy_save_results(at, results_prefix=results_prefix)
+            new_config = at_copy_save_calc_results(at, prefix=results_prefix)
             new_config.set_constraint(org_constraints)
             traj.append(new_config)
 
         opt.attach(process_step, interval=traj_step_interval)
 
         # preliminary value
         final_status = 'unconverged'
@@ -166,15 +171,15 @@
             if skip_failures:
                 sys.stderr.write(f'Structure optimization failed with exception \'{exc}\'\n')
                 sys.stderr.flush()
             else:
                 raise
 
         if len(traj) == 0 or traj[-1] != at:
-            new_config = at_copy_save_results(at, results_prefix=results_prefix)
+            new_config = at_copy_save_calc_results(at, prefix=results_prefix)
             new_config.set_constraint(org_constraints)
             traj.append(new_config)
 
         # set for first config, to be overwritten if it's also last config
         traj[0].info['optimize_config_type'] = 'optimize_initial'
 
         if opt.converged():
@@ -191,18 +196,16 @@
             if dataset is None:
                 print('final symmetry group number None')
             else:
                 print('final symmetry group number {}, international (Hermann-Mauguin) {} Hall {} prec {}'.format(
                     dataset['number'], dataset['international'], dataset['hall'], 0.01))
 
 
-        if update_config_type:
-            # save config_type
-            for at0 in traj:
-                config_type_append(at0, at0.info['optimize_config_type'])
+        for at in traj:
+            save_config_type(at, update_config_type, at.info["optimize_config_type"])
 
         # Note that if resampling doesn't include original last config, later
         # steps won't be able to identify those configs as the (perhaps unconverged) minima.
         # Perhaps status should be set after resampling?
         traj = subselect_from_traj(traj, subselect=traj_subselect)
 
         all_trajs.append(traj)
```

### Comparing `wfl-0.2.7/wfl/generate/phonopy.py` & `wfl-0.3.0/wfl/generate/phonopy.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/smiles.py` & `wfl-0.3.0/wfl/generate/smiles.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/generate/supercells.py` & `wfl-0.3.0/wfl/generate/supercells.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/map.py` & `wfl-0.3.0/wfl/map.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/select/by_descriptor.py` & `wfl-0.3.0/wfl/select/by_descriptor.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/select/convex_hull.py` & `wfl-0.3.0/wfl/select/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/select/flat_histogram.py` & `wfl-0.3.0/wfl/select/flat_histogram.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/select/selection_space.py` & `wfl-0.3.0/wfl/select/selection_space.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/select/simple.py` & `wfl-0.3.0/wfl/select/simple.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/configs.py` & `wfl-0.3.0/wfl/utils/configs.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/convex_hull.py` & `wfl-0.3.0/wfl/utils/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/file_utils.py` & `wfl-0.3.0/wfl/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/find_voids.py` & `wfl-0.3.0/wfl/utils/find_voids.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/gap_xml_tools.py` & `wfl-0.3.0/wfl/utils/gap_xml_tools.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/logging.py` & `wfl-0.3.0/wfl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/misc.py` & `wfl-0.3.0/wfl/utils/misc.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/ndim_neighbor_list.py` & `wfl-0.3.0/wfl/utils/ndim_neighbor_list.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/parallel.py` & `wfl-0.3.0/wfl/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/params.py` & `wfl-0.3.0/wfl/utils/params.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/pressure.py` & `wfl-0.3.0/wfl/utils/pressure.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/quip_cli_strings.py` & `wfl-0.3.0/wfl/utils/quip_cli_strings.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/replace_eval_in_strs.py` & `wfl-0.3.0/wfl/utils/replace_eval_in_strs.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/round_sig_figs.py` & `wfl-0.3.0/wfl/utils/round_sig_figs.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/version.py` & `wfl-0.3.0/wfl/utils/version.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl/utils/vol_composition_space.py` & `wfl-0.3.0/wfl/utils/vol_composition_space.py`

 * *Files identical despite different names*

### Comparing `wfl-0.2.7/wfl.egg-info/PKG-INFO` & `wfl-0.3.0/wfl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfl
-Version: 0.2.7
+Version: 0.3.0
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `wfl-0.2.7/wfl.egg-info/SOURCES.txt` & `wfl-0.3.0/wfl.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 wfl/select/__init__.py
 wfl/select/by_descriptor.py
 wfl/select/convex_hull.py
 wfl/select/flat_histogram.py
 wfl/select/selection_space.py
 wfl/select/simple.py
 wfl/utils/__init__.py
-wfl/utils/at_copy_save_results.py
 wfl/utils/configs.py
 wfl/utils/convex_hull.py
 wfl/utils/file_utils.py
 wfl/utils/find_voids.py
 wfl/utils/gap_xml_tools.py
 wfl/utils/julia.py
 wfl/utils/logging.py
@@ -150,9 +149,10 @@
 wfl/utils/ndim_neighbor_list.py
 wfl/utils/parallel.py
 wfl/utils/params.py
 wfl/utils/pressure.py
 wfl/utils/quip_cli_strings.py
 wfl/utils/replace_eval_in_strs.py
 wfl/utils/round_sig_figs.py
+wfl/utils/save_calc_results.py
 wfl/utils/version.py
 wfl/utils/vol_composition_space.py
```

