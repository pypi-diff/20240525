# Comparing `tmp/kfactory-0.9.2.tar.gz` & `tmp/kfactory-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.9.2.tar", last modified: Fri Oct  6 13:43:54 2023, max compression
+gzip compressed data, was "kfactory-0.9.3.tar", last modified: Fri Oct  6 14:10:31 2023, max compression
```

## Comparing `kfactory-0.9.2.tar` & `kfactory-0.9.3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.758207 kfactory-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-10-06 13:43:37.000000 kfactory-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-06 13:43:37.000000 kfactory-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-06 13:43:37.000000 kfactory-0.9.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-06 13:43:37.000000 kfactory-0.9.2/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-06 13:43:37.000000 kfactory-0.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-06 13:43:37.000000 kfactory-0.9.2/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-06 13:43:37.000000 kfactory-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2023-10-06 13:43:37.000000 kfactory-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-06 13:43:37.000000 kfactory-0.9.2/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2023-10-06 13:43:37.000000 kfactory-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-06 13:43:37.000000 kfactory-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-10-06 13:43:37.000000 kfactory-0.9.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-06 13:43:54.758207 kfactory-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-10-06 13:43:37.000000 kfactory-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-10-06 13:43:37.000000 kfactory-0.9.2/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.718207 kfactory-0.9.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.722207 kfactory-0.9.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   138035 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   985194 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (127)   129785 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/config.md
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/dosdonts.md
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/gdsfactory.md
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.726207 kfactory-0.9.2/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/notebooks/04_KCL.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/notebooks/demo.gds
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/pre.md
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/star.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-10-06 13:43:37.000000 kfactory-0.9.2/docs/source/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2023-10-06 13:43:37.000000 kfactory-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 13:43:54.758207 kfactory-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.714207 kfactory-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.730207 kfactory-0.9.2/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.734207 kfactory-0.9.2/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.734207 kfactory-0.9.2/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/dbu/straight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/straight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cells/taper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.738207 kfactory-0.9.2/src/kfactory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cli/runshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/cli/sea.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    56615 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (127)   153274 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.738207 kfactory-0.9.2/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20414 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.738207 kfactory-0.9.2/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.742207 kfactory-0.9.2/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.742207 kfactory-0.9.2/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15081 2023-10-06 13:43:37.000000 kfactory-0.9.2/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.730207 kfactory-0.9.2/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-06 13:43:54.000000 kfactory-0.9.2/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-06 13:43:54.000000 kfactory-0.9.2/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 13:43:54.000000 kfactory-0.9.2/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-06 13:43:54.000000 kfactory-0.9.2/src/kfactory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-06 13:43:54.000000 kfactory-0.9.2/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-06 13:43:54.000000 kfactory-0.9.2/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.750207 kfactory-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_cplxcells.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.714207 kfactory-0.9.2/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:43:54.754207 kfactory-0.9.2/tests/test_data/ref/
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A180_AS1.gds
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A90_AS1.gds
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A180_R150.gds
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A90_R150.gds
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_data/ref/Straight_W500_L1000_LWG_EWGSTD.gds
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_data/ref/taper.gds
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_netlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-10-06 13:43:37.000000 kfactory-0.9.2/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.511182 kfactory-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.483181 kfactory-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.483181 kfactory-0.9.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2023-10-06 14:10:00.000000 kfactory-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-06 14:10:00.000000 kfactory-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-06 14:10:00.000000 kfactory-0.9.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.483181 kfactory-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-06 14:10:00.000000 kfactory-0.9.3/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-06 14:10:00.000000 kfactory-0.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-06 14:10:00.000000 kfactory-0.9.3/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-06 14:10:00.000000 kfactory-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2023-10-06 14:10:00.000000 kfactory-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-06 14:10:00.000000 kfactory-0.9.3/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2023-10-06 14:10:00.000000 kfactory-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-10-06 14:10:00.000000 kfactory-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-10-06 14:10:00.000000 kfactory-0.9.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-06 14:10:31.507182 kfactory-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-10-06 14:10:00.000000 kfactory-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.487181 kfactory-0.9.3/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-10-06 14:10:00.000000 kfactory-0.9.3/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.487181 kfactory-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.487181 kfactory-0.9.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.487181 kfactory-0.9.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.491181 kfactory-0.9.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   138035 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   985194 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (127)   129785 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/dosdonts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9791 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/gdsfactory.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.491181 kfactory-0.9.3/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/notebooks/04_KCL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/notebooks/demo.gds
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2023-10-06 14:10:00.000000 kfactory-0.9.3/docs/source/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2023-10-06 14:10:00.000000 kfactory-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 14:10:31.511182 kfactory-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.479181 kfactory-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.491181 kfactory-0.9.3/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.495181 kfactory-0.9.3/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.495181 kfactory-0.9.3/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/dbu/straight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10932 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/straight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cells/taper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.495181 kfactory-0.9.3/src/kfactory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cli/runshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/cli/sea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56616 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (127)   153274 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.495181 kfactory-0.9.3/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20414 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.499181 kfactory-0.9.3/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.499181 kfactory-0.9.3/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.499181 kfactory-0.9.3/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15081 2023-10-06 14:10:00.000000 kfactory-0.9.3/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.495181 kfactory-0.9.3/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-06 14:10:31.000000 kfactory-0.9.3/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-06 14:10:31.000000 kfactory-0.9.3/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 14:10:31.000000 kfactory-0.9.3/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-06 14:10:31.000000 kfactory-0.9.3/src/kfactory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-06 14:10:31.000000 kfactory-0.9.3/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-06 14:10:31.000000 kfactory-0.9.3/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.503182 kfactory-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_cplxcells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.483181 kfactory-0.9.3/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 14:10:31.503182 kfactory-0.9.3/tests/test_data/ref/
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A180_AS1.gds
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A90_AS1.gds
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A180_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A90_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_data/ref/Straight_W500_L1000_LWG_EWGSTD.gds
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_data/ref/taper.gds
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-10-06 14:10:00.000000 kfactory-0.9.3/tests/test_spiral.py
```

### Comparing `kfactory-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/.github/workflows/pages.yml` & `kfactory-0.9.3/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/.github/workflows/release.yml` & `kfactory-0.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/.github/workflows/test_code.yml` & `kfactory-0.9.3/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/.pre-commit-config.yaml` & `kfactory-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/CHANGELOG.md` & `kfactory-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the changes for the upcoming release can be found in <https://github.com/gdsfactory/kfactory/tree/main/changelog.d/>.
 
 <!-- towncrier release notes start -->
 
+## [0.9.3](https://github.com/gdsfactory/kfactory/releases/v0.9.3) - 2023-10-06
+
+
+### Fixed
+
+- Fixed layer enclosure errors in extrude_path
+
+
 ## [0.9.2](https://github.com/gdsfactory/kfactory/releases/v0.9.2) - 2023-10-06
 
 No significant changes.
 
 
 ## [0.9.1](https://github.com/gdsfactory/kfactory/releases/v0.9.1) - 2023-10-04
```

### Comparing `kfactory-0.9.2/LICENSE` & `kfactory-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/Makefile` & `kfactory-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/PKG-INFO` & `kfactory-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.9.2
+Version: 0.9.3
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,22 +61,22 @@
 Requires-Dist: kfactory[git]; extra == "ci"
 Provides-Extra: ipy
 Requires-Dist: ipython; extra == "ipy"
 Requires-Dist: ipywidgets; extra == "ipy"
 Requires-Dist: ipytree; extra == "ipy"
 Requires-Dist: ipyevents; extra == "ipy"
 
-# KFactory 0.9.2
+# KFactory 0.9.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.9.2` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.9.3` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.9.2/README.md` & `kfactory-0.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# KFactory 0.9.2
+# KFactory 0.9.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.9.2` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.9.3` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.9.2/docs/mkdocs.yml` & `kfactory-0.9.3/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/_static/complex.png` & `kfactory-0.9.3/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/_static/klive.webm` & `kfactory-0.9.3/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/_static/waveguide.png` & `kfactory-0.9.3/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/complex_cell.py` & `kfactory-0.9.3/docs/source/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/config.md` & `kfactory-0.9.3/docs/source/config.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/gdsfactory.md` & `kfactory-0.9.3/docs/source/gdsfactory.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/gen_ref_pages.py` & `kfactory-0.9.3/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/intro.md` & `kfactory-0.9.3/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/notebooks/00_geometry.py` & `kfactory-0.9.3/docs/source/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/notebooks/01_references.py` & `kfactory-0.9.3/docs/source/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/notebooks/02_DRC.py` & `kfactory-0.9.3/docs/source/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/notebooks/03_Enclosures.py` & `kfactory-0.9.3/docs/source/notebooks/03_Enclosures.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/notebooks/04_KCL.py` & `kfactory-0.9.3/docs/source/notebooks/04_KCL.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/notebooks/demo.gds` & `kfactory-0.9.3/docs/source/notebooks/demo.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/pre.md` & `kfactory-0.9.3/docs/source/pre.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/star.py` & `kfactory-0.9.3/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/docs/source/waveguide.py` & `kfactory-0.9.3/docs/source/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/pyproject.toml` & `kfactory-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.9.2"
+version = "0.9.3"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.12",
 	"scipy",
 	"ruamel.yaml",
@@ -243,15 +243,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.9.2"
+current = "0.9.3"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `kfactory-0.9.2/src/kfactory/__init__.py` & `kfactory-0.9.3/src/kfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from . import cells, placer, routing, port, technology, enclosure, utils
 from .conf import config
 from .enclosure import LayerEnclosure, KCellEnclosure
 
 from aenum import constant  # type: ignore[import]
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
```

### Comparing `kfactory-0.9.2/src/kfactory/cells/bezier.py` & `kfactory-0.9.3/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cells/circular.py` & `kfactory-0.9.3/src/kfactory/cells/circular.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cells/dbu/straight.py` & `kfactory-0.9.3/src/kfactory/cells/dbu/straight.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cells/dbu/taper.py` & `kfactory-0.9.3/src/kfactory/cells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cells/euler.py` & `kfactory-0.9.3/src/kfactory/cells/euler.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cells/straight.py` & `kfactory-0.9.3/src/kfactory/cells/straight.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cells/taper.py` & `kfactory-0.9.3/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cli/__init__.py` & `kfactory-0.9.3/src/kfactory/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cli/runshow.py` & `kfactory-0.9.3/src/kfactory/cli/runshow.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/cli/sea.py` & `kfactory-0.9.3/src/kfactory/cli/sea.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/conf.py` & `kfactory-0.9.3/src/kfactory/conf.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/enclosure.py` & `kfactory-0.9.3/src/kfactory/enclosure.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                         end_angle,
                     )
                 )
                 _r -= kdb.Region(_path.to_itype(target.kcl.dbu))
             reg.insert(_r)
             if _layer == layer and i == j:
                 ret_path = _path
-        target.shapes(layer).insert(reg.merge())
+        target.shapes(_layer).insert(reg.merge())
     return ret_path
 
 
 def extrude_path_dynamic_points(
     path: list[kdb.DPoint],
     widths: Callable[[float], float] | list[float],
     start_angle: float | None = None,
```

### Comparing `kfactory-0.9.2/src/kfactory/kcell.py` & `kfactory-0.9.3/src/kfactory/kcell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/placer.py` & `kfactory-0.9.3/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/port.py` & `kfactory-0.9.3/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/routing/electrical.py` & `kfactory-0.9.3/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/routing/manhattan.py` & `kfactory-0.9.3/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/routing/optical.py` & `kfactory-0.9.3/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/technology/layer_map.py` & `kfactory-0.9.3/src/kfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/utils/__init__.py` & `kfactory-0.9.3/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/utils/fill.py` & `kfactory-0.9.3/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/utils/simplify.py` & `kfactory-0.9.3/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/utils/violations.py` & `kfactory-0.9.3/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory/widgets/interactive.py` & `kfactory-0.9.3/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.9.3/src/kfactory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.9.2
+Version: 0.9.3
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,22 +61,22 @@
 Requires-Dist: kfactory[git]; extra == "ci"
 Provides-Extra: ipy
 Requires-Dist: ipython; extra == "ipy"
 Requires-Dist: ipywidgets; extra == "ipy"
 Requires-Dist: ipytree; extra == "ipy"
 Requires-Dist: ipyevents; extra == "ipy"
 
-# KFactory 0.9.2
+# KFactory 0.9.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.9.2` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.9.3` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.9.2/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.9.3/src/kfactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/src/kfactory.egg-info/requires.txt` & `kfactory-0.9.3/src/kfactory.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/conftest.py` & `kfactory-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_cell.py` & `kfactory-0.9.3/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_cells.py` & `kfactory-0.9.3/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_cplxcells.py` & `kfactory-0.9.3/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A180_AS1.gds` & `kfactory-0.9.3/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A180_AS1.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A90_AS1.gds` & `kfactory-0.9.3/tests/test_data/ref/BendCircular_W1_R10_LWG_EWGSTD_A90_AS1.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A180_R150.gds` & `kfactory-0.9.3/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A180_R150.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A90_R150.gds` & `kfactory-0.9.3/tests/test_data/ref/BendEuler_W1_R10_LWG_EWGSTD_A90_R150.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_data/ref/Straight_W500_L1000_LWG_EWGSTD.gds` & `kfactory-0.9.3/tests/test_data/ref/Straight_W500_L1000_LWG_EWGSTD.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_data/ref/taper.gds` & `kfactory-0.9.3/tests/test_data/ref/taper.gds`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_enclosure.py` & `kfactory-0.9.3/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_extrude.py` & `kfactory-0.9.3/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_meta.py` & `kfactory-0.9.3/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_netlist.py` & `kfactory-0.9.3/tests/test_netlist.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_partial.py` & `kfactory-0.9.3/tests/test_partial.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_pdk.py` & `kfactory-0.9.3/tests/test_pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_ports.py` & `kfactory-0.9.3/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_rename.py` & `kfactory-0.9.3/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_routing.py` & `kfactory-0.9.3/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.9.2/tests/test_spiral.py` & `kfactory-0.9.3/tests/test_spiral.py`

 * *Files identical despite different names*

