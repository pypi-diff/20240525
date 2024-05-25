# Comparing `tmp/netbom-0.0.14.tar.gz` & `tmp/netbom-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbom-0.0.14.tar", last modified: Sat May 25 17:45:21 2024, max compression
+gzip compressed data, was "netbom-0.0.15.tar", last modified: Sat May 25 18:03:45 2024, max compression
```

## Comparing `netbom-0.0.14.tar` & `netbom-0.0.15.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.780969 netbom-0.0.14/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.780969 netbom-0.0.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-25 17:45:15.000000 netbom-0.0.14/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-25 17:45:15.000000 netbom-0.0.14/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-25 17:45:15.000000 netbom-0.0.14/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-25 17:45:15.000000 netbom-0.0.14/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 17:45:15.000000 netbom-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-25 17:45:15.000000 netbom-0.0.14/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-25 17:45:21.788969 netbom-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-25 17:45:15.000000 netbom-0.0.14/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 17:45:15.000000 netbom-0.0.14/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.784969 netbom-0.0.14/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.784969 netbom-0.0.14/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    26815 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/figures/Altium_LED-Resistor.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/figures/Altium_LED-Resistor_netlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35851 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/figures/KiCad_LED-Resistor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/netlist.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-25 17:45:15.000000 netbom-0.0.14/docs/netlist_readers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 17:45:15.000000 netbom-0.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 17:45:15.000000 netbom-0.0.14/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 17:45:15.000000 netbom-0.0.14/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 17:45:21.788969 netbom-0.0.14/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.780969 netbom-0.0.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.784969 netbom-0.0.14/src/netbom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/bom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.784969 netbom-0.0.14/src/netbom/bom_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/bom_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/bom_readers/altium_bom_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.784969 netbom-0.0.14/src/netbom/netlist_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/netlist_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-25 17:45:15.000000 netbom-0.0.14/src/netbom/netlist_readers/rinf_netlist_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/src/netbom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-25 17:45:21.000000 netbom-0.0.14/src/netbom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-25 17:45:21.000000 netbom-0.0.14/src/netbom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:45:21.000000 netbom-0.0.14/src/netbom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 17:45:21.000000 netbom-0.0.14/src/netbom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 17:45:21.000000 netbom-0.0.14/src/netbom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 17:45:21.000000 netbom-0.0.14/src/netbom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.780969 netbom-0.0.14/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/tests/examples/bom/
--rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/bom/Altium_LED-Resistor.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/bom/Altium_LT3580-Module.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/tests/examples/netlist/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/netlist/Altium_LED-Resistor.FRP
--rw-r--r--   0 runner    (1001) docker     (127)    24611 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/netlist/Altium_LT3580-Module.FRP
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/netlist/KiCad_LED-Resistor.frp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.780969 netbom-0.0.14/tests/examples/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/tests/examples/projects/Altium_LED-Resistor/
--rw-r--r--   0 runner    (1001) docker     (127)    34887 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb
--rw-r--r--   0 runner    (1001) docker     (127)    35840 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:45:21.788969 netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pcb
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro
--rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/test_bom_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/test_netlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-25 17:45:15.000000 netbom-0.0.14/tests/test_netlist_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.577588 netbom-0.0.15/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.581588 netbom-0.0.15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-25 18:03:35.000000 netbom-0.0.15/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-25 18:03:35.000000 netbom-0.0.15/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-25 18:03:35.000000 netbom-0.0.15/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-25 18:03:35.000000 netbom-0.0.15/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 18:03:35.000000 netbom-0.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-25 18:03:35.000000 netbom-0.0.15/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-25 18:03:45.585588 netbom-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-25 18:03:35.000000 netbom-0.0.15/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 18:03:35.000000 netbom-0.0.15/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.581588 netbom-0.0.15/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.581588 netbom-0.0.15/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    26815 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/figures/Altium_LED-Resistor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/figures/Altium_LED-Resistor_netlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35851 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/figures/KiCad_LED-Resistor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/netlist.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-25 18:03:35.000000 netbom-0.0.15/docs/netlist_readers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 18:03:35.000000 netbom-0.0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 18:03:35.000000 netbom-0.0.15/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 18:03:35.000000 netbom-0.0.15/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 18:03:45.589588 netbom-0.0.15/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.577588 netbom-0.0.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.581588 netbom-0.0.15/src/netbom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/bom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.581588 netbom-0.0.15/src/netbom/bom_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/bom_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/bom_readers/altium_bom_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/src/netbom/netlist_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/netlist_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-25 18:03:35.000000 netbom-0.0.15/src/netbom/netlist_readers/rinf_netlist_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/src/netbom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-25 18:03:45.000000 netbom-0.0.15/src/netbom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-25 18:03:45.000000 netbom-0.0.15/src/netbom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:03:45.000000 netbom-0.0.15/src/netbom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 18:03:45.000000 netbom-0.0.15/src/netbom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 18:03:45.000000 netbom-0.0.15/src/netbom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 18:03:45.000000 netbom-0.0.15/src/netbom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.577588 netbom-0.0.15/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/tests/examples/bom/
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/bom/Altium_LED-Resistor.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/bom/Altium_LT3580-Module.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/tests/examples/netlist/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/netlist/Altium_LED-Resistor.FRP
+-rw-r--r--   0 runner    (1001) docker     (127)    24611 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/netlist/Altium_LT3580-Module.FRP
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/netlist/KiCad_LED-Resistor.frp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.577588 netbom-0.0.15/tests/examples/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/tests/examples/projects/Altium_LED-Resistor/
+-rw-r--r--   0 runner    (1001) docker     (127)    34887 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb
+-rw-r--r--   0 runner    (1001) docker     (127)    35840 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:03:45.585588 netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pcb
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/test_bom_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/test_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-25 18:03:35.000000 netbom-0.0.15/tests/test_netlist_readers.py
```

### Comparing `netbom-0.0.14/.github/workflows/publish.yml` & `netbom-0.0.15/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/.github/workflows/tests.yml` & `netbom-0.0.15/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/.gitignore` & `netbom-0.0.15/.gitignore`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/LICENSE` & `netbom-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/Makefile` & `netbom-0.0.15/Makefile`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/PKG-INFO` & `netbom-0.0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbom
-Version: 0.0.14
+Version: 0.0.15
 Summary: Library to read, convert and process electrical netlists and bill of materials generated in Altium Designer and KiCad.
 Home-page: https://github.com/partmanager/netbom
 Author: Piotr Kuligowski
 Project-URL: Bug Tracker, https://github.com/partmanager/netbom/issues
 Project-URL: Changelog, https://github.com/partmanager/netbom/releases
 Project-URL: Source Code, https://github.com/partmanager/netbom
 Project-URL: Documentation, https://partmanager.github.io/netbom
```

### Comparing `netbom-0.0.14/README.rst` & `netbom-0.0.15/README.rst`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/docs/conf.py` & `netbom-0.0.15/docs/conf.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/docs/figures/Altium_LED-Resistor.svg` & `netbom-0.0.15/docs/figures/Altium_LED-Resistor.svg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/docs/figures/Altium_LED-Resistor_netlist.svg` & `netbom-0.0.15/docs/figures/Altium_LED-Resistor_netlist.svg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/docs/figures/KiCad_LED-Resistor.svg` & `netbom-0.0.15/docs/figures/KiCad_LED-Resistor.svg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/docs/netlist.rst` & `netbom-0.0.15/docs/netlist.rst`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/docs/netlist_readers.rst` & `netbom-0.0.15/docs/netlist_readers.rst`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/requirements-dev.txt` & `netbom-0.0.15/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/setup.cfg` & `netbom-0.0.15/setup.cfg`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/src/netbom/bom.py` & `netbom-0.0.15/src/netbom/bom.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/src/netbom/bom_readers/altium_bom_reader.py` & `netbom-0.0.15/src/netbom/bom_readers/altium_bom_reader.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/src/netbom/netlist.py` & `netbom-0.0.15/src/netbom/netlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,22 +175,20 @@
 
 class NetlistDesignator:
     def __init__(self, designator: str, pin_net: dict) -> None:
         self._designator = designator
         self._items = pin_net
 
     def append(self, pin_net: dict) -> None:
-        """Method appending new {pin: net} pairs, deduplicating
-        and sorting them.
+        """Method appending new {pin: net} pairs and deduplicating them.
 
         :param pin_net: {pin: net} dictionary
         :type pin_net: dict
         """
         self._items.update(pin_net)
-        self._items = dict(sorted(self._items.items()))
 
     def to_dict(self) -> dict:
         """Method converting NetlistDesignator to dict.
 
         :return: NetlistDesignator converted to dict.
         :rtype: dict
         """
```

### Comparing `netbom-0.0.14/src/netbom/netlist_readers/rinf_netlist_reader.py` & `netbom-0.0.15/src/netbom/netlist_readers/rinf_netlist_reader.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/src/netbom.egg-info/PKG-INFO` & `netbom-0.0.15/src/netbom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbom
-Version: 0.0.14
+Version: 0.0.15
 Summary: Library to read, convert and process electrical netlists and bill of materials generated in Altium Designer and KiCad.
 Home-page: https://github.com/partmanager/netbom
 Author: Piotr Kuligowski
 Project-URL: Bug Tracker, https://github.com/partmanager/netbom/issues
 Project-URL: Changelog, https://github.com/partmanager/netbom/releases
 Project-URL: Source Code, https://github.com/partmanager/netbom
 Project-URL: Documentation, https://partmanager.github.io/netbom
```

### Comparing `netbom-0.0.14/src/netbom.egg-info/SOURCES.txt` & `netbom-0.0.15/src/netbom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/bom/Altium_LED-Resistor.xlsx` & `netbom-0.0.15/tests/examples/bom/Altium_LED-Resistor.xlsx`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/bom/Altium_LT3580-Module.xlsx` & `netbom-0.0.15/tests/examples/bom/Altium_LT3580-Module.xlsx`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/netlist/Altium_LED-Resistor.FRP` & `netbom-0.0.15/tests/examples/netlist/Altium_LED-Resistor.FRP`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/netlist/Altium_LT3580-Module.FRP` & `netbom-0.0.15/tests/examples/netlist/Altium_LT3580-Module.FRP`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb` & `netbom-0.0.15/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.PrjPcb`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc` & `netbom-0.0.15/tests/examples/projects/Altium_LED-Resistor/Altium_LED-Resistor.SchDoc`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl` & `netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_prl`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro` & `netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_pro`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch` & `netbom-0.0.15/tests/examples/projects/KiCad_LED-Resistor/KiCad_LED-Resistor.kicad_sch`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/test_bom.py` & `netbom-0.0.15/tests/test_bom.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/test_bom_readers.py` & `netbom-0.0.15/tests/test_bom_readers.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/test_netlist.py` & `netbom-0.0.15/tests/test_netlist.py`

 * *Files identical despite different names*

### Comparing `netbom-0.0.14/tests/test_netlist_readers.py` & `netbom-0.0.15/tests/test_netlist_readers.py`

 * *Files identical despite different names*

