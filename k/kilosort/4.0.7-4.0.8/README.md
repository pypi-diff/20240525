# Comparing `tmp/kilosort-4.0.7.tar.gz` & `tmp/kilosort-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilosort-4.0.7.tar", last modified: Thu May  9 23:07:23 2024, max compression
+gzip compressed data, was "kilosort-4.0.8.tar", last modified: Sat May 25 01:50:09 2024, max compression
```

## Comparing `kilosort-4.0.7.tar` & `kilosort-4.0.8.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.300179 kilosort-4.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.284179 kilosort-4.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.288179 kilosort-4.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/installation_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/other.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.288179 kilosort-4.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-09 23:07:14.000000 kilosort-4.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 23:07:14.000000 kilosort-4.0.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-09 23:07:14.000000 kilosort-4.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 23:07:14.000000 kilosort-4.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-09 23:07:23.300179 kilosort-4.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-09 23:07:14.000000 kilosort-4.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.292179 kilosort-4.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/drift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/gui_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/multi_shank.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.292179 kilosort-4.0.7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/load_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/make_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.296179 kilosort-4.0.7/kilosort/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/CCG.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/clustering_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/datashift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.296179 kilosort-4.0.7/kilosort/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/data_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/header_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21624 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/message_log_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/minor_gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/probe_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/run_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/sanity_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/settings_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    37007 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21027 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/run_kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/swarmsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/template_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/wTEMP.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.300179 kilosort-4.0.7/kilosort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 23:07:14.000000 kilosort-4.0.7/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:07:23.300179 kilosort-4.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-09 23:07:14.000000 kilosort-4.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.300179 kilosort-4.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_full_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 23:07:14.000000 kilosort-4.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.089532 kilosort-4.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.073532 kilosort-4.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.073532 kilosort-4.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-25 01:49:59.000000 kilosort-4.0.8/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-25 01:49:59.000000 kilosort-4.0.8/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-25 01:49:59.000000 kilosort-4.0.8/.github/ISSUE_TEMPLATE/installation_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-25 01:49:59.000000 kilosort-4.0.8/.github/ISSUE_TEMPLATE/other.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.077532 kilosort-4.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-25 01:49:59.000000 kilosort-4.0.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-25 01:49:59.000000 kilosort-4.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-25 01:49:59.000000 kilosort-4.0.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-25 01:49:59.000000 kilosort-4.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 01:49:59.000000 kilosort-4.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-05-25 01:50:09.089532 kilosort-4.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-05-25 01:49:59.000000 kilosort-4.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.077532 kilosort-4.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/drift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/gui_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/multi_shank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.077532 kilosort-4.0.8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/tutorials/basic_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   542612 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/tutorials/kilosort4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/tutorials/load_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/tutorials/make_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 01:49:59.000000 kilosort-4.0.8/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.081532 kilosort-4.0.8/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/CCG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/clustering_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/datashift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.085532 kilosort-4.0.8/kilosort/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/data_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/header_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21624 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/message_log_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/minor_gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/probe_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/run_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/sanity_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33882 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/settings_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/gui/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37330 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23004 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/run_kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/swarmsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/template_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-25 01:49:59.000000 kilosort-4.0.8/kilosort/wTEMP.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.085532 kilosort-4.0.8/kilosort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-05-25 01:50:09.000000 kilosort-4.0.8/kilosort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-25 01:50:09.000000 kilosort-4.0.8/kilosort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:50:09.000000 kilosort-4.0.8/kilosort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-25 01:50:09.000000 kilosort-4.0.8/kilosort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 01:50:09.000000 kilosort-4.0.8/kilosort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 01:49:59.000000 kilosort-4.0.8/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 01:50:09.089532 kilosort-4.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-25 01:49:59.000000 kilosort-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:50:09.085532 kilosort-4.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_full_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-25 01:49:59.000000 kilosort-4.0.8/tests/test_spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-25 01:49:59.000000 kilosort-4.0.8/tox.ini
```

### Comparing `kilosort-4.0.7/.github/ISSUE_TEMPLATE/bug_report.yml` & `kilosort-4.0.8/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 name: Bug report
 description: Report a bug.
-title: "BUG: <Please write a comprehensive title after the 'BUG: ' prefix>"
+title: "BUG: <Please replace this text with a comprehensive title>"
 
 body:
 - type: markdown
   attributes:
     value: >
       Thank you for taking the time to file a bug report. Before creating a new
-      issue, please make sure to take a few minutes to check if this issue has been 
-      brought up before.
+      issue, please take a few minutes to try these steps:
+      1) Check if the issue has already been brought up.
+      2) Try upgrading to the latest version of Kilosort.
+      3) Check relevant pages at kilosort.readthedocs.io
+
+- type: markdown
+  attributes:
+    value: >
+      If the bug occurred during sorting, please also upload the kilosort.log
+      file located in the results directory (v4.0.8 or later).
     
 - type: textarea
   attributes: 
     label: "Describe the issue:"
   validations:
     required: true
 
@@ -31,15 +39,15 @@
       Please include full error message, if any.
     render: shell
 
 - type: textarea
   attributes:
     label: "Version information:"
     description: >
-      Version of operating system and python used, as well as any other
+      Version of python, Kilosort, operating system, and any other
       software versions you think might be relevant to the bug (e.g. CUDA toolkit).
   validations:
     required: true
 
 - type: textarea
   attributes:
     label: "Context for the issue:"
```

### Comparing `kilosort-4.0.7/.github/ISSUE_TEMPLATE/installation_issue.yml` & `kilosort-4.0.8/.github/ISSUE_TEMPLATE/installation_issue.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Installation issue
 description: Report an issue with installation for Kilosort.
-title: "INSTALLATION: <Please write a comprehensive title.>"
+title: "INSTALLATION: <Please replace this text with a comprehensive title>"
 
 body:
     
 - type: textarea
   attributes: 
     label: "Describe the issue:"
     description: >
```

### Comparing `kilosort-4.0.7/.github/workflows/test_and_deploy.yml` & `kilosort-4.0.8/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/.gitignore` & `kilosort-4.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/.readthedocs.yml` & `kilosort-4.0.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/CODE_OF_CONDUCT.md` & `kilosort-4.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/LICENSE` & `kilosort-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/PKG-INFO` & `kilosort-4.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.7
+Version: 4.0.8
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -49,15 +49,15 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/blob/master/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 
 
-You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
+You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available here: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mouseland/kilosort/blob/main/docs/tutorials/kilosort4.ipynb). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
 
 Example notebooks are provided in the `docs/source/tutorials` folder and in the [docs](https://kilosort.readthedocs.io/en/latest/tutorials/tutorials.html). The notebooks include: 
 
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
```

### Comparing `kilosort-4.0.7/README.md` & `kilosort-4.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/blob/master/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 
 
-You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
+You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available here: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mouseland/kilosort/blob/main/docs/tutorials/kilosort4.ipynb). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
 
 Example notebooks are provided in the `docs/source/tutorials` folder and in the [docs](https://kilosort.readthedocs.io/en/latest/tutorials/tutorials.html). The notebooks include: 
 
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
```

### Comparing `kilosort-4.0.7/docs/Makefile` & `kilosort-4.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/conf.py` & `kilosort-4.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/drift.rst` & `kilosort-4.0.8/docs/drift.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/gui_guide.rst` & `kilosort-4.0.8/docs/gui_guide.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/hardware.rst` & `kilosort-4.0.8/docs/hardware.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/index.rst` & `kilosort-4.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/make.bat` & `kilosort-4.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/multi_shank.rst` & `kilosort-4.0.8/docs/multi_shank.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/parameters.rst` & `kilosort-4.0.8/docs/parameters.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/tutorials/basic_example.ipynb` & `kilosort-4.0.8/docs/tutorials/basic_example.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.963638444888445%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'This tutorial is also available as a [collab "*

 * *            "notebook](https://github.com/MouseLand/Kilosort/blob/main/docs/tutorials/kilosort4.ipynb)\\n')], "*

 * *            "delete: [2]}}, 1: {'source': {insert: [(4, 'Downloading the recording may take a few "*

 * *            "minutes. If it fails, please try running the cell again.\\n'), (6, 'You can "*

 * *            'alternatively use any .bin file. See the "Loading other data formats" tutorial for '*

 * *            "loading  […]*

```diff
@@ -3,32 +3,30 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Example spike-sorting analysis with sample data\n",
                 "\n",
-                "This tutorial is also available as a [collab notebook](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing)\n",
+                "This tutorial is also available as a [collab notebook](https://github.com/MouseLand/Kilosort/blob/main/docs/tutorials/kilosort4.ipynb)\n",
                 "if you would like to try Kilosort4 without installing the code locally."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 1. Download example data\n",
                 "\n",
                 "This is an example electrophysiological recording from the International Brain Laboratory, recorded using a Neuropixels 1.0 probe (all data [here](https://ibl.flatironinstitute.org/public/)). The full recording is over 4000 seconds long, and the cropped recording is 90 seconds long.\n",
                 "\n",
-                "Downloading the cropped recording will take around 3 minutes in google colab. If it fails, please try again (press play again), it sometimes hangs.\n",
+                "Downloading the recording may take a few minutes. If it fails, please try running the cell again.\n",
                 "\n",
-                "You can alternatively use any .bin file. See the \"Loading other data formats\" tutorial for loading other file extensions.\n",
-                "\n",
-                "We also used data from Nick Steinmetz, available to download [here](http://data.cortexlab.net/singlePhase3/). For that data use `probe_name='neuropixPhase3A_kilosortChanMap.mat'`."
+                "You can alternatively use any .bin file. See the \"Loading other data formats\" tutorial for loading other file extensions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -48,18 +46,14 @@
                 "            self.total = tsize\n",
                 "        self.update(b * bsize - self.n)\n",
                 "def download_url(url, output_path):\n",
                 "    with DownloadProgressBar(unit='B', unit_scale=True,\n",
                 "                             miniters=1, desc=url.split('/')[-1]) as t:\n",
                 "        urllib.request.urlretrieve(url, filename=output_path, reporthook=t.update_to)\n",
                 "\n",
-                "## FULL DATASET (download locally then decompress)\n",
-                "# compressed using mtscomp (https://github.com/int-brain-lab/mtscomp)\n",
-                "# URL = 'https://ibl.flatironinstitute.org/public/mainenlab/Subjects/ZFM-02370/2021-04-28/001/raw_ephys_data/probe00/_spikeglx_ephysData_g0_t0.imec0.ap.e510da60-53e0-4e00-b369-3ea16c45623a.cbin'\n",
-                "\n",
                 "## CROPPED DATASET\n",
                 "URL = 'http://www.kilosort.org/downloads/ZFM-02370_mini.imec0.ap.bin'\n",
                 "download_url(URL, SAVE_PATH)"
             ]
         },
         {
             "cell_type": "code",
@@ -256,28 +250,33 @@
                 "        ax.axis('off')\n",
                 "    plt.show()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "kilosort",
+            "display_name": "Python 3.9.18 ('kilosort4')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.9.18"
         },
-        "orig_nbformat": 4
+        "orig_nbformat": 4,
+        "vscode": {
+            "interpreter": {
+                "hash": "c450ffd893003221542b409439a3c6dd3d0fae98f595b9e4724fd711cbdc16b9"
+            }
+        }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `kilosort-4.0.7/docs/tutorials/load_data.ipynb` & `kilosort-4.0.8/docs/tutorials/load_data.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/docs/tutorials/make_probe.ipynb` & `kilosort-4.0.8/docs/tutorials/make_probe.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/CCG.py` & `kilosort-4.0.8/kilosort/CCG.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/bench.py` & `kilosort-4.0.8/kilosort/bench.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/clustering_qr.py` & `kilosort-4.0.8/kilosort/clustering_qr.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/datashift.py` & `kilosort-4.0.8/kilosort/datashift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import logging
+logger = logging.getLogger(__name__)
+
 from scipy.sparse import coo_matrix
 import numpy as np
 from scipy.ndimage import gaussian_filter
 import torch
+
 from kilosort import spikedetect
 
+
 def bin_spikes(ops, st):
     """ for each batch, the spikes in that batch are binned to a 2D matrix by amplitude and depth
     """
 
     # the bin edges are based on min and max of channel y positions
     ymin = ops['yc'].min()
     ymax = ops['yc'].max()
@@ -132,15 +137,15 @@
     # upsamples the dot-product matrices by 10 to get finer estimates of vertica ldrift
     dtup = np.linspace(-n,n,2*n*10+1)
 
     # get 1D upsampling matrix
     Kn = kernelD(dt,dtup,1) 
 
     # smooth the dot-product matrices across blocks, batches and across vertical offsets
-    dcs = gaussian_filter(dcs, [0.5, 0.5, 0.5])
+    dcs = gaussian_filter(dcs, ops['drift_smoothing'])
 
     # for each block, upsample the dot-product matrix and find new max
     imin = np.zeros((Nbatches, nblocks))
     for j in range(nblocks):
         dcup = Kn.T @ dcs[:,:,j]
         imax = np.argmax(dcup, 0)
 
@@ -181,15 +186,15 @@
 def run(ops, bfile, device=torch.device('cuda'), progress_bar=None):
     """ this step computes a drift correction model
     it returns vertical correction amplitudes for each batch, and for multiple blocks in a batch if nblocks > 1. 
     """
     
     if ops['nblocks']<1:
         ops['dshift'] = None 
-        print('nblocks = 0, skipping drift correction')
+        logger.info('nblocks = 0, skipping drift correction')
         return ops, None
     
     # the first step is to extract all spikes using the universal templates
     st, _, ops  = spikedetect.run(ops, bfile, device=device, progress_bar=progress_bar)
 
     # spikes are binned by amplitude and y-position to construct a "fingerprint" for each batch
     F, ysamp = bin_spikes(ops, st)
```

### Comparing `kilosort-4.0.7/kilosort/gui/__init__.py` & `kilosort-4.0.8/kilosort/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/converter.py` & `kilosort-4.0.8/kilosort/gui/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,19 +105,22 @@
             " faster.\n However, sorting will be slower and the results will not "
             "be browsable in Phy.\n We recommend using this option to check that "
             "your data is being loaded correctly."
         )
         self.convert_button = QtWidgets.QPushButton('Convert to Binary')
         self.convert_button.clicked.connect(self.convert_to_binary)
         self.convert_input = QtWidgets.QLineEdit()
+        self.convert_input.setPlaceholderText(
+            "NOTE: Must include .bin extension in filename."
+            )
         self.convert_input.setReadOnly(True)
         self.convert_button.setToolTip(
             "'Convert to Binary' will copy the data to a new .bin file.\n"
             "This process is slow for large recordings, but results will be "
-            "browsable in Phy.\n We recommend this option for most use cases."
+            "browsable in Phy.\n We recommend this option for most use cases.\n"
         )
 
         layout.addWidget(self.spacer, 5, 0, 2, 6)
         layout.addWidget(self.wrapper_button, 6, 0, 1, 6)
         layout.addWidget(self.convert_button, 7, 0, 1, 6)
         layout.addWidget(self.convert_input, 7, 6, 1, 10)
```

### Comparing `kilosort-4.0.7/kilosort/gui/data_view_box.py` & `kilosort-4.0.8/kilosort/gui/data_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/header_box.py` & `kilosort-4.0.8/kilosort/gui/header_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/launch.py` & `kilosort-4.0.8/kilosort/gui/launch.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/logger.py` & `kilosort-4.0.8/kilosort/gui/logger.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/main.py` & `kilosort-4.0.8/kilosort/gui/main.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/message_log_box.py` & `kilosort-4.0.8/kilosort/gui/message_log_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/minor_gui_elements.py` & `kilosort-4.0.8/kilosort/gui/minor_gui_elements.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/palettes.py` & `kilosort-4.0.8/kilosort/gui/palettes.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/probe_view_box.py` & `kilosort-4.0.8/kilosort/gui/probe_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/run_box.py` & `kilosort-4.0.8/kilosort/gui/run_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/sanity_plots.py` & `kilosort-4.0.8/kilosort/gui/sanity_plots.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/gui/settings_box.py` & `kilosort-4.0.8/kilosort/gui/settings_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pprint
 from pathlib import Path
 import json
+import ast
 
 import numpy as np
 import torch
 from qtpy import QtCore, QtWidgets, QtGui
 from scipy.io.matlab.miobase import MatReadError
 
 from kilosort.gui.logger import setup_logger
@@ -270,15 +271,21 @@
                 # Use default value
                 d = str(p['default'])
             getattr(self, f'{k}_input').setText(d)
             getattr(self, f'{k}_input').editingFinished.emit()
         for k, p in EXTRA_PARAMETERS.items():
             if self.gui.qt_settings.contains(k):
                 # Use cached value
-                d = str(self.gui.qt_settings.value(k))
+                v = self.gui.qt_settings.value(k)
+                if k == 'drift_smoothing':
+                    # List of floats gets cached as list of strings, so
+                    # have to convert back.
+                    d = str([float(s) for s in v])
+                else:
+                    d = str(v)
             else:
                 # Use default value
                 d = str(p['default'])
             getattr(epw, f'{k}_input').setText(d)
             getattr(epw, f'{k}_input').editingFinished.emit()
 
     @QtCore.Slot()
@@ -425,21 +432,26 @@
 
         except AssertionError:
             logger.exception("Please select a valid binary file path.")
             self.disable_load()
 
     def check_valid_binary_path(self, filename):
         if filename is None:
+            print('Binary path is None.')
             return False
         else:
             f = Path(filename)
             if f.exists() and f.is_file():
                 if f.suffix in _ALLOWED_FILE_TYPES or self.use_file_object:
                     return True
+                else:
+                    print(f'Binary file has invalid suffix. Must be {_ALLOWED_FILE_TYPES}')
+                    return False
             else:
+                print('Binary file does not exist at that path.')
                 return False
 
     def disable_all_input(self, value):
         for button in self.buttons:
             button.setDisabled(value)
         for field in self.input_fields:
             field.setDisabled(value)
@@ -804,15 +816,17 @@
     reset = True
     try:
         value = getattr(sender_obj, f'{k}_input').text()
         if (value is None) or (str(value).lower() == 'none'):
             v = None
         else:
             v = _str_to_type(value, p['type'])
-            if not isinstance(v, bool):
+            if isinstance(v, bool) or isinstance(v, list):
+                pass
+            else:
                 assert v >= p['min']
                 assert v <= p['max']
                 assert v not in p['exclude']
         setattr(sender_obj, k, v)
         main_obj.gui.qt_settings.setValue(k, v)
         reset = False
 
@@ -844,10 +858,12 @@
     if dtype is bool:
         if string.lower() == 'false':
             v = False
         elif string.lower() == 'true':
             v = True
         else:
             raise TypeError(f'{string} should be True or False for bool.')
+    elif dtype is list:
+        v = ast.literal_eval(string)
     else:
         v = dtype(string)
     return v
```

### Comparing `kilosort-4.0.7/kilosort/gui/sorter.py` & `kilosort-4.0.8/kilosort/gui/sorter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import time
+import logging
+logger = logging.getLogger(__name__)
 
 import numpy as np
 import torch
 from qtpy import QtCore
 
-from kilosort.gui.logger import setup_logger
+#from kilosort.gui.logger import setup_logger
 from kilosort.run_kilosort import (
-    initialize_ops, compute_preprocessing, compute_drift_correction,
+    setup_logger, initialize_ops, compute_preprocessing, compute_drift_correction,
     detect_spikes, cluster_spikes, save_sorting
     )
 
-logger = setup_logger(__name__)
+#logger = setup_logger(__name__)
 
 
 class KiloSortWorker(QtCore.QThread):
     finishedPreprocess = QtCore.Signal(object)
     finishedSpikesort = QtCore.Signal(object)
     finishedAll = QtCore.Signal(object)
     progress_bar = QtCore.Signal(int)
@@ -35,17 +37,17 @@
         if "spikesort" in self.steps:
             settings = self.context.params
             probe = self.context.probe
             settings["data_dir"] = self.data_path.parent
             settings["filename"] = self.data_path
             results_dir = self.results_directory
             if not results_dir.exists():
-                logger.info(f"Results dir at {results_dir} does not exist."
-                             "The folder will be created.")
                 results_dir.mkdir(parents=True)
+            
+            setup_logger(results_dir)
 
             tic0 = time.time()
 
             # TODO: make these options in GUI
             do_CAR=True
             invert_sign=False
         
@@ -95,9 +97,8 @@
             self.ops = ops
             self.st = st[kept_spikes]
             self.clu = clu[kept_spikes]
             self.tF = tF[kept_spikes]
             self.is_refractory = is_ref
             self.plotDataReady.emit('probe')
 
-            logger.info(f"Spike sorting output saved in\n{results_dir}")
             self.finishedSpikesort.emit(self.context)
```

### Comparing `kilosort-4.0.7/kilosort/hierarchical.py` & `kilosort-4.0.8/kilosort/hierarchical.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/io.py` & `kilosort-4.0.8/kilosort/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 from pathlib import Path
 from typing import Tuple, Union
 import os, shutil
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 import time
+import logging
+logger = logging.getLogger(__name__)
 
 from scipy.io import loadmat
 import numpy as np
 import torch
 from torch.fft import fft, ifft, fftshift
 
 from kilosort import CCG
@@ -454,16 +456,18 @@
         sample_indices = self._get_shifted_indices(idx)
         # Shift data to pos-only
         if self.dtype == 'uint16':
             data = data + 2**15
             if self.uint_set_warning:
                 # Inform user of shift to hopefully avoid confusion, but only
                 # do this once per bfile.
-                print("NOTE: When setting new values for uint16 data, 2**15 will "
-                      "be added to the given values before writing to file.")
+                logger.info(
+                    "NOTE: When setting new values for uint16 data, 2**15 will "
+                    "be added to the given values before writing to file."
+                    )
                 self.uint_set_warning = False
         # Convert back from float to file dtype
         data = data.astype(self.dtype)
         self.file[sample_indices] = data
         
     def __getitem__(self, *items):
         if self.file is None:
@@ -689,15 +693,15 @@
                 # Skip subsequent preprocessing, zero-out the batch.
                 return torch.zeros_like(X)
 
         # whitening, with optional drift correction
         if self.whiten_mat is not None:
             if self.dshift is not None and ops is not None and ibatch is not None:
                 M = get_drift_matrix(ops, self.dshift[ibatch], device=self.device)
-                #print(M.dtype, X.dtype, self.whiten_mat.dtype)
+                #logger.info(M.dtype, X.dtype, self.whiten_mat.dtype)
                 X = (M @ self.whiten_mat) @ X
             else:
                 X = self.whiten_mat @ X
         return X
 
     def __getitem__(self, *items):
         samples = super().__getitem__(*items)
@@ -764,28 +768,28 @@
     """
 
     filepath = Path(filepath)
     filepath.mkdir(exist_ok=True, parents=True)
     binary_filename = filepath / f'{data_name}'
     probe_filename = filepath / f'{probe_name}'
 
-    print('='*40)
-    print('Loading recording with SpikeInterface...')
+    logger.info('='*40)
+    logger.info('Loading recording with SpikeInterface...')
 
     # Using actual data shape is less fragile than relying on .get_num_channels()
     N = recording.get_total_samples()
-    print(f'number of samples: {N}')
+    logger.info(f'number of samples: {N}')
     c = recording.get_traces(start_frame=0, end_frame=1, segment_index=0).shape[1]
-    print(f'number of channels: {c}')
+    logger.info(f'number of channels: {c}')
     s = recording.get_num_segments()
-    print(f'numbef of segments: {s}')
+    logger.info(f'numbef of segments: {s}')
     fs = recording.get_sampling_frequency()
-    print(f'sampling rate: {fs}')
+    logger.info(f'sampling rate: {fs}')
     dtype = recording.get_dtype()
-    print(f'dtype: {dtype}')
+    logger.info(f'dtype: {dtype}')
 
     # Determine start/end indices for each segment
     indices = []
     for k in range(s):
         n = recording.get_num_samples(segment_index=k)
         i = 0 + k*chunksize
         while i < n:
@@ -799,38 +803,42 @@
         t = recording.get_traces(start_frame=i, end_frame=j, segment_index=k)
         memmap[i:j,:] = t
         memmap.flush()
         del(t)
 
     y = np.memmap(binary_filename, dtype=dtype, mode='w+', shape=(N,c))
     total_chunks = len(indices)
-    print('='*40)
-    print(f'Converting {total_chunks} data chunks '
-          f'with a chunksize of {chunksize} samples...')
+    logger.info('='*40)
+    logger.info(
+        f'Converting {total_chunks} data chunks '
+        f'with a chunksize of {chunksize} samples...'
+        )
     with ThreadPoolExecutor(max_workers=max_workers) as exe:
         futures = [exe.submit(copy_chunk, y, i, j, k) for i, j, k in indices]
         # TODO: every some-amount-of-time, check list of futures
         #       for completion
         while exe._work_queue.qsize() > 0:
             time.sleep(10)
-            print(f'{total_chunks - exe._work_queue.qsize()} of {total_chunks}'
-                   ' chunks converted...')
-    print(f'Data conversion finished.')
-    print('='*40)
+            logger.info(
+                f'{total_chunks - exe._work_queue.qsize()} of {total_chunks}'
+                ' chunks converted...'
+                )
+    logger.info(f'Data conversion finished.')
+    logger.info('='*40)
 
     del(y)  # Close memmap after copying
 
     if export_probe:
         try:
             from probeinterface import write_prb
             try:
                 pg = recording.get_probegroup()
                 write_prb(probe_filename, pg)
             except ValueError:
-                print(
+                logger.info(
                     'SpikeInterface recording contains no probe information,\n'
                     'could not write .prb file.'
                 )
                 probe_filename = None
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
                 'Could not import `write_prb` from probeinterface when exporting '
@@ -882,38 +890,40 @@
 
         """
 
         if recording_extractor.get_num_segments() > 1:
             try:
                 import spikeinterface as si
                 self.recording = si.concatenate_recordings([recording_extractor])
-                print('SpikeInterface recording contains more than one segment, '
-                      'segments will be concatenated as if contiguous.')
+                logger.info(
+                    'SpikeInterface recording contains more than one segment, '
+                    'segments will be concatenated as if contiguous.'
+                    )
             except ModuleNotFoundError:
                 raise ModuleNotFoundError(
                     'SpikeInterface could not be imported, but is needed for '
                     'loading multi-segment SpikeInterface recordings. Please '
                     'run `pip install spikeinterface`.'
                 )
 
-        print('='*40)
-        print('Loading recording with SpikeInterface...')
+        logger.info('='*40)
+        logger.info('Loading recording with SpikeInterface...')
         self.recording = recording_extractor
         self.N = self.recording.get_total_samples()
-        print(f'number of samples: {self.N}')
+        logger.info(f'number of samples: {self.N}')
         self.c = self.recording.get_traces(start_frame=0, end_frame=1, segment_index=0).shape[1]
-        print(f'number of channels: {self.c}')
+        logger.info(f'number of channels: {self.c}')
         self.s = self.recording.get_num_segments()
-        print(f'numbef of segments: {self.s}')
+        logger.info(f'numbef of segments: {self.s}')
         self.fs = self.recording.get_sampling_frequency()
-        print(f'sampling rate: {self.fs}')
+        logger.info(f'sampling rate: {self.fs}')
         self.dtype = self.recording.get_dtype()
-        print(f'dtype: {self.dtype}')
+        logger.info(f'dtype: {self.dtype}')
         self.shape = (self.N, self.c)
-        print('='*40)
+        logger.info('='*40)
     
 
     def __getitem__(self, *items):
         idx, *crop = items
         if not isinstance(idx, tuple): idx = tuple([idx])
         sample_idx = idx[0]
         channel_ids = None if len(idx) == 1 else idx[1]
```

### Comparing `kilosort-4.0.7/kilosort/parameters.py` & `kilosort-4.0.8/kilosort/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,27 @@
     },
 
     'sig_interp': {
         'gui_name': 'sig_interp', 'type': float, 'min': 0, 'max': np.inf,
         'exclude': [0], 'default': 20, 'step': 'preprocessing',
         'description':
             """
-            For drift correction, sigma for interpolation (spatial standard
-            deviation). Approximate smoothness scale in units of microns.
+            Approximate spatial smoothness scale in units of microns.
+            """
+    },
+
+    'drift_smoothing': {
+        'gui_name': 'drift smoothing', 'type': list, 'min': None, 'max': None,
+        'exclude': [], 'default': [0.5, 0.5, 0.5], 'step': 'preprocessing',
+        'description':
+            """
+            Amount of gaussian smoothing to apply to the spatiotemporal drift
+            estimation, for x,y,time axes in units of registration blocks
+            (for x,y axes) and batch size (for time axis). The x,y smoothing has
+            no effect for `nblocks = 1`.
             """
     },
 
 
     ### SPIKE DETECTION
     # NOTE: if left as None, will be set to `int(20 * settings['nt']/61)`
     'nt0min': {
```

### Comparing `kilosort-4.0.7/kilosort/postprocessing.py` & `kilosort-4.0.8/kilosort/postprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/preprocessing.py` & `kilosort-4.0.8/kilosort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/run_kilosort.py` & `kilosort-4.0.8/kilosort/run_kilosort.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import time
 from pathlib import Path
+import logging
+logger = logging.getLogger(__name__)
 
 import numpy as np
 import torch
 
 from kilosort import (
     preprocessing,
     datashift,
@@ -86,53 +88,57 @@
     Returns
     -------
     ops, st, clu, tF, Wall, similar_templates, is_ref, est_contam_rate
         Description TODO
 
     """
 
-    if not do_CAR:
-        print("Skipping common average reference.")
-
-    tic0 = time.time()
-
     # Configure settings, ops, and file paths
     if settings is None or settings.get('n_chan_bin', None) is None:
         raise ValueError(
             '`n_chan_bin` is a required setting. This is the total number of '
             'channels in the binary file, which may or may not be equal to the '
             'number of channels specified by the probe.'
             )
     settings = {**DEFAULT_SETTINGS, **settings}
+    # NOTE: This modifies settings in-place
+    filename, data_dir, results_dir, probe = \
+        set_files(settings, filename, probe, probe_name, data_dir, results_dir)
+    setup_logger(results_dir)
+    logger.info(f"Sorting {filename}")
+    logger.info('-'*40)
 
     if data_dtype is None:
-        print("Interpreting binary file as default dtype='int16'. If data was "
-                "saved in a different format, specify `data_dtype`.")
+        logger.info(
+            "Interpreting binary file as default dtype='int16'. If data was "
+            "saved in a different format, specify `data_dtype`."
+            )
+
+    if not do_CAR:
+        logger.info("Skipping common average reference.")
 
     if device is None:
         if torch.cuda.is_available():
-            print('Using GPU for PyTorch computations. '
-                  'Specify `device` to change this.')
+            logger.info('Using GPU for PyTorch computations. '
+                        'Specify `device` to change this.')
             device = torch.device('cuda')
         else:
-            print('Using CPU for PyTorch computations. '
-                  'Specify `device` to change this.')
+            logger.info('Using CPU for PyTorch computations. '
+                        'Specify `device` to change this.')
             device = torch.device('cpu')
 
-    # NOTE: Also modifies settings in-place
-    filename, data_dir, results_dir, probe = \
-        set_files(settings, filename, probe, probe_name, data_dir, results_dir)
-    ops = initialize_ops(settings, probe, data_dtype, do_CAR, invert_sign, device)
-
     if probe['chanMap'].max() >= settings['n_chan_bin']:
         raise ValueError(
             f'Largest value of chanMap exceeds channel count of data, '
              'make sure chanMap is 0-indexed.'
         )
 
+    tic0 = time.time()
+    ops = initialize_ops(settings, probe, data_dtype, do_CAR, invert_sign, device)
+
     # Set preprocessing and drift correction parameters
     ops = compute_preprocessing(ops, device, tic0=tic0, file_object=file_object)
     np.random.seed(1)
     torch.cuda.manual_seed_all(1)
     torch.random.manual_seed(1)
     ops, bfile, st0 = compute_drift_correction(
         ops, device, tic0=tic0, progress_bar=progress_bar,
@@ -169,49 +175,76 @@
             raise ValueError('no path to data provided, set "data_dir=" or "filename="')
         data_dir = Path(data_dir).resolve()
         if not data_dir.exists():
             raise FileExistsError(f"data_dir '{data_dir}' does not exist")
 
         # Find binary file in the folder
         filename  = io.find_binary(data_dir=data_dir)
-        print(f"sorting {filename}")
     else:
         filename = Path(filename)
         if not filename.exists():
             raise FileExistsError(f"filename '{filename}' does not exist")
         data_dir = filename.parent
         
     # Convert paths to strings when saving to ops, otherwise ops can only
     # be loaded on the operating system that originally ran the code.
     settings['filename'] = filename
     settings['data_dir'] = data_dir
 
+    # Try to set results_dir based on settings, otherwise use default.
     results_dir = settings.get('results_dir', None) if results_dir is None else results_dir
     results_dir = Path(results_dir).resolve() if results_dir is not None else None
+    if results_dir is None:
+        results_dir = data_dir / 'kilosort4'
     
     # find probe configuration file and load
     if probe is None:
         if probe_name is not None:     probe_path = PROBE_DIR / probe_name
         elif 'probe_name' in settings: probe_path = PROBE_DIR / settings['probe_name']
         elif 'probe_path' in settings: probe_path = Path(settings['probe_path']).resolve()
         else: raise ValueError('no probe_name or probe_path provided, set probe_name=')
         if not probe_path.exists():
             raise FileExistsError(f"probe_path '{probe_path}' does not exist")
         
         probe  = io.load_probe(probe_path)
-        print(f"using probe {probe_path.name}")
     else:
         # Make sure xc, yc are float32, otherwise there are casting problems
         # with some pytorch functions.
         probe['xc'] = probe['xc'].astype(np.float32)
         probe['yc'] = probe['yc'].astype(np.float32)
 
     return filename, data_dir, results_dir, probe
 
 
+def setup_logger(results_dir):
+    # Adapted from
+    # https://docs.python.org/2/howto/logging-cookbook.html#logging-to-multiple-destinations
+    # In summary: only send logging.debug statements to log file, not console.
+
+    # set up logging to file for root logger
+    logging.basicConfig(level=logging.DEBUG,
+                        format='%(asctime)s %(name)-12s %(levelname)-8s %(message)s',
+                        datefmt='%m-%d %H:%M',
+                        filename=results_dir/'kilosort4.log',
+                        filemode='w')
+
+    # define a Handler which writes INFO messages or higher to the sys.stderr
+    console = logging.StreamHandler()
+    console.setLevel(logging.INFO)
+    # set a format which is simpler for console use
+    console_formatter = logging.Formatter('%(name)-12s: %(message)s')
+    console.setFormatter(console_formatter)
+    # add the console handler to the root logger
+    logging.getLogger('').addHandler(console)
+
+    # Set numba logger to INFO or above only, so that it doesn't spam the log file
+    numba_log = logging.getLogger('numba')
+    numba_log.setLevel(logging.INFO)
+
+
 def initialize_ops(settings, probe, data_dtype, do_CAR, invert_sign, device) -> dict:
     """Package settings and probe information into a single `ops` dictionary."""
 
     if settings['nt0min'] is None:
         settings['nt0min'] = int(20 * settings['nt']/61)
     # TODO: Clean this up during refactor. Lots of confusing duplication here.
     ops = settings  
@@ -275,14 +308,18 @@
     Returns
     -------
     ops : dict
     
     """
 
     tic = time.time()
+    logger.info(' ')
+    logger.info('Computing preprocessing variables.')
+    logger.info('-'*40)
+
     n_chan_bin, fs, NT, nt, twav_min, chan_map, dtype, do_CAR, invert, \
         xc, yc, tmin, tmax, artifact = get_run_parameters(ops)
     nskip = ops['settings']['nskip']
     whitening_range = ops['settings']['whitening_range']
     
     # Compute high pass filter
     hp_filter = preprocessing.get_highpass_filter(ops['settings']['fs'], device=device)
@@ -301,16 +338,16 @@
     ops['Nbatches'] = bfile.n_batches
     ops['preprocessing'] = {}
     ops['preprocessing']['whiten_mat'] = whiten_mat
     ops['preprocessing']['hp_filter'] = hp_filter
     ops['Wrot'] = whiten_mat
     ops['fwav'] = hp_filter
 
-    print(f'Preprocessing filters computed in {time.time()-tic : .2f}s; ' +
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'Preprocessing filters computed in {time.time()-tic : .2f}s; ' +
+                f'total {time.time()-tic0 : .2f}s')
 
     return ops
 
 
 def compute_drift_correction(ops, device, tic0=np.nan, progress_bar=None,
                              file_object=None):
     """Compute drift correction parameters and save them to `ops`.
@@ -334,15 +371,17 @@
     -------
     ops : dict
     bfile : kilosort.io.BinaryFiltered
         Wrapped file object for handling data.
     
     """
     tic = time.time()
-    print('\ncomputing drift')
+    logger.info(' ')
+    logger.info('Computing drift correction.')
+    logger.info('-'*40)
 
     n_chan_bin, fs, NT, nt, twav_min, chan_map, dtype, do_CAR, invert, \
         _, _, tmin, tmax, artifact = get_run_parameters(ops)
     hp_filter = ops['preprocessing']['hp_filter']
     whiten_mat = ops['preprocessing']['whiten_mat']
 
     bfile = io.BinaryFiltered(
@@ -350,16 +389,16 @@
         hp_filter=hp_filter, whiten_mat=whiten_mat, device=device, do_CAR=do_CAR,
         invert_sign=invert, dtype=dtype, tmin=tmin, tmax=tmax,
         artifact_threshold=artifact, file_object=file_object
         )
 
     ops, st = datashift.run(ops, bfile, device=device, progress_bar=progress_bar)
     bfile.close()
-    print(f'drift computed in {time.time()-tic : .2f}s; ' + 
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'drift computed in {time.time()-tic : .2f}s; ' + 
+                f'total {time.time()-tic0 : .2f}s')
     
     # binary file with drift correction
     bfile = io.BinaryFiltered(
         ops['filename'], n_chan_bin, fs, NT, nt, twav_min, chan_map, 
         hp_filter=hp_filter, whiten_mat=whiten_mat, device=device,
         dshift=ops['dshift'], do_CAR=do_CAR, dtype=dtype, tmin=tmin, tmax=tmax,
         artifact_threshold=artifact, file_object=file_object
@@ -395,63 +434,71 @@
         TODO
     Wall : np.ndarray
         TODO
 
     """
 
     tic = time.time()
-    print(f'\nExtracting spikes using templates')
+    logger.info(' ')
+    logger.info(f'Extracting spikes using templates')
+    logger.info('-'*40)
     st0, tF, ops = spikedetect.run(ops, bfile, device=device, progress_bar=progress_bar)
     tF = torch.from_numpy(tF)
-    print(f'{len(st0)} spikes extracted in {time.time()-tic : .2f}s; ' + 
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'{len(st0)} spikes extracted in {time.time()-tic : .2f}s; ' + 
+                f'total {time.time()-tic0 : .2f}s')
     if len(st0) == 0:
         raise ValueError('No spikes detected, cannot continue sorting.')
 
     tic = time.time()
-    print('\nFirst clustering')
+    logger.info(' ')
+    logger.info('First clustering')
+    logger.info('-'*40)
     clu, Wall = clustering_qr.run(ops, st0, tF, mode='spikes', device=device,
                                   progress_bar=progress_bar)
     Wall3 = template_matching.postprocess_templates(Wall, ops, clu, st0, device=device)
-    print(f'{clu.max()+1} clusters found, in {time.time()-tic : .2f}s; ' +
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'{clu.max()+1} clusters found, in {time.time()-tic : .2f}s; ' +
+                f'total {time.time()-tic0 : .2f}s')
     
     tic = time.time()
-    print('\nExtracting spikes using cluster waveforms')
+    logger.info(' ')
+    logger.info('Extracting spikes using cluster waveforms')
+    logger.info('-'*40)
     st, tF, ops = template_matching.extract(ops, bfile, Wall3, device=device,
                                                  progress_bar=progress_bar)
-    print(f'{len(st)} spikes extracted in {time.time()-tic : .2f}s; ' +
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'{len(st)} spikes extracted in {time.time()-tic : .2f}s; ' +
+                f'total {time.time()-tic0 : .2f}s')
 
     negative_spikes = (st[:,0] < 0).sum()
     if negative_spikes > 0:
-        print(
-            f'{negative_spikes} spikes with negative spike times were detected.\n'
-            'We are aware of an issue causing this to happen for a small number '
-            'of spikes, and are working on a fix.'
-            )
+        logger.info(f'{negative_spikes} spikes with negative times were detected.')
+        logger.info('We are aware of an issue causing this to happen for a small number of spikes, ')
+        logger.info('and are working on a fix.')
 
     return st, tF, Wall, clu
 
 
 def cluster_spikes(st, tF, ops, device, bfile, tic0=np.nan, progress_bar=None):
     tic = time.time()
-    print('\nFinal clustering')
+    logger.info(' ')
+    logger.info('Final clustering')
+    logger.info('-'*40)
     clu, Wall = clustering_qr.run(ops, st, tF,  mode = 'template', device=device,
                                   progress_bar=progress_bar)
-    print(f'{clu.max()+1} clusters found, in {time.time()-tic : .2f}s; ' + 
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'{clu.max()+1} clusters found, in {time.time()-tic : .2f}s; ' + 
+                f'total {time.time()-tic0 : .2f}s')
 
     tic = time.time()
-    print('\nMerging clusters')
+    logger.info(' ')
+    logger.info('Merging clusters')
+    logger.info('-'*40)
     Wall, clu, is_ref = template_matching.merging_function(ops, Wall, clu, st[:,0],
                                                            device=device)
     clu = clu.astype('int32')
-    print(f'{clu.max()+1} units found, in {time.time()-tic : .2f}s; ' + 
-            f'total {time.time()-tic0 : .2f}s')
+    logger.info(f'{clu.max()+1} units found, in {time.time()-tic : .2f}s; ' + 
+                f'total {time.time()-tic0 : .2f}s')
 
     bfile.close()
 
     return clu, Wall
 
 
 def save_sorting(ops, results_dir, st, clu, tF, Wall, imin, tic0=np.nan,
@@ -484,32 +531,35 @@
     ops : dict
     similar_templates : np.ndarray
     is_ref : np.ndarray
     est_contam_rate : np.ndarray
     
     """
 
-    print('\nSaving to phy and computing refractory periods')
+    logger.info(' ')
+    logger.info('Saving to phy and computing refractory periods')
+    logger.info('-'*40)
     results_dir, similar_templates, is_ref, est_contam_rate, kept_spikes = \
         io.save_to_phy(
             st, clu, tF, Wall, ops['probe'], ops, imin, results_dir=results_dir,
             data_dtype=ops['data_dtype'], save_extra_vars=save_extra_vars
             )
-    print(f'{int(is_ref.sum())} units found with good refractory periods')
+    logger.info(f'{int(is_ref.sum())} units found with good refractory periods')
     
     runtime = time.time()-tic0
     seconds = runtime % 60
     mins = runtime // 60
     hrs = mins // 60
     mins = mins % 60
-    print(f'\nTotal runtime: {runtime:.2f}s = {int(hrs):02d}:' +
-          f'{int(mins):02d}:{round(seconds)} h:m:s')
-    ops['runtime'] = runtime 
 
+    logger.info(f'Total runtime: {runtime:.2f}s = {int(hrs):02d}:' +
+                f'{int(mins):02d}:{round(seconds)} h:m:s')
+    ops['runtime'] = runtime 
     io.save_ops(ops, results_dir)
+    logger.info(f'Sorting output saved in: {results_dir}.')
 
     return ops, similar_templates, is_ref, est_contam_rate, kept_spikes
 
 
 def load_sorting(results_dir, device=None, load_extra_vars=False):
     if device is None:
         if torch.cuda.is_available():
```

### Comparing `kilosort-4.0.7/kilosort/simulation.py` & `kilosort-4.0.8/kilosort/simulation.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/spikedetect.py` & `kilosort-4.0.8/kilosort/spikedetect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from io import StringIO
-import warnings
+import logging
+logger = logging.getLogger(__name__)
 
 from torch.nn.functional import max_pool2d, avg_pool2d, conv1d, max_pool1d
 import numpy as np
 import torch
 from sklearn.cluster import KMeans
 from sklearn.decomposition import TruncatedSVD
 from tqdm import tqdm
@@ -179,23 +180,23 @@
     return yct
 
 def run(ops, bfile, device=torch.device('cuda'), progress_bar=None):        
     sig = ops['settings']['min_template_size']
     nsizes = ops['settings']['template_sizes'] 
 
     if ops['settings']['templates_from_data']:
-        print('Re-computing universal templates from data.')
+        logger.info('Re-computing universal templates from data.')
         # Determine templates and PC features from data.
         ops['wPCA'], ops['wTEMP'] = extract_wPCA_wTEMP(
             ops, bfile, nt=ops['nt'], twav_min=ops['nt0min'], 
             Th_single_ch=ops['settings']['Th_single_ch'], nskip=25,
             device=device
             )
     else:
-        print('Using built-in universal templates.')
+        logger.info('Using built-in universal templates.')
         # Use pre-computed templates.
         ops['wPCA'], ops['wTEMP'] = get_waves(ops, device=device)
 
     ops = template_centers(ops)
     [ys, xs] = np.meshgrid(ops['yup'], ops['xup'])
     ys, xs = ys.flatten(), xs.flatten()
     xc, yc = ops['xc'], ops['yc']
```

### Comparing `kilosort-4.0.7/kilosort/swarmsplitter.py` & `kilosort-4.0.8/kilosort/swarmsplitter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/template_matching.py` & `kilosort-4.0.8/kilosort/template_matching.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort/utils.py` & `kilosort-4.0.8/kilosort/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import os, tempfile, shutil, pathlib
+import logging
+logger = logging.getLogger(__name__)
+
 from tqdm import tqdm
 from urllib.request import urlopen
 from urllib.error import HTTPError
 
 _DOWNLOADS_URL = 'https://www.kilosort.org/downloads'
 _DOWNLOADS_DIR_ENV = os.environ.get("KILOSORT_LOCAL_DOWNLOADS_PATH")
 _DOWNLOADS_DIR_DEFAULT = pathlib.Path.home().joinpath('.kilosort')
@@ -14,41 +17,42 @@
     'neuropixPhase3A_kilosortChanMap.mat',
     'neuropixPhase3B1_kilosortChanMap.mat',
     'neuropixPhase3B2_kilosortChanMap.mat',
     'NP2_kilosortChanMap.mat', 
     'Linear16x1_kilosortChanMap.mat',
     ]
 
+
 def template_path(basename='wTEMP.npz'):
     """ currently only one set of example templates to use"""
     return cache_template_path(basename)
 
 def cache_template_path(basename):
     DOWNLOADS_DIR.mkdir(parents=True, exist_ok=True)
     url = f'{_DOWNLOADS_URL}/{basename}'
     cached_file = os.fspath(DOWNLOADS_DIR.joinpath(basename)) 
     if not os.path.exists(cached_file):
-        print('Downloading: "{}" to {}\n'.format(url, cached_file))
+        logger.info('Downloading: "{}" to {}\n'.format(url, cached_file))
         download_url_to_file(url, cached_file, progress=True)
     return cached_file
 
 def download_probes(probe_dir=None):
     if probe_dir is None:
         probe_dir = PROBE_DIR
     probe_dir.mkdir(parents=True, exist_ok=True)
     for probe_name in probe_names:
         url = f'{_DOWNLOADS_URL}/{probe_name}'
         cached_file = os.fspath(probe_dir.joinpath(probe_name)) 
         if not os.path.exists(cached_file):
-            print('Downloading: "{}" to {}\n'.format(url, cached_file))
+            logger.info('Downloading: "{}" to {}\n'.format(url, cached_file))
             try:
                 download_url_to_file(url, cached_file, progress=True)
             except HTTPError as e:
-                print(f'Unable to download probe {probe_name}, error:')
-                print(e)
+                logger.info(f'Unable to download probe {probe_name}, error:')
+                logger.info(e)
 
 
 def download_url_to_file(url, dst, progress=True):
     r"""Download object at the given URL to a local path.
             Thanks to torch, slightly modified
     Args:
         url (string): URL of the object to download
```

### Comparing `kilosort-4.0.7/kilosort/wTEMP.npz` & `kilosort-4.0.8/kilosort/wTEMP.npz`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/kilosort.egg-info/PKG-INFO` & `kilosort-4.0.8/kilosort.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.7
+Version: 4.0.8
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -49,15 +49,15 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/blob/master/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 
 
-You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
+You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available here: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mouseland/kilosort/blob/main/docs/tutorials/kilosort4.ipynb). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
 
 Example notebooks are provided in the `docs/source/tutorials` folder and in the [docs](https://kilosort.readthedocs.io/en/latest/tutorials/tutorials.html). The notebooks include: 
 
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
```

### Comparing `kilosort-4.0.7/kilosort.egg-info/SOURCES.txt` & `kilosort-4.0.8/kilosort.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/hardware.rst
 docs/index.rst
 docs/make.bat
 docs/multi_shank.rst
 docs/parameters.rst
 docs/requirements.txt
 docs/tutorials/basic_example.ipynb
+docs/tutorials/kilosort4.ipynb
 docs/tutorials/load_data.ipynb
 docs/tutorials/make_probe.ipynb
 docs/tutorials/tutorials.rst
 kilosort/CCG.py
 kilosort/__init__.py
 kilosort/__main__.py
 kilosort/bench.py
```

### Comparing `kilosort-4.0.7/setup.py` & `kilosort-4.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tests/conftest.py` & `kilosort-4.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tests/test_clustering.py` & `kilosort-4.0.8/tests/test_clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,49 +38,51 @@
 
     return {'xc': xc[contact_indices], 'yc': yc[contact_indices]}
 
 
 class TestCenters:
     ops = {'dminx': 32}
 
-    def __init__(self, data_directory):
-        # This is just here to make sure probes are downloaded before these
-        # tests are run.
-        pass
-
-    def test_linear(self):
-        self.ops['probe'] = load_probe(PROBE_DIR/'Linear16x1_kilosortChanMap.mat')
+    def test_linear(self, data_directory):
+        # NOTE: The `data_directory` argument is only there to make sure probes are
+        # downloaded before these tests are run.
+        probe = load_probe(PROBE_DIR/'Linear16x1_kilosortChanMap.mat')
+        self.ops['xc'] = probe['xc']
         centers = x_centers(self.ops)
         # X positions are all 1um
         assert len(centers) == 1
         assert np.abs(centers[0] - 1) < 5
 
     def test_np1(self):
-        self.ops['probe'] = load_probe(PROBE_DIR/'neuropixPhase3B1_kilosortChanMap.mat')
+        probe = load_probe(PROBE_DIR/'neuropixPhase3B1_kilosortChanMap.mat')
+        self.ops['xc'] = probe['xc']
         centers = x_centers(self.ops)
         # One shank from 11um to 59um, should be 1 center near 35um
         assert len(centers) == 1
         assert np.abs(centers[0] - 35) < 5
 
     def test_np2_1shank(self):
-        self.ops['probe'] = load_probe(PROBE_DIR/'NP2_kilosortChanMap.mat')
+        probe = load_probe(PROBE_DIR/'NP2_kilosortChanMap.mat')
+        self.ops['xc'] = probe['xc']
         centers = x_centers(self.ops)
         # One shank from 0 to 32um, should be 1 center near 16um
         assert len(centers) == 1
         assert np.abs(centers[0] - 16) < 5
 
     def test_np2_3shank(self):
-        self.ops['probe'] = random_np2(n_shanks=3)
+        probe = random_np2(n_shanks=3)
+        self.ops['xc'] = probe['xc']
         centers = x_centers(self.ops)
         assert len(centers == 3)
         true = np.array([22, 272, 522, 772])
         for c in centers:
             # Each center is within 2 microns of exactly one true center
             print(f'center: {c}')
             assert (np.abs(c - true) < 5).sum() == 1
 
     def test_np2_4shank(self):
-        self.ops['probe'] = random_np2(n_shanks=4)
+        probe = random_np2(n_shanks=4)
+        self.ops['xc'] = probe['xc']
         centers = x_centers(self.ops)
         # All centers should be within 2 microns of the true values
         print(f'centers: {centers}')
         assert np.allclose(np.sort(centers), np.sort([22, 272, 522, 772]), atol=5)
```

### Comparing `kilosort-4.0.7/tests/test_dtype.py` & `kilosort-4.0.8/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tests/test_full_pipeline.py` & `kilosort-4.0.8/tests/test_full_pipeline.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tests/test_io.py` & `kilosort-4.0.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tests/test_parameters.py` & `kilosort-4.0.8/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tests/test_preprocessing.py` & `kilosort-4.0.8/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.7/tox.ini` & `kilosort-4.0.8/tox.ini`

 * *Files identical despite different names*

