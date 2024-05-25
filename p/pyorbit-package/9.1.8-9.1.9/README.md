# Comparing `tmp/pyorbit-package-9.1.8.tar.gz` & `tmp/pyorbit-package-9.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorbit-package-9.1.8.tar", last modified: Thu Mar  9 10:55:11 2023, max compression
+gzip compressed data, was "pyorbit-package-9.1.9.tar", last modified: Tue Mar 14 15:56:20 2023, max compression
```

## Comparing `pyorbit-package-9.1.8.tar` & `pyorbit-package-9.1.9.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.531958 pyorbit-package-9.1.8/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      562 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/.gitignore
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      729 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/.readthedocs.yaml
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1089 2022-06-09 12:46:56.000000 pyorbit-package-9.1.8/LICENSE
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9422 2023-03-09 10:55:11.531958 pyorbit-package-9.1.8/PKG-INFO
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      150 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/PyORBIT_GetResults.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      150 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/PyORBIT_Results.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      145 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/PyORBIT_Run.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8842 2023-03-07 16:13:54.000000 pyorbit-package-9.1.8/README.md
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.501958 pyorbit-package-9.1.8/docs/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      604 2022-06-09 12:46:56.000000 pyorbit-package-9.1.8/docs/Makefile
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.501958 pyorbit-package-9.1.8/docs/_static/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)   153624 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/docs/_static/PyORBIT_logo_transp.png
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.501958 pyorbit-package-9.1.8/docs/_templates/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      427 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/docs/_templates/globaltoc.html
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      120 2022-06-09 12:46:56.000000 pyorbit-package-9.1.8/docs/api.rst
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/docs/common_objects/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3906 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/common_objects/planets.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)       17 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/common_objects/star.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1096 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/common_objects.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4526 2022-07-12 08:40:41.000000 pyorbit-package-9.1.8/docs/conf.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/docs/configuration_file/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10374 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/configuration_file/prepare_common.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2050 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/configuration_file/prepare_input.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3956 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/index.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7426 2022-07-12 08:40:41.000000 pyorbit-package-9.1.8/docs/installation.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      811 2022-06-09 12:46:56.000000 pyorbit-package-9.1.8/docs/make.bat
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/docs/models/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1404 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/models/radial_velocities.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      448 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/models.md
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/docs/old/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      227 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/old/modules_abstract_common.rst
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      217 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/old/modules_abstract_model.rst
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      196 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/old/modules_planets.rst
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13475 2022-07-12 08:40:41.000000 pyorbit-package-9.1.8/docs/prepare_datasets.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1508 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/prepare_yaml.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      128 2022-11-03 17:41:48.000000 pyorbit-package-9.1.8/docs/requirements.txt
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/docs/results_interpretation/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    15819 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/results_interpretation/terminal_output.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1938 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/docs/results_interpretation.md
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      736 2022-11-18 15:42:54.000000 pyorbit-package-9.1.8/extra_requirements.txt
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      143 2022-06-09 12:46:56.000000 pyorbit-package-9.1.8/fetch_constants.sh
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/pyorbit/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      617 2023-03-09 10:54:43.000000 pyorbit-package-9.1.8/pyorbit/__init__.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/pyorbit/classes/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    21876 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_abstract.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1519 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_dynesty.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      985 2022-11-09 14:27:39.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_emcee.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2113 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_multinest.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1318 2022-11-03 17:41:48.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_nestle.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1363 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_optimize.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1232 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_polychord.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1366 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_ultranest.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      981 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/classes/model_container_zeus.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.511958 pyorbit-package-9.1.8/pyorbit/common/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10769 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/common/abstract_common.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9767 2022-07-12 08:40:41.000000 pyorbit-package-9.1.8/pyorbit/common/activity.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5540 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/cheops_modelling.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      511 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/common_jitter.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      465 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/common_offset.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3784 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/common/correlation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9816 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/dataset.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      631 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/dilution_factor.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2529 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/harmonics.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2101 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/lightcurve_detrending.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7745 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/common/limb_darkening.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      667 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/common/normalization_factor.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    14988 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/common/planets.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1434 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/common/polynomial_trend.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2361 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/common/sinusoid.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5300 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/common/star_parameters.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12370 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/model_definitions.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.521958 pyorbit-package-9.1.8/pyorbit/models/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)        0 2022-06-09 12:46:56.000000 pyorbit-package-9.1.8/pyorbit/models/__init__.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13456 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/abstract_model.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    19080 2023-02-28 17:05:28.000000 pyorbit-package-9.1.8/pyorbit/models/abstract_transit.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7549 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/batman_transit.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8394 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/batman_transit_rprs_subset.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10131 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/batman_transit_secondary_phasecurve.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8423 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/batman_transit_ttv_subset.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9082 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/batman_transit_ttv_subset_faster.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7583 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/batman_transit_with_ttv.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12753 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite2_granulation_oscillation_rotation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6780 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite2_granulation_rotation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3797 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite2_matern32.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5723 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite2_rotation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3708 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite_matern32.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3692 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite_matern32_common.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6488 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/celerite_rotation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1648 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/models/celerite_term.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10062 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/models/cheops_detrending.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10079 2023-02-28 17:05:28.000000 pyorbit-package-9.1.8/pyorbit/models/cheops_factormodel.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1422 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/common_jitter.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1385 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/common_offset.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3483 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/models/complex_correlation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3645 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/correlated_jitter.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2344 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/correlation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1356 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/dilution_factor.py
--rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)    14707 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_framework_quasiperiodic_activity.py
--rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)    15156 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/models/gp_multidimensional_quasiperiodic_activity.py
--rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)     9064 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_pyaneti_quasiperiodic_activity.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8368 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6811 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity_alternative.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8965 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity_common.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7891 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity_derivative.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6997 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_cosine_activity.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4305 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/harmonics.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8570 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/lightcurve_detrending.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5771 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/lightcurve_linear_detrending.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9353 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/lightcurve_poly_detrending.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2803 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/normalization_factor.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    14455 2023-02-28 16:44:58.000000 pyorbit-package-9.1.8/pyorbit/models/polynomial_trend.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3386 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/pytransit_transit.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4172 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/pytransit_transit_with_ttv.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4244 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/pytransit_transit_with_ttv_ancyllary.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    33852 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/radial_velocities.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4834 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/rossitermclaughlin_ohta.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8356 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/rossitermclaughlin_starry.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6978 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/sinusoid.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9633 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/spectral_rotation.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5722 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/spiderman_thermal.py
--rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)    10374 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/tinygp_multidimensional_quasiperiodic_activity.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4744 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/models/tinygp_quasiperiodic_activity.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7035 2023-03-07 12:32:03.000000 pyorbit-package-9.1.8/pyorbit/pyorbit_results.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2834 2023-03-06 11:39:25.000000 pyorbit-package-9.1.8/pyorbit/pyorbit_run.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.521958 pyorbit-package-9.1.8/pyorbit/samplers/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)        0 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/samplers/__init__.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9256 2023-03-07 14:59:16.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_dynesty.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    15761 2023-03-07 15:03:39.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_emcee.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    14381 2023-03-07 15:05:25.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_emcee_mpi.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    75433 2023-03-09 09:57:53.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_getresults.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4207 2023-03-07 15:12:25.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_multinest.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8375 2023-03-07 15:12:37.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_nestle.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2640 2023-02-03 14:47:27.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_optimize.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3675 2023-03-07 15:57:14.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_polychord.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3929 2023-03-07 15:13:10.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_pyde.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3882 2023-03-07 15:13:16.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_ultranest.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12143 2023-03-07 15:16:01.000000 pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_zeus.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.521958 pyorbit-package-9.1.8/pyorbit/subroutines/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      125 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/subroutines/__init__.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12997 2023-03-06 17:42:58.000000 pyorbit-package-9.1.8/pyorbit/subroutines/common.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2877 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/subroutines/constants.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    46204 2023-03-06 11:07:24.000000 pyorbit-package-9.1.8/pyorbit/subroutines/input_parser.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13441 2022-11-03 17:41:48.000000 pyorbit-package-9.1.8/pyorbit/subroutines/io_subroutines.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10156 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/subroutines/kepler_exo.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10002 2022-06-30 13:06:26.000000 pyorbit-package-9.1.8/pyorbit/subroutines/kepler_old.py
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)    47578 2023-03-09 10:50:20.000000 pyorbit-package-9.1.8/pyorbit/subroutines/results_analysis.py
-drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-09 10:55:11.531958 pyorbit-package-9.1.8/pyorbit_package.egg-info/
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9422 2023-03-09 10:55:11.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/PKG-INFO
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4848 2023-03-09 10:55:11.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/SOURCES.txt
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)        1 2023-03-09 10:55:11.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/dependency_links.txt
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      122 2023-03-09 10:55:11.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/entry_points.txt
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)        1 2022-06-20 16:56:17.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/not-zip-safe
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)      184 2023-03-09 10:55:11.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/requires.txt
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)        8 2023-03-09 10:55:11.000000 pyorbit-package-9.1.8/pyorbit_package.egg-info/top_level.txt
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)       38 2023-03-09 10:55:11.531958 pyorbit-package-9.1.8/setup.cfg
--rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2026 2023-03-09 10:54:30.000000 pyorbit-package-9.1.8/setup.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      562 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/.gitignore
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      729 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/.readthedocs.yaml
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1089 2022-06-09 12:46:56.000000 pyorbit-package-9.1.9/LICENSE
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9447 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/PKG-INFO
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      150 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/PyORBIT_GetResults.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      150 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/PyORBIT_Results.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      184 2023-03-10 16:11:00.000000 pyorbit-package-9.1.9/PyORBIT_Run.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8867 2023-03-14 15:55:59.000000 pyorbit-package-9.1.9/README.md
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.286950 pyorbit-package-9.1.9/docs/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      604 2022-06-09 12:46:56.000000 pyorbit-package-9.1.9/docs/Makefile
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.286950 pyorbit-package-9.1.9/docs/_static/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)   153624 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/docs/_static/PyORBIT_logo_transp.png
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.286950 pyorbit-package-9.1.9/docs/_templates/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      427 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/docs/_templates/globaltoc.html
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      120 2022-06-09 12:46:56.000000 pyorbit-package-9.1.9/docs/api.rst
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.286950 pyorbit-package-9.1.9/docs/common_objects/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3906 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/common_objects/planets.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)       17 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/common_objects/star.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1096 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/common_objects.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4526 2022-07-12 08:40:41.000000 pyorbit-package-9.1.9/docs/conf.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.296950 pyorbit-package-9.1.9/docs/configuration_file/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10374 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/configuration_file/prepare_common.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2050 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/configuration_file/prepare_input.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3956 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/index.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7426 2022-07-12 08:40:41.000000 pyorbit-package-9.1.9/docs/installation.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      811 2022-06-09 12:46:56.000000 pyorbit-package-9.1.9/docs/make.bat
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.296950 pyorbit-package-9.1.9/docs/models/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1404 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/models/radial_velocities.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      448 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/models.md
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.296950 pyorbit-package-9.1.9/docs/old/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      227 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/old/modules_abstract_common.rst
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      217 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/old/modules_abstract_model.rst
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      196 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/old/modules_planets.rst
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13475 2022-07-12 08:40:41.000000 pyorbit-package-9.1.9/docs/prepare_datasets.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1508 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/prepare_yaml.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      128 2022-11-03 17:41:48.000000 pyorbit-package-9.1.9/docs/requirements.txt
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.296950 pyorbit-package-9.1.9/docs/results_interpretation/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    15819 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/results_interpretation/terminal_output.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1938 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/docs/results_interpretation.md
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      736 2022-11-18 15:42:54.000000 pyorbit-package-9.1.9/extra_requirements.txt
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      143 2022-06-09 12:46:56.000000 pyorbit-package-9.1.9/fetch_constants.sh
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.296950 pyorbit-package-9.1.9/pyorbit/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      617 2023-03-14 15:56:10.000000 pyorbit-package-9.1.9/pyorbit/__init__.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.296950 pyorbit-package-9.1.9/pyorbit/classes/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    21876 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_abstract.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1519 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_dynesty.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      985 2022-11-09 14:27:39.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_emcee.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2113 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_multinest.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1318 2022-11-03 17:41:48.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_nestle.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1363 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_optimize.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1232 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_polychord.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1366 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_ultranest.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      981 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/classes/model_container_zeus.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.306950 pyorbit-package-9.1.9/pyorbit/common/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10769 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/common/abstract_common.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10619 2023-03-14 15:32:10.000000 pyorbit-package-9.1.9/pyorbit/common/activity.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5540 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/cheops_modelling.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      511 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/common_jitter.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      465 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/common_offset.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3784 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/common/correlation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10040 2023-03-10 17:13:43.000000 pyorbit-package-9.1.9/pyorbit/common/dataset.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      631 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/dilution_factor.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2529 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/harmonics.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2101 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/lightcurve_detrending.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7745 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/common/limb_darkening.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      667 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/common/normalization_factor.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    14988 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/common/planets.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1434 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/common/polynomial_trend.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2361 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/common/sinusoid.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5300 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/common/star_parameters.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12461 2023-03-14 15:54:46.000000 pyorbit-package-9.1.9/pyorbit/model_definitions.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/pyorbit/models/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)        0 2022-06-09 12:46:56.000000 pyorbit-package-9.1.9/pyorbit/models/__init__.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13456 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/abstract_model.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    19080 2023-02-28 17:05:28.000000 pyorbit-package-9.1.9/pyorbit/models/abstract_transit.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7351 2023-03-10 16:46:32.000000 pyorbit-package-9.1.9/pyorbit/models/batman_transit.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8261 2023-03-10 16:46:45.000000 pyorbit-package-9.1.9/pyorbit/models/batman_transit_rprs_subset.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9998 2023-03-10 16:46:55.000000 pyorbit-package-9.1.9/pyorbit/models/batman_transit_secondary_phasecurve.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8318 2023-03-10 17:04:21.000000 pyorbit-package-9.1.9/pyorbit/models/batman_transit_ttv_subset.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8949 2023-03-10 16:47:06.000000 pyorbit-package-9.1.9/pyorbit/models/batman_transit_ttv_subset_faster.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7430 2023-03-10 16:46:25.000000 pyorbit-package-9.1.9/pyorbit/models/batman_transit_with_ttv.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12753 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite2_granulation_oscillation_rotation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6780 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite2_granulation_rotation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3797 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite2_matern32.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5723 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite2_rotation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4794 2023-03-14 15:53:35.000000 pyorbit-package-9.1.9/pyorbit/models/celerite2_sho.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3708 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite_matern32.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3692 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite_matern32_common.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6488 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/celerite_rotation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1648 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/models/celerite_term.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10062 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/models/cheops_detrending.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10079 2023-02-28 17:05:28.000000 pyorbit-package-9.1.9/pyorbit/models/cheops_factormodel.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1422 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/common_jitter.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1385 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/common_offset.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3483 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/models/complex_correlation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3645 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/correlated_jitter.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2344 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/correlation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     1356 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/dilution_factor.py
+-rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)    14707 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_framework_quasiperiodic_activity.py
+-rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)    15156 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/models/gp_multidimensional_quasiperiodic_activity.py
+-rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)     9064 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_pyaneti_quasiperiodic_activity.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8368 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6811 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity_alternative.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8965 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity_common.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7891 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity_derivative.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6997 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_cosine_activity.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4305 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/harmonics.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8570 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/lightcurve_detrending.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5771 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/lightcurve_linear_detrending.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9353 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/lightcurve_poly_detrending.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2803 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/normalization_factor.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    14455 2023-02-28 16:44:58.000000 pyorbit-package-9.1.9/pyorbit/models/polynomial_trend.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3386 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/pytransit_transit.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4172 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/pytransit_transit_with_ttv.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4244 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/pytransit_transit_with_ttv_ancyllary.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    33852 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/radial_velocities.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4834 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/rossitermclaughlin_ohta.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8356 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/rossitermclaughlin_starry.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     6978 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/sinusoid.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9633 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/spectral_rotation.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     5722 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/spiderman_thermal.py
+-rwxr-xr-x   0 malavolta  (1000) malavolta  (1000)    10374 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/tinygp_multidimensional_quasiperiodic_activity.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4744 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/models/tinygp_quasiperiodic_activity.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     7035 2023-03-07 12:32:03.000000 pyorbit-package-9.1.9/pyorbit/pyorbit_results.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2834 2023-03-06 11:39:25.000000 pyorbit-package-9.1.9/pyorbit/pyorbit_run.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/pyorbit/samplers/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)        0 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/samplers/__init__.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9257 2023-03-10 16:06:36.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_dynesty.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    15761 2023-03-07 15:03:39.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_emcee.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    14381 2023-03-07 15:05:25.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_emcee_mpi.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    75433 2023-03-09 09:57:53.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_getresults.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4207 2023-03-07 15:12:25.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_multinest.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     8375 2023-03-07 15:12:37.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_nestle.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2640 2023-02-03 14:47:27.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_optimize.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3675 2023-03-07 15:57:14.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_polychord.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3929 2023-03-07 15:13:10.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_pyde.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     3882 2023-03-07 15:13:16.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_ultranest.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    12143 2023-03-07 15:16:01.000000 pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_zeus.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/pyorbit/subroutines/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      125 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/subroutines/__init__.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13093 2023-03-14 11:23:08.000000 pyorbit-package-9.1.9/pyorbit/subroutines/common.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2877 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/subroutines/constants.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    46204 2023-03-06 11:07:24.000000 pyorbit-package-9.1.9/pyorbit/subroutines/input_parser.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    13441 2022-11-03 17:41:48.000000 pyorbit-package-9.1.9/pyorbit/subroutines/io_subroutines.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10156 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/subroutines/kepler_exo.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    10002 2022-06-30 13:06:26.000000 pyorbit-package-9.1.9/pyorbit/subroutines/kepler_old.py
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)    47474 2023-03-10 15:17:18.000000 pyorbit-package-9.1.9/pyorbit/subroutines/results_analysis.py
+drwxr-xr-x   0 malavolta  (1000) malavolta  (1000)        0 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/pyorbit_package.egg-info/
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     9447 2023-03-14 15:56:20.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/PKG-INFO
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     4880 2023-03-14 15:56:20.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/SOURCES.txt
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)        1 2023-03-14 15:56:20.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/dependency_links.txt
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      122 2023-03-14 15:56:20.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/entry_points.txt
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)        1 2022-06-20 16:56:17.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/not-zip-safe
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)      184 2023-03-14 15:56:20.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/requires.txt
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)        8 2023-03-14 15:56:20.000000 pyorbit-package-9.1.9/pyorbit_package.egg-info/top_level.txt
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)       38 2023-03-14 15:56:20.316950 pyorbit-package-9.1.9/setup.cfg
+-rw-r--r--   0 malavolta  (1000) malavolta  (1000)     2026 2023-03-14 15:55:24.000000 pyorbit-package-9.1.9/setup.py
```

### Comparing `pyorbit-package-9.1.8/.gitignore` & `pyorbit-package-9.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/.readthedocs.yaml` & `pyorbit-package-9.1.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/LICENSE` & `pyorbit-package-9.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/PKG-INFO` & `pyorbit-package-9.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorbit-package
-Version: 9.1.8
+Version: 9.1.9
 Summary: PyORBIT: a code for exoplanet orbital parameters and stellar activity
 Home-page: https://github.com/LucaMalavolta/PyORBIT
 Author: Luca Malavolta
 Author-email: luca.malavolta@unipd.it
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -15,19 +15,21 @@
 License-File: LICENSE
 
 
 ![PyORBIT logo](docs/_static/PyORBIT_logo_transp.png?raw=true)
 
 ### A code for exoplanet orbital parameters and stellar activity.
 ***
-### `PyORBIT` version 9.1 by Luca Malavolta - December 2022
+### `PyORBIT` version 9.1 by Luca Malavolta - March 2023
 
 **News**
 
-* Imrpoved output: `spaces`, `bounds`, and `priors` explicitely written out at runtime
+* Added celerite2 SHO term
+
+* Improved output: `spaces`, `bounds`, and `priors` explicitely written out at runtime
 
 * Minor changes:
   * `dataset_variables` and `common_variables` changed to `dataset_parameters`
     and `common_parameters`
   * New models added
   * All instances named `variables` renamed to `parameters` for internal
     consistency. Backward compatibility ensured by new method in `model_container_abstract`
```

### Comparing `pyorbit-package-9.1.8/README.md` & `pyorbit-package-9.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 ![PyORBIT logo](docs/_static/PyORBIT_logo_transp.png?raw=true)
 
 ### A code for exoplanet orbital parameters and stellar activity.
 ***
-### `PyORBIT` version 9.1 by Luca Malavolta - December 2022
+### `PyORBIT` version 9.1 by Luca Malavolta - March 2023
 
 **News**
 
-* Imrpoved output: `spaces`, `bounds`, and `priors` explicitely written out at runtime
+* Added celerite2 SHO term
+
+* Improved output: `spaces`, `bounds`, and `priors` explicitely written out at runtime
 
 * Minor changes:
   * `dataset_variables` and `common_variables` changed to `dataset_parameters`
     and `common_parameters`
   * New models added
   * All instances named `variables` renamed to `parameters` for internal
     consistency. Backward compatibility ensured by new method in `model_container_abstract`
```

### Comparing `pyorbit-package-9.1.8/docs/Makefile` & `pyorbit-package-9.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/_static/PyORBIT_logo_transp.png` & `pyorbit-package-9.1.9/docs/_static/PyORBIT_logo_transp.png`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/common_objects/planets.md` & `pyorbit-package-9.1.9/docs/common_objects/planets.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/common_objects.md` & `pyorbit-package-9.1.9/docs/common_objects.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/conf.py` & `pyorbit-package-9.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/configuration_file/prepare_common.md` & `pyorbit-package-9.1.9/docs/configuration_file/prepare_common.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/configuration_file/prepare_input.md` & `pyorbit-package-9.1.9/docs/configuration_file/prepare_input.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/index.md` & `pyorbit-package-9.1.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/installation.md` & `pyorbit-package-9.1.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/make.bat` & `pyorbit-package-9.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/models/radial_velocities.md` & `pyorbit-package-9.1.9/docs/models/radial_velocities.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/prepare_datasets.md` & `pyorbit-package-9.1.9/docs/prepare_datasets.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/prepare_yaml.md` & `pyorbit-package-9.1.9/docs/prepare_yaml.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/results_interpretation/terminal_output.md` & `pyorbit-package-9.1.9/docs/results_interpretation/terminal_output.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/docs/results_interpretation.md` & `pyorbit-package-9.1.9/docs/results_interpretation.md`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/extra_requirements.txt` & `pyorbit-package-9.1.9/extra_requirements.txt`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/__init__.py` & `pyorbit-package-9.1.9/pyorbit/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 from .samplers.pyorbit_dynesty import *
 from .samplers.pyorbit_nestle import *
 from .samplers.pyorbit_ultranest import *
 from .samplers.pyorbit_multinest import *
 from .samplers.pyorbit_getresults import *
 from .subroutines.input_parser import yaml_parser
 
-__version__ = "9.1.8"
+__version__ = "9.1.9"
```

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_abstract.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_abstract.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_dynesty.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_dynesty.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_emcee.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_emcee.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_multinest.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_multinest.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_nestle.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_nestle.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_optimize.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_optimize.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_polychord.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_polychord.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_ultranest.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_ultranest.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/classes/model_container_zeus.py` & `pyorbit-package-9.1.9/pyorbit/classes/model_container_zeus.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/abstract_common.py` & `pyorbit-package-9.1.9/pyorbit/common/abstract_common.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/activity.py` & `pyorbit-package-9.1.9/pyorbit/common/activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,38 @@
                 'bounds': [0.00000001, 1000000.0],
                 'priors': ['Uniform', []],
                 'spaces': 'Linear',
                 'fixed' : None,
                 'unit': 'as input',
             },
         #celerite 2 parameters
+        'sho_period': # undamped period of the granulation
+            {
+                'bounds': [1.0, 1000.0],
+                'priors': ['Uniform', []],
+                'spaces': 'Linear',
+                'fixed' : None,
+                'unit': 'days',
+            },
+        'sho_tau': # the standard deviation of the process
+            {
+                'bounds': [0.00000001, 1000000.0],
+                'priors': ['Uniform', []],
+                'spaces': 'Log_Base2',
+                'fixed' : None,
+                'unit': 'as input',
+            },
+        'sho_sigma': # the standard deviation of the process
+            {
+                'bounds': [0.00000001, 1000000.0],
+                'priors': ['Uniform', []],
+                'spaces': 'Log_Base2',
+                'fixed' : None,
+                'unit': 'as input',
+            },
         'grn_period': # undamped period of the granulation
             {
                 'bounds': [1.0, 1000.0],
                 'priors': ['Uniform', []],
                 'spaces': 'Linear',
                 'fixed' : None,
                 'unit': 'days',
```

### Comparing `pyorbit-package-9.1.8/pyorbit/common/cheops_modelling.py` & `pyorbit-package-9.1.9/pyorbit/common/cheops_modelling.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/correlation.py` & `pyorbit-package-9.1.9/pyorbit/common/correlation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/dataset.py` & `pyorbit-package-9.1.9/pyorbit/common/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,16 +218,20 @@
         else:
             return additive_model + external_model + (1. + unitary_model)*normalization_model
 
     def compute_residuals(self):
         self.residuals = self.y - self.model
 
     def model_logchi2(self):
-
         env = 1.0 / (self.e ** 2.0 + self.jitter ** 2.0)
+
+        #chi2 = -0.5 * (self.n * np.log(2 * np.pi) +
+        #               np.sum(self.residuals ** 2 * env - np.log(env)))
+        #print('{0:25s} {1:12f} {2:12f} \n'.format(self.name_ref, chi2, np.std(self.residuals)))
+
         return -0.5 * (self.n * np.log(2 * np.pi) +
                        np.sum(self.residuals ** 2 * env - np.log(env)))
 
     def update_bounds_spaces_priors_starts(self):
 
         for var_generic in list(set(self.bounds) & set(self.variable_compressed)):
             for var in self.variable_compressed[var_generic]:
```

### Comparing `pyorbit-package-9.1.8/pyorbit/common/dilution_factor.py` & `pyorbit-package-9.1.9/pyorbit/common/dilution_factor.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/harmonics.py` & `pyorbit-package-9.1.9/pyorbit/common/harmonics.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/lightcurve_detrending.py` & `pyorbit-package-9.1.9/pyorbit/common/lightcurve_detrending.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/limb_darkening.py` & `pyorbit-package-9.1.9/pyorbit/common/limb_darkening.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/normalization_factor.py` & `pyorbit-package-9.1.9/pyorbit/common/normalization_factor.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/planets.py` & `pyorbit-package-9.1.9/pyorbit/common/planets.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/polynomial_trend.py` & `pyorbit-package-9.1.9/pyorbit/common/polynomial_trend.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/sinusoid.py` & `pyorbit-package-9.1.9/pyorbit/common/sinusoid.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/common/star_parameters.py` & `pyorbit-package-9.1.9/pyorbit/common/star_parameters.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/model_definitions.py` & `pyorbit-package-9.1.9/pyorbit/model_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 from pyorbit.models.gp_quasiperiodic_activity_derivative import \
     GaussianProcess_QuasiPeriodicActivity_Derivative
 
 from pyorbit.models.celerite2_granulation_rotation import Celerite2_Granulation_Rotation
 from pyorbit.models.celerite2_rotation import Celerite2_Rotation
 from pyorbit.models.celerite2_matern32 import Celerite2_Matern32
+from pyorbit.models.celerite2_sho import Celerite2_SHO
 
 from pyorbit.models.celerite_rotation import Celerite_Rotation
 from pyorbit.models.celerite_matern32 import Celerite_Matern32
 from pyorbit.models.celerite_matern32_common import Celerite_Matern32_Common
 
 from pyorbit.models.correlation import LocalCorrelation
 from pyorbit.models.correlated_jitter import LocalCorrelatedJitter
@@ -180,14 +181,15 @@
     'gp_quasiperiodic_alternative': GaussianProcess_QuasiPeriodicActivity_Alternative,
     'gp_quasiperiodic_derivative': GaussianProcess_QuasiPeriodicActivity_Derivative,
     'gp_quasiperiodic_cosine': GaussianProcess_QuasiPeriodicCosineActivity,
     'celerite2_granulation_rotation': Celerite2_Granulation_Rotation,
     'celerite2_granulation_oscillation_rotation': Celerite2_Granulation_Oscillation_Rotation,
     'celerite2_rotation': Celerite2_Rotation,
     'celerite2_matern32': Celerite2_Matern32,
+    'celerite2_sho': Celerite2_SHO,
     'celerite_matern32': Celerite_Matern32,
     'celerite_matern32_common': Celerite_Matern32_Common,
     'celerite_rotation': Celerite_Rotation,
     'local_correlation': LocalCorrelation,
     'correlation': LocalCorrelation,
     'complex_correlation': ComplexCorrelation,
     'polynomial_trend': PolynomialTrend,
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/abstract_model.py` & `pyorbit-package-9.1.9/pyorbit/models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/abstract_transit.py` & `pyorbit-package-9.1.9/pyorbit/models/abstract_transit.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/batman_transit.py` & `pyorbit-package-9.1.9/pyorbit/models/batman_transit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 
-from pyorbit.subroutines.common import np, convert_rho_to_a, convert_b_to_i
-import pyorbit.subroutines.constants as constants
-import pyorbit.subroutines.kepler_exo as kepler_exo
+from pyorbit.subroutines.common import np
 from pyorbit.models.abstract_model import AbstractModel
 from pyorbit.models.abstract_transit import AbstractTransit
-import multiprocessing
 
 try:
     import batman
 except ImportError:
     pass
 
 
@@ -53,19 +50,17 @@
             import multiprocessing
             if self.code_options['nthreads'] > multiprocessing.cpu_count():
                 print('Batman nthreads automatically lowered to the maximum CPU count')
                 self.code_options['nthreads'] = multiprocessing.cpu_count()
         except:
             self.code_options['nthreads'] = 1
 
-        if not batman.openmp.detect():
-            print('OpenMP not supported, batman nthreads automatically lowered to 1')
-            self.code_options['nthreads'] = 1
-
-        #self.code_options['nthreads'] = 10
+        #if not batman.openmp.detect():
+        #    print('OpenMP not supported, batman nthreads automatically lowered to 1')
+        #    self.code_options['nthreads'] = 1
 
         self.batman_params = batman.TransitParams()
 
         """ Initialization with random transit parameters"""
         self.batman_params.t0 = 0.  # time of inferior conjunction
         self.batman_params.per = 1.  # orbital period
         # planet radius (in units of stellar radii)
@@ -135,17 +130,17 @@
         print 'ecc  ', self.batman_params.ecc
         print 'w    ', self.batman_params.w
         print 'u    ', self.batman_params.u
         """
         for par, i_par in self.ldvars.items():
             self.batman_params.u[i_par] = parameter_values[par]
 
-        if not self.use_inclination:
-            if parameter_values['b'] > 1. + parameter_values['R_Rs']/2. :
-                return -1000000000.00000
+        #if not self.use_inclination:
+        #    if parameter_values['b'] > 1. + parameter_values['R_Rs']/2. :
+        #        return -1000000000.00000
 
 
         """
         From the batman manual:
         Reinitializing the model is by far the slowest component of batman,
         because it calculates the optimal step size for the integration starting
         from a very small value.
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/batman_transit_rprs_subset.py` & `pyorbit-package-9.1.9/pyorbit/models/batman_transit_rprs_subset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from pyorbit.subroutines.common import np, convert_rho_to_a, convert_b_to_i
-import pyorbit.subroutines.constants as constants
-import pyorbit.subroutines.kepler_exo as kepler_exo
+from pyorbit.subroutines.common import np
 from pyorbit.models.abstract_model import AbstractModel
 from pyorbit.models.abstract_transit import AbstractTransit
 
 try:
     import batman
 except ImportError:
     pass
@@ -51,17 +49,17 @@
             import multiprocessing
             if self.code_options['nthreads'] > multiprocessing.cpu_count():
                 print('Batman nthreads automatically lowered to the maximum CPU count')
                 self.code_options['nthreads'] = multiprocessing.cpu_count()
         except:
             self.code_options['nthreads'] = 1
 
-        if not batman.openmp.detect():
-            print('OpenMP not supported, batman nthreads automatically lowered to 1')
-            self.code_options['nthreads'] = 1
+        #if not batman.openmp.detect():
+        #    print('OpenMP not supported, batman nthreads automatically lowered to 1')
+        #    self.code_options['nthreads'] = 1
 
         self.batman_params = batman.TransitParams()
 
         """ Initialization with random transit parameters"""
         self.batman_params.t0 = 0.  # time of inferior conjunction
         self.batman_params.per = 1.  # orbital period
         # planet radius (in units of stellar radii)
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/batman_transit_secondary_phasecurve.py` & `pyorbit-package-9.1.9/pyorbit/models/batman_transit_secondary_phasecurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 
-from pyorbit.subroutines.common import np, convert_rho_to_a, convert_b_to_i
-import pyorbit.subroutines.constants as constants
-import pyorbit.subroutines.kepler_exo as kepler_exo
+from pyorbit.subroutines.common import np
 from pyorbit.models.abstract_model import AbstractModel
 from pyorbit.models.abstract_transit import AbstractTransit
 
 try:
     import batman
 except ImportError:
     pass
@@ -58,17 +56,17 @@
             import multiprocessing
             if self.code_options['nthreads'] > multiprocessing.cpu_count():
                 print('Batman nthreads automatically lowered to the maximum CPU count')
                 self.code_options['nthreads'] = multiprocessing.cpu_count()
         except:
             self.code_options['nthreads'] = 1
 
-        if not batman.openmp.detect():
-            print('OpenMP not supported, batman nthreads automatically lowered to 1')
-            self.code_options['nthreads'] = 1
+        #if not batman.openmp.detect():
+        #    print('OpenMP not supported, batman nthreads automatically lowered to 1')
+        #    self.code_options['nthreads'] = 1
 
         self.batman_params = batman.TransitParams()
 
         if kwargs.get('nightside_emission', True):
             self.nightside_emission = True
         else:
             self.nightside_emission = False
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/batman_transit_ttv_subset.py` & `pyorbit-package-9.1.9/pyorbit/models/batman_transit_ttv_subset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from pyorbit.subroutines.common import np, convert_rho_to_a, convert_b_to_i
-import pyorbit.subroutines.constants as constants
-import pyorbit.subroutines.kepler_exo as kepler_exo
+from pyorbit.subroutines.common import np
 from pyorbit.models.abstract_model import AbstractModel
 from pyorbit.models.abstract_transit import AbstractTransit
 
 try:
     import batman
 except ImportError:
     pass
@@ -49,17 +47,17 @@
             import multiprocessing
             if self.code_options['nthreads'] > multiprocessing.cpu_count():
                 print('Batman nthreads automatically lowered to the maximum CPU count')
                 self.code_options['nthreads'] = multiprocessing.cpu_count()
         except:
             self.code_options['nthreads'] = 1
 
-        if not batman.openmp.detect():
-            print('OpenMP not supported, batman nthreads automatically lowered to 1')
-            self.code_options['nthreads'] = 1
+        #if not batman.openmp.detect():
+        #    print('OpenMP not supported, batman nthreads automatically lowered to 1')
+        #    self.code_options['nthreads'] = 1
 
         self.batman_params = batman.TransitParams()
 
         """ Initialization with random transit parameters"""
         self.batman_params.t0 = 0.  # time of inferior conjunction
         self.batman_params.per = 1.  # orbital period
         # planet radius (in units of stellar radii)
@@ -149,14 +147,15 @@
         for the integration starting from a very small value.
         -> However, we estimated the optimal step size from random parameters,
         so at some point we'll need to
         reinitialize the model so that the correct step size is computed.
         """
 
         random_selector = np.random.randint(1000)
+        random_selector = 50
 
         if x0_input is None:
             y_output = np.zeros(dataset.n)
         else:
             y_output = x0_input * 0.
 
         if not self.use_inclination:
@@ -181,15 +180,14 @@
                                             supersample_factor=self.code_options[
                                                 dataset.name_ref]['sample_factor'],
                                             exp_time=self.code_options[dataset.name_ref]['exp_time'],
                                             nthreads=self.code_options['nthreads'])
 
                 y_output[sel_data] = self.batman_models[dataset.name_ref+ '_'+repr(i_sub)].light_curve(self.batman_params) - 1.
 
-
             else:
                 original_dataset = dataset.x0[(dataset.submodel_id==i_sub)]
                 sel_data = (x0_input >= np.amin(original_dataset)) &  (x0_input <= np.amax(original_dataset))
 
                 temporary_model = batman.TransitModel(self.batman_params,
                                             x0_input[sel_data],
                                             supersample_factor=self.code_options[
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/batman_transit_ttv_subset_faster.py` & `pyorbit-package-9.1.9/pyorbit/models/batman_transit_ttv_subset_faster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from pyorbit.subroutines.common import np, convert_rho_to_a, convert_b_to_i
-import pyorbit.subroutines.constants as constants
-import pyorbit.subroutines.kepler_exo as kepler_exo
+from pyorbit.subroutines.common import np
 from pyorbit.models.abstract_model import AbstractModel
 from pyorbit.models.abstract_transit import AbstractTransit
 from scipy import interpolate
 
 try:
     import batman
 except ImportError:
@@ -50,17 +48,17 @@
             import multiprocessing
             if self.code_options['nthreads'] > multiprocessing.cpu_count():
                 print('Batman nthreads automatically lowered to the maximum CPU count')
                 self.code_options['nthreads'] = multiprocessing.cpu_count()
         except:
             self.code_options['nthreads'] = 1
 
-        if not batman.openmp.detect():
-            print('OpenMP not supported, batman nthreads automatically lowered to 1')
-            self.code_options['nthreads'] = 1
+        #if not batman.openmp.detect():
+        #    print('OpenMP not supported, batman nthreads automatically lowered to 1')
+        #    self.code_options['nthreads'] = 1
 
         self.batman_params = batman.TransitParams()
 
         """ Initialization with random transit parameters"""
         self.batman_params.t0 = 0.  # time of inferior conjunction
         self.batman_params.per = 1.  # orbital period
         # planet radius (in units of stellar radii)
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/batman_transit_with_ttv.py` & `pyorbit-package-9.1.9/pyorbit/models/batman_transit_with_ttv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from pyorbit.subroutines.common import np, convert_rho_to_a, convert_b_to_i
-import pyorbit.subroutines.constants as constants
-import pyorbit.subroutines.kepler_exo as kepler_exo
+from pyorbit.subroutines.common import np
 from pyorbit.models.abstract_model import AbstractModel
 from pyorbit.models.abstract_transit import AbstractTransit
-import multiprocessing
 
 try:
     import batman
 except ImportError:
     pass
 
 
@@ -50,17 +47,17 @@
             import multiprocessing
             if self.code_options['nthreads'] > multiprocessing.cpu_count():
                 print('Batman nthreads automatically lowered to the maximum CPU count')
                 self.code_options['nthreads'] = multiprocessing.cpu_count()
         except:
             self.code_options['nthreads'] = 1
 
-        if not batman.openmp.detect():
-            print('OpenMP not supported, batman nthreads automatically lowered to 1')
-            self.code_options['nthreads'] = 1
+        #if not batman.openmp.detect():
+        #    print('OpenMP not supported, batman nthreads automatically lowered to 1')
+        #    self.code_options['nthreads'] = 1
 
         self.batman_params = batman.TransitParams()
 
         """ Initialization with random transit parameters"""
         self.batman_params.t0 = 0.  # time of inferior conjunction
         self.batman_params.per = 1.  # orbital period
         # planet radius (in units of stellar radii)
@@ -132,17 +129,17 @@
         print 'ecc  ', self.batman_params.ecc
         print 'w    ', self.batman_params.w
         print 'u    ', self.batman_params.u
         """
         for par, i_par in self.ldvars.items():
             self.batman_params.u[i_par] = parameter_values[par]
 
-        if not self.use_inclination:
-            if parameter_values['b'] > 1. + parameter_values['R_Rs'] :
-                return 0.00
+        #if not self.use_inclination:
+        #    if parameter_values['b'] > 1. + parameter_values['R_Rs'] :
+        #        return 0.00
 
 
         """
         From the batman manual:
         Reinitializing the model is by far the slowest component of batman,
         because it calculates the optimal step size
         for the integration starting from a very small value.
```

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite2_granulation_oscillation_rotation.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite2_granulation_oscillation_rotation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite2_granulation_rotation.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite2_granulation_rotation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite2_matern32.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite2_matern32.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite2_rotation.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite2_rotation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite_matern32.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite_matern32.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite_matern32_common.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite_matern32_common.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite_rotation.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite_rotation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/celerite_term.py` & `pyorbit-package-9.1.9/pyorbit/models/celerite_term.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/cheops_detrending.py` & `pyorbit-package-9.1.9/pyorbit/models/cheops_detrending.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/cheops_factormodel.py` & `pyorbit-package-9.1.9/pyorbit/models/cheops_factormodel.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/common_jitter.py` & `pyorbit-package-9.1.9/pyorbit/models/common_jitter.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/common_offset.py` & `pyorbit-package-9.1.9/pyorbit/models/common_offset.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/complex_correlation.py` & `pyorbit-package-9.1.9/pyorbit/models/complex_correlation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/correlated_jitter.py` & `pyorbit-package-9.1.9/pyorbit/models/correlated_jitter.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/correlation.py` & `pyorbit-package-9.1.9/pyorbit/models/correlation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/dilution_factor.py` & `pyorbit-package-9.1.9/pyorbit/models/dilution_factor.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_framework_quasiperiodic_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_framework_quasiperiodic_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_multidimensional_quasiperiodic_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_multidimensional_quasiperiodic_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_pyaneti_quasiperiodic_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_pyaneti_quasiperiodic_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity_alternative.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity_alternative.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity_common.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity_common.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_activity_derivative.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_activity_derivative.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/gp_quasiperiodic_cosine_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/gp_quasiperiodic_cosine_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/harmonics.py` & `pyorbit-package-9.1.9/pyorbit/models/harmonics.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/lightcurve_detrending.py` & `pyorbit-package-9.1.9/pyorbit/models/lightcurve_detrending.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/lightcurve_linear_detrending.py` & `pyorbit-package-9.1.9/pyorbit/models/lightcurve_linear_detrending.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/lightcurve_poly_detrending.py` & `pyorbit-package-9.1.9/pyorbit/models/lightcurve_poly_detrending.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/normalization_factor.py` & `pyorbit-package-9.1.9/pyorbit/models/normalization_factor.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/polynomial_trend.py` & `pyorbit-package-9.1.9/pyorbit/models/polynomial_trend.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/pytransit_transit.py` & `pyorbit-package-9.1.9/pyorbit/models/pytransit_transit.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/pytransit_transit_with_ttv.py` & `pyorbit-package-9.1.9/pyorbit/models/pytransit_transit_with_ttv.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/pytransit_transit_with_ttv_ancyllary.py` & `pyorbit-package-9.1.9/pyorbit/models/pytransit_transit_with_ttv_ancyllary.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/radial_velocities.py` & `pyorbit-package-9.1.9/pyorbit/models/radial_velocities.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/rossitermclaughlin_ohta.py` & `pyorbit-package-9.1.9/pyorbit/models/rossitermclaughlin_ohta.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/rossitermclaughlin_starry.py` & `pyorbit-package-9.1.9/pyorbit/models/rossitermclaughlin_starry.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/sinusoid.py` & `pyorbit-package-9.1.9/pyorbit/models/sinusoid.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/spectral_rotation.py` & `pyorbit-package-9.1.9/pyorbit/models/spectral_rotation.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/spiderman_thermal.py` & `pyorbit-package-9.1.9/pyorbit/models/spiderman_thermal.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/tinygp_multidimensional_quasiperiodic_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/tinygp_multidimensional_quasiperiodic_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/models/tinygp_quasiperiodic_activity.py` & `pyorbit-package-9.1.9/pyorbit/models/tinygp_quasiperiodic_activity.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/pyorbit_results.py` & `pyorbit-package-9.1.9/pyorbit/pyorbit_results.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/pyorbit_run.py` & `pyorbit-package-9.1.9/pyorbit/pyorbit_run.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_dynesty.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_dynesty.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     if use_default:
         print('Setting up the Dynamic Nested Sampling, number of live points = {0:6.0f}'.format(nlive))
         print('Using default Dynesty hyperparameters')
         print()
     else:
         print('Setting up the Dynamic Nested Sampling, number of live points = {0:6.0f}'.format(nlive))
         print('                                        posterior/evidence split = {0:4.3f}'.format(pfrac_value))
-        print('                                        inizial stopping criterio = {0:5.4f}'.format(dlogz))
+        print('                                        inizial stopping criterion = {0:5.4f}'.format(dlogz))
         print()
 
     if use_threading_pool:
 
         with multiprocessing.Pool() as pool:
             dsampler = dynesty.DynamicNestedSampler(mc.dynesty_call,
                                                     mc.dynesty_priors,
```

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_emcee.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_emcee.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_emcee_mpi.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_emcee_mpi.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_getresults.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_getresults.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_multinest.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_multinest.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_nestle.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_nestle.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_optimize.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_optimize.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_polychord.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_polychord.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_pyde.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_pyde.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_ultranest.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_ultranest.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/samplers/pyorbit_zeus.py` & `pyorbit-package-9.1.9/pyorbit/samplers/pyorbit_zeus.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/common.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,16 @@
         print('ERROR!!! ')
         return None
 
 def pick_sampleMED_parameters(samples, lnprob):
     pams_perc = np.percentile(samples, [15.865, 50, 84.135], axis=0)
     dist_array = 0.0
     for i_pam in range(0, len(samples[0,:])):
-        dist_array += ((samples[:, i_pam]-pams_perc[1, i_pam])/(pams_perc[2,i_pam]-pams_perc[0,i_pam]))**2
+        #dist_array += ((samples[:, i_pam]-pams_perc[1, i_pam])/(pams_perc[2,i_pam]-pams_perc[0,i_pam]))**2
+        dist_array += ((samples[:, i_pam]-pams_perc[1, i_pam])/(np.ptp(samples[:, i_pam])))**2
 
     id_val = np.argmin(dist_array)
     return samples[id_val, :], lnprob[id_val]
 
 def convert_rho_to_a(P, rho):
 
     return np.power(constants.Gsi * (constants.d2s * constants.d2s) * (P**2)
```

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/constants.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/constants.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/input_parser.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/input_parser.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/io_subroutines.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/io_subroutines.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/kepler_exo.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/kepler_exo.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/kepler_old.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/kepler_old.py`

 * *Files identical despite different names*

### Comparing `pyorbit-package-9.1.8/pyorbit/subroutines/results_analysis.py` & `pyorbit-package-9.1.9/pyorbit/subroutines/results_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
                             mc.priors,
                             dataset.prior_kind,
                             dataset.prior_pams)
 
         for model_name in dataset.models:
             if len(mc.models[model_name].sampler_parameters[dataset_name])==0: continue
             print('----- dataset: {0:25s} ----- model: {1:30s}'.format(dataset_name,model_name))
-            print(mc.models[model_name].prior_kind)
-            print(mc.models[model_name].prior_pams)
             print_analysis_info(mc.models[model_name].sampler_parameters[dataset_name],
                                 mc.bounds,
                                 mc.spaces,
                                 mc.priors,
                                 mc.models[model_name].prior_kind[dataset_name],
                                 mc.models[model_name].prior_pams[dataset_name])
```

### Comparing `pyorbit-package-9.1.8/pyorbit_package.egg-info/PKG-INFO` & `pyorbit-package-9.1.9/pyorbit_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorbit-package
-Version: 9.1.8
+Version: 9.1.9
 Summary: PyORBIT: a code for exoplanet orbital parameters and stellar activity
 Home-page: https://github.com/LucaMalavolta/PyORBIT
 Author: Luca Malavolta
 Author-email: luca.malavolta@unipd.it
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -15,19 +15,21 @@
 License-File: LICENSE
 
 
 ![PyORBIT logo](docs/_static/PyORBIT_logo_transp.png?raw=true)
 
 ### A code for exoplanet orbital parameters and stellar activity.
 ***
-### `PyORBIT` version 9.1 by Luca Malavolta - December 2022
+### `PyORBIT` version 9.1 by Luca Malavolta - March 2023
 
 **News**
 
-* Imrpoved output: `spaces`, `bounds`, and `priors` explicitely written out at runtime
+* Added celerite2 SHO term
+
+* Improved output: `spaces`, `bounds`, and `priors` explicitely written out at runtime
 
 * Minor changes:
   * `dataset_variables` and `common_variables` changed to `dataset_parameters`
     and `common_parameters`
   * New models added
   * All instances named `variables` renamed to `parameters` for internal
     consistency. Backward compatibility ensured by new method in `model_container_abstract`
```

### Comparing `pyorbit-package-9.1.8/pyorbit_package.egg-info/SOURCES.txt` & `pyorbit-package-9.1.9/pyorbit_package.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 pyorbit/models/batman_transit_ttv_subset.py
 pyorbit/models/batman_transit_ttv_subset_faster.py
 pyorbit/models/batman_transit_with_ttv.py
 pyorbit/models/celerite2_granulation_oscillation_rotation.py
 pyorbit/models/celerite2_granulation_rotation.py
 pyorbit/models/celerite2_matern32.py
 pyorbit/models/celerite2_rotation.py
+pyorbit/models/celerite2_sho.py
 pyorbit/models/celerite_matern32.py
 pyorbit/models/celerite_matern32_common.py
 pyorbit/models/celerite_rotation.py
 pyorbit/models/celerite_term.py
 pyorbit/models/cheops_detrending.py
 pyorbit/models/cheops_factormodel.py
 pyorbit/models/common_jitter.py
```

### Comparing `pyorbit-package-9.1.8/setup.py` & `pyorbit-package-9.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pyorbit-package",
-    version='9.1.8',
+    version='9.1.9',
     author="Luca Malavolta",
 	author_email = 'luca.malavolta@unipd.it',
 	url = 'https://github.com/LucaMalavolta/PyORBIT',
 	packages =['pyorbit', 'pyorbit.common', 'pyorbit.classes', 'pyorbit.models', 'pyorbit.samplers', 'pyorbit.subroutines'],
 	license = 'MIT License',
 	description ='PyORBIT: a code for exoplanet orbital parameters and stellar activity',
     long_description=long_description,
```

