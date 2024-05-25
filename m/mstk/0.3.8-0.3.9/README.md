# Comparing `tmp/mstk-0.3.8.tar.gz` & `tmp/mstk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mstk-0.3.8.tar", last modified: Sun Feb  4 14:52:30 2024, max compression
+gzip compressed data, was "mstk-0.3.9.tar", last modified: Sun Feb 25 13:10:32 2024, max compression
```

## Comparing `mstk-0.3.8.tar` & `mstk-0.3.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.781879 mstk-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-02-04 14:52:21.000000 mstk-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-04 14:52:30.781879 mstk-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-04 14:52:21.000000 mstk-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.761879 mstk-0.3.8/mstk/
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.765879 mstk-0.3.8/mstk/analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/canny.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/energy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/ewald.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/neighborlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/analyzer/vle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.765879 mstk-0.3.8/mstk/chem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/chem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/chem/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/chem/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/chem/formula.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/chem/rdkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.761879 mstk-0.3.8/mstk/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.769879 mstk-0.3.8/mstk/data/forcefield/
--rw-r--r--   0 runner    (1001) docker     (127)    80183 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/data/forcefield/SPICA_v1.zfp
--rw-r--r--   0 runner    (1001) docker     (127)   525802 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/data/forcefield/gaff.zff
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/data/forcefield/gaff.zft
--rw-r--r--   0 runner    (1001) docker     (127)   527008 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/data/forcefield/gaff_mod.zff
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/data/forcefield/primitive.zff
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/data/forcefield/primitive.zft
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.769879 mstk-0.3.8/mstk/forcefield/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/dff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    50992 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/ffterm.py
--rw-r--r--   0 runner    (1001) docker     (127)    36032 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/forcefield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.769879 mstk-0.3.8/mstk/forcefield/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/io/padua.py
--rw-r--r--   0 runner    (1001) docker     (127)     9327 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/io/ppf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/io/zff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/io/zfp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.769879 mstk-0.3.8/mstk/forcefield/typer/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/typer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/typer/gaff_typer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/typer/typer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/forcefield/typer/zft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.769879 mstk-0.3.8/mstk/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/misc/docmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/misc/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.769879 mstk-0.3.8/mstk/ommhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/force.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/grofile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.773879 mstk-0.3.8/mstk/ommhelper/reporter/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/reporter/checkpointreporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/reporter/drudetemperaturereporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/reporter/groreporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22849 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/reporter/statedatareporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/reporter/viscosityreporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/ommhelper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.773879 mstk-0.3.8/mstk/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/scheduler/pbsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/scheduler/remote_slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.773879 mstk-0.3.8/mstk/simsys/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/simsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18745 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/simsys/gmxexporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/simsys/lmpexporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/simsys/namdexporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31291 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/simsys/ommexporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    21437 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/simsys/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.777879 mstk-0.3.8/mstk/topology/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.777879 mstk-0.3.8/mstk/topology/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/gro.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/msd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/smi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/io/zmat.py
--rw-r--r--   0 runner    (1001) docker     (127)    55472 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/residue.py
--rw-r--r--   0 runner    (1001) docker     (127)    22771 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/unitcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/topology/virtualsite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.777879 mstk-0.3.8/mstk/trajectory/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.777879 mstk-0.3.8/mstk/trajectory/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/combined_trj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/dcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/gro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/xtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/io/xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/trajectory/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.777879 mstk-0.3.8/mstk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.781879 mstk-0.3.8/mstk/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/wrapper/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)    40192 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/wrapper/gmx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-02-04 14:52:21.000000 mstk-0.3.8/mstk/wrapper/packmol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.781879 mstk-0.3.8/mstk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-04 14:52:30.000000 mstk-0.3.8/mstk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-02-04 14:52:30.000000 mstk-0.3.8/mstk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 14:52:30.000000 mstk-0.3.8/mstk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-04 14:52:30.000000 mstk-0.3.8/mstk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:52:30.781879 mstk-0.3.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5497 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/analyze-rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/ffconv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8075 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/logplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6891 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/sim-build.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5550 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/sim-export.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3336 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/topconv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3558 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/trjconv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4211 2024-02-04 14:52:21.000000 mstk-0.3.8/scripts/wham-pp.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 14:52:30.781879 mstk-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-04 14:52:21.000000 mstk-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.792016 mstk-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-02-25 13:10:24.000000 mstk-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-25 13:10:32.792016 mstk-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-25 13:10:24.000000 mstk-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.772016 mstk-0.3.9/mstk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.776016 mstk-0.3.9/mstk/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/canny.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/energy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/ewald.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/neighborlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/analyzer/vle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.776016 mstk-0.3.9/mstk/chem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/chem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/chem/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/chem/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/chem/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/chem/rdkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.772016 mstk-0.3.9/mstk/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.780016 mstk-0.3.9/mstk/data/forcefield/
+-rw-r--r--   0 runner    (1001) docker     (127)    80183 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/data/forcefield/SPICA_v1.zfp
+-rw-r--r--   0 runner    (1001) docker     (127)   525802 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/data/forcefield/gaff.zff
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/data/forcefield/gaff.zft
+-rw-r--r--   0 runner    (1001) docker     (127)   527008 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/data/forcefield/gaff_mod.zff
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/data/forcefield/primitive.zff
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/data/forcefield/primitive.zft
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.780016 mstk-0.3.9/mstk/forcefield/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/dff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50992 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/ffterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36032 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/forcefield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.780016 mstk-0.3.9/mstk/forcefield/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15881 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/io/padua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9327 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/io/ppf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/io/zff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/io/zfp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.780016 mstk-0.3.9/mstk/forcefield/typer/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/typer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/typer/gaff_typer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/typer/typer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/forcefield/typer/zft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.780016 mstk-0.3.9/mstk/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/misc/docmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/misc/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.780016 mstk-0.3.9/mstk/ommhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/grofile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.784016 mstk-0.3.9/mstk/ommhelper/reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/reporter/checkpointreporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/reporter/drudetemperaturereporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/reporter/groreporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23765 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/reporter/statedatareporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/reporter/viscosityreporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/ommhelper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.784016 mstk-0.3.9/mstk/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/scheduler/pbsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/scheduler/remote_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.784016 mstk-0.3.9/mstk/simsys/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/simsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18745 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/simsys/gmxexporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/simsys/lmpexporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/simsys/namdexporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31291 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/simsys/ommexporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21435 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/simsys/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.788016 mstk-0.3.9/mstk/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.788016 mstk-0.3.9/mstk/topology/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/gro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/msd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/smi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/io/zmat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55546 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22771 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/unitcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/topology/virtualsite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.788016 mstk-0.3.9/mstk/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.788016 mstk-0.3.9/mstk/trajectory/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/combined_trj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/dcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/gro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/xtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/io/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/trajectory/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.788016 mstk-0.3.9/mstk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.792016 mstk-0.3.9/mstk/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/wrapper/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40192 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/wrapper/gmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-02-25 13:10:24.000000 mstk-0.3.9/mstk/wrapper/packmol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.792016 mstk-0.3.9/mstk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-25 13:10:32.000000 mstk-0.3.9/mstk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-02-25 13:10:32.000000 mstk-0.3.9/mstk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 13:10:32.000000 mstk-0.3.9/mstk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-25 13:10:32.000000 mstk-0.3.9/mstk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 13:10:32.792016 mstk-0.3.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5497 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/analyze-rdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/ffconv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8075 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/logplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6891 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/sim-build.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5528 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/sim-export.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3336 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/topconv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3558 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/trjconv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4211 2024-02-25 13:10:24.000000 mstk-0.3.9/scripts/wham-pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 13:10:32.792016 mstk-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-25 13:10:24.000000 mstk-0.3.9/setup.py
```

### Comparing `mstk-0.3.8/LICENSE` & `mstk-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/PKG-INFO` & `mstk-0.3.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-Metadata-Version: 2.1
-Name: mstk
-Version: 0.3.8
-Summary: Molecular simulation toolkit
-Home-page: https://github.com/z-gong/mstk
-Author: Zheng Gong
-Author-email: z.gong@outlook.com
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # mstk
 
-A toolkit to make molecular simulation less painful
+_A toolkit to make molecular simulation less painful_
+
+`mstk` is a Python toolkit designed to streamline the setup and management of molecular simulations, particularly geared
+towards non-biological applications in material science and chemical engineering. It simplifies atom typing, force field
+parameter assignment, and input file generation for major simulation engines.
 
-## Capabilities
+## Features
 
 * Assign atom types and force field parameters based on local chemical environment
-* Generate input files for simulation engines like LAMMPS, GROMACS, NAMD, OpenMM
+* Generate input files for LAMMPS, GROMACS, NAMD and OpenMM
 * Support Drude polarizable model, coarse-grained model, virtual site, linear angle...
-* Read/write common topology files (LAMMPS, PSF, PDB, ZMAT etc...)
-* Read/write common trajectory files (LAMMPS, GRO, DCD, XTC, etc...)
+* Read/write common topology (PSF, ZMAT, PDB, LAMMPS, ...) and trajectory (GRO, XTC, DCD, LAMMPS, ...) files
 * Access local and remote job schedulers like Slurm
 
-## Examples
+## Installation
 
-The following code builds a liquid mixture of 100 benzene and 1000 water molecules, ready for simulation.
+```
+conda install -c conda-forge numpy pandas rdkit openmm chemfiles packmol
+pip install mstk
+```
+
+## Quick Example
+
+Build a liquid mixture of 100 benzene and 1000 water molecules, ready for simulation.
 
 ```python
 from mstk.topology import Molecule, Topology
 from mstk.forcefield import ForceField, ZftTyper
 from mstk.simsys import System
 from mstk.wrapper import Packmol
 
-# Create molecule structures from SMILES
+# Create topology from SMILES
 benzene = Molecule.from_smiles('c1ccccc1')
 water = Molecule.from_smiles('O')
 top = Topology([benzene, water])
 
-# Assign atom type as defined in `data/forcefield/primitive.zft`
+# Assign atom types as defined in `data/forcefield/primitive.zft`
 typer = ZftTyper('primitive.zft')
 typer.type(top)
 
 # Build a bulk liquid simulation box with Packmol
-packmol = Packmol('/path/to/packmol')
+packmol = Packmol('packmol')
 top.cell.set_box([4.0, 4.0, 4.0])
 top.scale_with_packmol([100, 1000], packmol=packmol)
 
-# Assign force field as defined in `data/forcefield/primitive.zff`
+# Assign force field parameters as defined in `data/forcefield/primitive.zff`
 ff = ForceField.open('primitive.zff')
 ff.assign_charge(top)
 system = System(top, ff)
 
-# generate input files for LAMMPS, GROMACS and NAMD
+# Generate input files for LAMMPS, GROMACS and NAMD
 system.export_lammps()
 system.export_gromacs()
 system.export_namd()
 
-# generate OpenMM system and topology
+# Generate OpenMM system and topology
 omm_sys = system.to_omm_system()
 omm_top = top.to_omm_topology()
 ```
 
+__Important Note__:
+*The __primitive__ atom typing and force field used above are for demonstration purpose only and are __not__ well
+optimized for production use.*
+*For reliable simulation, please prepare you own `zft` and `zff` files or get them from a validated source.*
+
 ## Documentation
 
 https://mstk.readthedocs.io/en/latest/index.html
 
 ## TODO
 
 - [ ] Take bond order into consideration for force field assignment
-- [ ] Add frozen marker in ZFF and ZFP for force field optimization
-- [ ] Re-organize algorithms scattered in topology and analyzer modules
+- [ ] Add frozen marker in `ZFF` and `ZFP` for force field optimization
+- [ ] Refactor algorithms across `topology` and `analyzer` modules
+- [ ] Separate `ommhelper` module into its own package
+- [ ] Remove `analyzer` module
 
 ## Known issue
 
-`mstk` use `chemfiles` to write `XTC` trajectory. However, lastest `chemfiles` fails writing binary trajectory format
-under WSL 1. If you are using WSL 1, please install `chemfiles 0.10.2`
+`mstk` use `chemfiles` to handle `XTC` trajectory. Latest `chemfiles` fails writing binary trajectory format under WSL 1.
+If you are using WSL 1, please install `chemfiles 0.10.2`
 
 ```
-conda install chemfiles-lib=0.10.2 chemfiles-python=0.10.2
+conda install -c conda-forge chemfiles-lib=0.10.2 chemfiles-python=0.10.2
 ```
```

### Comparing `mstk-0.3.8/README.md` & `mstk-0.3.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,100 @@
+Metadata-Version: 2.1
+Name: mstk
+Version: 0.3.9
+Summary: Molecular simulation toolkit
+Home-page: https://github.com/z-gong/mstk
+Author: Zheng Gong
+Author-email: z.gong@outlook.com
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mstk
 
-A toolkit to make molecular simulation less painful
+_A toolkit to make molecular simulation less painful_
+
+`mstk` is a Python toolkit designed to streamline the setup and management of molecular simulations, particularly geared
+towards non-biological applications in material science and chemical engineering. It simplifies atom typing, force field
+parameter assignment, and input file generation for major simulation engines.
 
-## Capabilities
+## Features
 
 * Assign atom types and force field parameters based on local chemical environment
-* Generate input files for simulation engines like LAMMPS, GROMACS, NAMD, OpenMM
+* Generate input files for LAMMPS, GROMACS, NAMD and OpenMM
 * Support Drude polarizable model, coarse-grained model, virtual site, linear angle...
-* Read/write common topology files (LAMMPS, PSF, PDB, ZMAT etc...)
-* Read/write common trajectory files (LAMMPS, GRO, DCD, XTC, etc...)
+* Read/write common topology (PSF, ZMAT, PDB, LAMMPS, ...) and trajectory (GRO, XTC, DCD, LAMMPS, ...) files
 * Access local and remote job schedulers like Slurm
 
-## Examples
+## Installation
 
-The following code builds a liquid mixture of 100 benzene and 1000 water molecules, ready for simulation.
+```
+conda install -c conda-forge numpy pandas rdkit openmm chemfiles packmol
+pip install mstk
+```
+
+## Quick Example
+
+Build a liquid mixture of 100 benzene and 1000 water molecules, ready for simulation.
 
 ```python
 from mstk.topology import Molecule, Topology
 from mstk.forcefield import ForceField, ZftTyper
 from mstk.simsys import System
 from mstk.wrapper import Packmol
 
-# Create molecule structures from SMILES
+# Create topology from SMILES
 benzene = Molecule.from_smiles('c1ccccc1')
 water = Molecule.from_smiles('O')
 top = Topology([benzene, water])
 
-# Assign atom type as defined in `data/forcefield/primitive.zft`
+# Assign atom types as defined in `data/forcefield/primitive.zft`
 typer = ZftTyper('primitive.zft')
 typer.type(top)
 
 # Build a bulk liquid simulation box with Packmol
-packmol = Packmol('/path/to/packmol')
+packmol = Packmol('packmol')
 top.cell.set_box([4.0, 4.0, 4.0])
 top.scale_with_packmol([100, 1000], packmol=packmol)
 
-# Assign force field as defined in `data/forcefield/primitive.zff`
+# Assign force field parameters as defined in `data/forcefield/primitive.zff`
 ff = ForceField.open('primitive.zff')
 ff.assign_charge(top)
 system = System(top, ff)
 
-# generate input files for LAMMPS, GROMACS and NAMD
+# Generate input files for LAMMPS, GROMACS and NAMD
 system.export_lammps()
 system.export_gromacs()
 system.export_namd()
 
-# generate OpenMM system and topology
+# Generate OpenMM system and topology
 omm_sys = system.to_omm_system()
 omm_top = top.to_omm_topology()
 ```
 
+__Important Note__:
+*The __primitive__ atom typing and force field used above are for demonstration purpose only and are __not__ well
+optimized for production use.*
+*For reliable simulation, please prepare you own `zft` and `zff` files or get them from a validated source.*
+
 ## Documentation
 
 https://mstk.readthedocs.io/en/latest/index.html
 
 ## TODO
 
 - [ ] Take bond order into consideration for force field assignment
-- [ ] Add frozen marker in ZFF and ZFP for force field optimization
-- [ ] Re-organize algorithms scattered in topology and analyzer modules
+- [ ] Add frozen marker in `ZFF` and `ZFP` for force field optimization
+- [ ] Refactor algorithms across `topology` and `analyzer` modules
+- [ ] Separate `ommhelper` module into its own package
+- [ ] Remove `analyzer` module
 
 ## Known issue
 
-`mstk` use `chemfiles` to write `XTC` trajectory. However, lastest `chemfiles` fails writing binary trajectory format
-under WSL 1. If you are using WSL 1, please install `chemfiles 0.10.2`
+`mstk` use `chemfiles` to handle `XTC` trajectory. Latest `chemfiles` fails writing binary trajectory format under WSL 1.
+If you are using WSL 1, please install `chemfiles 0.10.2`
 
 ```
-conda install chemfiles-lib=0.10.2 chemfiles-python=0.10.2
+conda install -c conda-forge chemfiles-lib=0.10.2 chemfiles-python=0.10.2
 ```
```

### Comparing `mstk-0.3.8/mstk/__init__.py` & `mstk-0.3.9/mstk/__init__.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/canny.py` & `mstk-0.3.9/mstk/analyzer/canny.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/energy_kernels.py` & `mstk-0.3.9/mstk/analyzer/energy_kernels.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/ewald.py` & `mstk-0.3.9/mstk/analyzer/ewald.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/fitting.py` & `mstk-0.3.9/mstk/analyzer/fitting.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/neighborlist.py` & `mstk-0.3.9/mstk/analyzer/neighborlist.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/series.py` & `mstk-0.3.9/mstk/analyzer/series.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/structure.py` & `mstk-0.3.9/mstk/analyzer/structure.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/analyzer/vle.py` & `mstk-0.3.9/mstk/analyzer/vle.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/chem/element.py` & `mstk-0.3.9/mstk/chem/element.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/chem/formula.py` & `mstk-0.3.9/mstk/chem/formula.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/chem/rdkit.py` & `mstk-0.3.9/mstk/chem/rdkit.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/data/forcefield/SPICA_v1.zfp` & `mstk-0.3.9/mstk/data/forcefield/SPICA_v1.zfp`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/data/forcefield/gaff.zff` & `mstk-0.3.9/mstk/data/forcefield/gaff.zff`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/data/forcefield/gaff.zft` & `mstk-0.3.9/mstk/data/forcefield/gaff.zft`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/data/forcefield/gaff_mod.zff` & `mstk-0.3.9/mstk/data/forcefield/gaff_mod.zff`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/data/forcefield/primitive.zff` & `mstk-0.3.9/mstk/data/forcefield/primitive.zff`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/dff_utils.py` & `mstk-0.3.9/mstk/forcefield/dff_utils.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/ffterm.py` & `mstk-0.3.9/mstk/forcefield/ffterm.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/forcefield.py` & `mstk-0.3.9/mstk/forcefield/forcefield.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/io/padua.py` & `mstk-0.3.9/mstk/forcefield/io/padua.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/io/ppf.py` & `mstk-0.3.9/mstk/forcefield/io/ppf.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/io/zff.py` & `mstk-0.3.9/mstk/forcefield/io/zff.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/io/zfp.py` & `mstk-0.3.9/mstk/forcefield/io/zfp.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/typer/gaff_typer.py` & `mstk-0.3.9/mstk/forcefield/typer/gaff_typer.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/typer/typer.py` & `mstk-0.3.9/mstk/forcefield/typer/typer.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/forcefield/typer/zft.py` & `mstk-0.3.9/mstk/forcefield/typer/zft.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/misc/docmeta.py` & `mstk-0.3.9/mstk/misc/docmeta.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/force.py` & `mstk-0.3.9/mstk/ommhelper/force.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/grofile.py` & `mstk-0.3.9/mstk/ommhelper/grofile.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/reporter/checkpointreporter.py` & `mstk-0.3.9/mstk/ommhelper/reporter/checkpointreporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/reporter/drudetemperaturereporter.py` & `mstk-0.3.9/mstk/ommhelper/reporter/drudetemperaturereporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/reporter/groreporter.py` & `mstk-0.3.9/mstk/ommhelper/reporter/groreporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/reporter/statedatareporter.py` & `mstk-0.3.9/mstk/ommhelper/reporter/statedatareporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 
 class StateDataReporter(object):
     '''
     StateDataReporter outputs information about a simulation, such as energy and temperature, to a file.
 
     This reporter is modified from the StateDataReporter shipped with OpenMM python API.
-    It adds support for reporting box size and collective variables.
+    It adds support for reporting pressure, energy contribution of individual force group, collective variables and box size.
 
     To use it, create a StateDataReporter, then add it to the Simulation's list of reporters.  The set of
     data to write is configurable using boolean flags passed to the constructor.  By default the data is
     written in comma-separated-value (CSV) format, but you can specify a different separator to use.
 
     Parameters
     ----------
@@ -113,23 +113,29 @@
         particle masses do not reflect their actual physical mass, such as
         when some particles have had their masses set to 0 to immobilize
         them.
     totalSteps : int=None
         The total number of steps that will be included in the simulation.
         This is required if either progress or remainingTime is set to True,
         and defines how many steps will indicate 100% completion.
+    forceGroups : list=[]
+        Write the energy contribution of each force group in this list separately
     cvs : list=[]
-        Collective variables defined by CustomCVForce
+        Write the value of each collective variable in this list separately.
+        Each element is a CustomCVForce object
+    extra : dict={}
+        Write extra data from a dictionary. The keys will be used as header names.
+        The values can change during the simulation.
     '''
 
     def __init__(self, file, reportInterval, step=True, time=False, potentialEnergy=True,
-                 kineticEnergy=False, totalEnergy=False, temperature=True, volume=True, box=True,
+                 kineticEnergy=False, totalEnergy=False, temperature=True, volume=False, box=True,
                  density=True, progress=False, remainingTime=False, speed=True, elapsedTime=False,
                  separator='\t', systemMass=None, totalSteps=None, append=False,
-                 cvs=None, pressure=True, pxx=False, pyy=False, pzz=False, extra={}):
+                 pressure=True, pxx=False, pyy=False, pzz=False, forceGroups=None, cvs=None, extra=None):
         self._reportInterval = reportInterval
         self._openedFile = isinstance(file, str)
         if (progress or remainingTime) and totalSteps is None:
             raise ValueError(
                 'Reporting progress or remaining time requires total steps to be specified')
         if self._openedFile:
             if append:
@@ -160,20 +166,21 @@
         self._needsVelocities = False
         self._needsForces = False
         self._needEnergy = potentialEnergy or kineticEnergy or totalEnergy or temperature \
                            or pressure or pxx or pyy or pzz
 
         self._boxSizeList = [[], [], []]
 
-        self._cvs = cvs or []
         self._pressure = pressure
         self._pxx = pxx
         self._pyy = pyy
         self._pzz = pzz
-        self._extra = extra
+        self._forceGroups = forceGroups or []
+        self._cvs = cvs or []
+        self._extra = extra or {}
 
     def describeNextReport(self, simulation):
         """Get information about the next report this object will generate.
 
         Parameters
         ----------
         simulation : Simulation
@@ -198,15 +205,15 @@
         simulation : Simulation
             The Simulation to generate a report for
         state : State
             The current state of the simulation
         """
         if not self._hasInitialized:
             self._initializeConstants(simulation)
-            headers = self._constructHeaders()
+            headers = self._constructHeaders(simulation)
             print('#"%s"' % ('"' + self._separator + '"').join(headers), file=self._out)
             try:
                 self._out.flush()
             except AttributeError:
                 pass
             self._initialClockTime = time.time()
             self._initialSimulationTime = state.getTime()
@@ -305,21 +312,23 @@
                     value = "%d:%02d:%02d" % (remainingHours, remainingMinutes, remainingSeconds)
                 elif remainingMinutes > 0:
                     value = "%d:%02d" % (remainingMinutes, remainingSeconds)
                 else:
                     value = "0:%02d" % remainingSeconds
             values.append(value)
 
-        for cv in self._cvs:
-            values.append(cv.getCollectiveVariableValues(simulation.context)[0])
-
         bool_press = [self._pxx, self._pyy, self._pzz]
         if any(bool_press):
             values.extend(self._compute_anisotropic_pressure(simulation.context, state, *bool_press))
 
+        for group in self._forceGroups:
+            values.append(simulation.context.getState(getEnergy=True, groups={group}).getPotentialEnergy().
+                          value_in_unit(unit.kilojoules_per_mole))
+        for cv in self._cvs:
+            values.append(cv.getCollectiveVariableValues(simulation.context)[0])
         if self._extra:
             values.extend(self._extra.values())
 
         self._boxSizeList[0].append(box[0][0].value_in_unit(unit.nanometer)),
         self._boxSizeList[1].append(box[1][1].value_in_unit(unit.nanometer)),
         self._boxSizeList[2].append(box[2][2].value_in_unit(unit.nanometer)),
 
@@ -364,15 +373,15 @@
                 matrix = np.zeros([n_atom, n_atom], dtype=bool)
                 for i in range(system.getNumConstraints()):
                     a1, a2, d = system.getConstraintParameters(i)
                     matrix[a1][a2] = True
                     matrix[a2][a1] = True
                 self._constrained_groups = find_clusters(list(range(n_atom)), lambda x, y: matrix[x][y])
 
-    def _constructHeaders(self):
+    def _constructHeaders(self, simulation):
         """Construct the headers for the CSV output
 
         Returns: a list of strings giving the title of each observable being reported on.
         """
         headers = []
         if self._progress:
             headers.append('Progress')
@@ -400,22 +409,25 @@
             headers.append('Density')
         if self._speed:
             headers.append('Speed')
         if self._elapsedTime:
             headers.append('Elapsed')
         if self._remainingTime:
             headers.append('Remaining')
-        for i, cv in enumerate(self._cvs):
-            headers.append('CV%i' % i)
         if self._pxx:
             headers.append('Pxx')
         if self._pyy:
             headers.append('Pyy')
         if self._pzz:
             headers.append('Pzz')
+        for group in self._forceGroups:
+            names = set(force.getName() for force in simulation.system.getForces() if force.getForceGroup() == group)
+            headers.append(f'E_{group}_{"+".join(names)}')
+        for i, cv in enumerate(self._cvs):
+            headers.append(f'CV_{i}')
         if self._extra:
             headers.extend(self._extra.keys())
         return headers
 
     def _checkForErrors(self, simulation, state):
         """Check for errors in the current state of the simulation
```

### Comparing `mstk-0.3.8/mstk/ommhelper/reporter/viscosityreporter.py` & `mstk-0.3.9/mstk/ommhelper/reporter/viscosityreporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/ommhelper/utils.py` & `mstk-0.3.9/mstk/ommhelper/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def minimize(sim, tolerance, gro_out=None, logger=None):
     '''
     Run energy minimization on a Simulation until the force on each atom is smaller than tolerance.
 
     Note that the tolerance here differs from that in OpenMM LocalEnergyMinimizer.
-    In OpenMM, the tolerance is set for the root mean square of N*3 force components in the whole system.
+    In OpenMM, the tolerance is set for the root-mean-square of N*3 force components in the whole system.
 
     Parameters
     ----------
     sim : app.Simulation
     tolerance : float
     gro_out : str
     logger : Logger
@@ -63,16 +63,16 @@
     if gro_out:
         GroFile.writeFile(sim.topology, state.getPositions(), state.getPeriodicBoxVectors(), gro_out)
 
 
 def apply_mc_barostat(system, pcoupl, P, T, nstep=100, rigid_molecule=True, logger=None):
     '''
     Add a MonteCarlo barostat to the system and return the added barostat
-    
-    #TODO It requires the forked OpenMM https://github.com/openmm/openmm/pull/3797
+
+    TODO It requires the forked OpenMM https://github.com/openmm/openmm/pull/3797
 
     Parameters
     ----------
     system : mm.System
     pcoupl : str
         The type of barostat. Can be one of the following: iso, semi-iso, aniso, xy, z.
     P : float
@@ -103,42 +103,53 @@
     elif pcoupl == 'xy':
         msg = 'Anisotropic barostat only for X and Y'
         force = mm.MonteCarloAnisotropicBarostat([P * bar] * 3, T * kelvin, True, True, False, nstep, rigid_molecule)
     elif pcoupl == 'z':
         msg = 'Anisotropic barostat only for Z'
         force = mm.MonteCarloAnisotropicBarostat([P * bar] * 3, T * kelvin, False, False, True, nstep, rigid_molecule)
     else:
-        raise Exception('Available pressure coupling types: iso, semi-iso, xyz, xy, z')
+        raise Exception('Available pressure coupling types: iso, semi-iso, aniso, xy, z')
 
     scaled_unit = 'molecules' if rigid_molecule else 'constrained groups'
     msg += f' with {scaled_unit} scaled'
 
     if logger:
         logger.info(msg)
 
     system.addForce(force)
 
     return force
 
 
 def energy_decomposition(sim: app.Simulation, logger=None):
-    groups = {}
+    '''
+    Get the energy contribution of different force groups
+
+    Parameters
+    ----------
+    sim : app.Simulation
+    logger : Logger
+
+    Returns
+    -------
+    energies : Dict[str, float]
+        The name and energy contribution of each force group
+    '''
+    groups = {}  # {id_group: {force1_name, force2_name, ...}, ...}
     for force in sim.system.getForces():
         i = force.getForceGroup()
         if i not in groups:
             groups[i] = set()
         groups[i].add(force.getName())
 
     energies = {}
     for i in sorted(groups.keys()):
         energy = sim.context.getState(getEnergy=True, groups={i}).getPotentialEnergy()._value
         if energy != 0 or i != 0:
-            name = '+'.join(groups[i])
-            if name in energies:
-                name += f'_{i}'
+            name = f'{i}_{"+".join(groups[i])}'
             energies[name] = energy
 
     if logger:
         for k, v in energies.items():
             logger.info(f'E_{k} = {v}')
 
     return energies
```

### Comparing `mstk-0.3.8/mstk/scheduler/pbsjob.py` & `mstk-0.3.9/mstk/scheduler/pbsjob.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/scheduler/remote_slurm.py` & `mstk-0.3.9/mstk/scheduler/remote_slurm.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/scheduler/scheduler.py` & `mstk-0.3.9/mstk/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/scheduler/slurm.py` & `mstk-0.3.9/mstk/scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/simsys/gmxexporter.py` & `mstk-0.3.9/mstk/simsys/gmxexporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/simsys/lmpexporter.py` & `mstk-0.3.9/mstk/simsys/lmpexporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/simsys/namdexporter.py` & `mstk-0.3.9/mstk/simsys/namdexporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,41 +23,41 @@
     Usually it is acceptable if the improper to be described is planer and quite rigid.
     '''
 
     def __init__(self):
         pass
 
     @staticmethod
-    def export(system, pdb_out, psf_out, prm_out, pdb_atom_type=False, **kwargs):
+    def export(system, pdb_out, psf_out, prm_out, **kwargs):
         '''
         Generate input files for NAMD from a system
 
         Parameters
         ----------
         system : System
         pdb_out : str or None
         psf_out : str or None
         prm_out : str or None
         '''
         if not system.use_pbc:
             raise Exception('PBC required for exporting NAMD')
 
         if pdb_out is not None:
-            NamdExporter._export_pdb(system, pdb_out, atom_type=pdb_atom_type)
+            NamdExporter._export_pdb(system, pdb_out)
         if psf_out is not None:
             NamdExporter._export_psf(system, psf_out)
         if prm_out is not None:
             NamdExporter._export_prm(system, prm_out)
 
     @staticmethod
-    def _export_pdb(system, pdb_out='conf.pdb', atom_type=False):
-        Pdb.save_to(system.topology, pdb_out, atom_type=atom_type)
+    def _export_pdb(system, pdb_out='conf.pdb'):
+        Pdb.save_to(system.topology, pdb_out)
 
     @staticmethod
-    def _export_psf(system, psf_out='topol.psf'):
+    def _export_psf(system, psf_out='top.psf'):
         Psf.save_to(system.topology, psf_out)
 
     @staticmethod
     def _export_prm(system: System, prm_out='ff.prm'):
         supported_terms = {LJ126Term,
                            HarmonicBondTerm,
                            HarmonicAngleTerm,
```

### Comparing `mstk-0.3.8/mstk/simsys/ommexporter.py` & `mstk-0.3.9/mstk/simsys/ommexporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/simsys/system.py` & `mstk-0.3.9/mstk/simsys/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         gro_out : str or None
         top_out : str or None
         mdp_out : str or None
         '''
         from .gmxexporter import GromacsExporter
         GromacsExporter.export(self, gro_out, top_out, mdp_out, **kwargs)
 
-    def export_namd(self, pdb_out='conf.pdb', psf_out='topol.psf', prm_out='ff.prm', **kwargs):
+    def export_namd(self, pdb_out='conf.pdb', psf_out='top.psf', prm_out='ff.prm', **kwargs):
         '''
         Generate input files for NAMD
 
         Parameters
         ----------
         pdb_out : str or None
         psf_out : str or None
```

### Comparing `mstk-0.3.8/mstk/topology/atom.py` & `mstk-0.3.9/mstk/topology/atom.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/connectivity.py` & `mstk-0.3.9/mstk/topology/connectivity.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/geometry.py` & `mstk-0.3.9/mstk/topology/geometry.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/gro.py` & `mstk-0.3.9/mstk/topology/io/gro.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/lammps.py` & `mstk-0.3.9/mstk/topology/io/lammps.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/msd.py` & `mstk-0.3.9/mstk/topology/io/msd.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/pdb.py` & `mstk-0.3.9/mstk/topology/io/pdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,24 +135,22 @@
             else:
                 self.topology.update_molecules(pieces)
         else:
             raise Exception(f'Invalid option for split_molecule: {split_molecule}')
         self.topology.generate_angle_dihedral_improper()
 
     @staticmethod
-    def save_to(top, file, atom_type=False, **kwargs):
+    def save_to(top, file, **kwargs):
         '''
         Save topology into a PDB file
 
         Parameters
         ----------
         top : Topology
         file : str
-        atom_type : bool
-            If True, atom type will be written in the atom name column, which is useful for visualizing
         '''
         if not top.has_position:
             raise Exception('Position is required for writing PDB file')
 
         if top.n_atom > 99999:
             logger.warning('Number of atoms exceeds the maximum supported by PDB (99999)')
 
@@ -167,19 +165,18 @@
         string = 'REMARK   Created by mstk\n'
         string += 'CRYST1%9s%9s%9s%7s%7s%7s P 1           1 \n' % (
             *(format_float(x, 9, 3) for x in lengths),
             *(format_float(x * RAD2DEG, 7, 2) for x in angles))
 
         for atom in top.atoms:
             pos = atom.position * 10  # convert from nm to A
-            atom_name = atom.type if atom_type else atom.name
             resname = atom.residue.name
             resid = atom.residue.id + 1
             line = 'HETATM%5d %4s %-4s %4d    %8s%8s%8s                      %2s\n' % (
-                (atom.id + 1) % 100000, atom_name[:4], resname[:4], resid % 10000,
+                (atom.id + 1) % 100000, atom.name[:4], resname[:4], resid % 10000,
                 *[format_float(x, 8, 3) for x in pos], atom.symbol[:2])
             string += line
 
         for atom in top.atoms:
             partners = [a for a in atom.bond_partners if a.id > atom.id]
             if len(partners) > 0:
                 line = 'CONECT%5d' % ((atom.id + 1) % 100000)
```

### Comparing `mstk-0.3.8/mstk/topology/io/psf.py` & `mstk-0.3.9/mstk/topology/io/psf.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/smi.py` & `mstk-0.3.9/mstk/topology/io/smi.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/xyz.py` & `mstk-0.3.9/mstk/topology/io/xyz.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/io/zmat.py` & `mstk-0.3.9/mstk/topology/io/zmat.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/molecule.py` & `mstk-0.3.9/mstk/topology/molecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,19 +128,22 @@
         smiles : str
 
         Returns
         -------
         molecule : Molecule
         '''
         words = smiles.strip().split()
+        if not words:
+            raise Exception('Invalid SMILES string')
+
         smiles = words[0]
         if len(words) > 1:
             name = words[1]
         else:
-            name = smiles
+            name = None
 
         rdmol = create_mol_from_smiles(smiles)
         mol = Molecule.from_rdmol(rdmol, name)
 
         return mol
 
     @staticmethod
```

### Comparing `mstk-0.3.8/mstk/topology/residue.py` & `mstk-0.3.9/mstk/topology/residue.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/topology.py` & `mstk-0.3.9/mstk/topology/topology.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/unitcell.py` & `mstk-0.3.9/mstk/topology/unitcell.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/topology/virtualsite.py` & `mstk-0.3.9/mstk/topology/virtualsite.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/frame.py` & `mstk-0.3.9/mstk/trajectory/frame.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/handler.py` & `mstk-0.3.9/mstk/trajectory/handler.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/io/combined_trj.py` & `mstk-0.3.9/mstk/trajectory/io/combined_trj.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/io/dcd.py` & `mstk-0.3.9/mstk/trajectory/io/dcd.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/io/gro.py` & `mstk-0.3.9/mstk/trajectory/io/gro.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/io/lammps.py` & `mstk-0.3.9/mstk/trajectory/io/lammps.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/io/xtc.py` & `mstk-0.3.9/mstk/trajectory/io/xtc.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/io/xyz.py` & `mstk-0.3.9/mstk/trajectory/io/xyz.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/trajectory/trajectory.py` & `mstk-0.3.9/mstk/trajectory/trajectory.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/utils/__init__.py` & `mstk-0.3.9/mstk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/wrapper/gauss.py` & `mstk-0.3.9/mstk/wrapper/gauss.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/wrapper/gmx.py` & `mstk-0.3.9/mstk/wrapper/gmx.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk/wrapper/packmol.py` & `mstk-0.3.9/mstk/wrapper/packmol.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/mstk.egg-info/PKG-INFO` & `mstk-0.3.9/mstk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,100 @@
 Metadata-Version: 2.1
 Name: mstk
-Version: 0.3.8
+Version: 0.3.9
 Summary: Molecular simulation toolkit
 Home-page: https://github.com/z-gong/mstk
 Author: Zheng Gong
 Author-email: z.gong@outlook.com
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mstk
 
-A toolkit to make molecular simulation less painful
+_A toolkit to make molecular simulation less painful_
 
-## Capabilities
+`mstk` is a Python toolkit designed to streamline the setup and management of molecular simulations, particularly geared
+towards non-biological applications in material science and chemical engineering. It simplifies atom typing, force field
+parameter assignment, and input file generation for major simulation engines.
+
+## Features
 
 * Assign atom types and force field parameters based on local chemical environment
-* Generate input files for simulation engines like LAMMPS, GROMACS, NAMD, OpenMM
+* Generate input files for LAMMPS, GROMACS, NAMD and OpenMM
 * Support Drude polarizable model, coarse-grained model, virtual site, linear angle...
-* Read/write common topology files (LAMMPS, PSF, PDB, ZMAT etc...)
-* Read/write common trajectory files (LAMMPS, GRO, DCD, XTC, etc...)
+* Read/write common topology (PSF, ZMAT, PDB, LAMMPS, ...) and trajectory (GRO, XTC, DCD, LAMMPS, ...) files
 * Access local and remote job schedulers like Slurm
 
-## Examples
+## Installation
+
+```
+conda install -c conda-forge numpy pandas rdkit openmm chemfiles packmol
+pip install mstk
+```
+
+## Quick Example
 
-The following code builds a liquid mixture of 100 benzene and 1000 water molecules, ready for simulation.
+Build a liquid mixture of 100 benzene and 1000 water molecules, ready for simulation.
 
 ```python
 from mstk.topology import Molecule, Topology
 from mstk.forcefield import ForceField, ZftTyper
 from mstk.simsys import System
 from mstk.wrapper import Packmol
 
-# Create molecule structures from SMILES
+# Create topology from SMILES
 benzene = Molecule.from_smiles('c1ccccc1')
 water = Molecule.from_smiles('O')
 top = Topology([benzene, water])
 
-# Assign atom type as defined in `data/forcefield/primitive.zft`
+# Assign atom types as defined in `data/forcefield/primitive.zft`
 typer = ZftTyper('primitive.zft')
 typer.type(top)
 
 # Build a bulk liquid simulation box with Packmol
-packmol = Packmol('/path/to/packmol')
+packmol = Packmol('packmol')
 top.cell.set_box([4.0, 4.0, 4.0])
 top.scale_with_packmol([100, 1000], packmol=packmol)
 
-# Assign force field as defined in `data/forcefield/primitive.zff`
+# Assign force field parameters as defined in `data/forcefield/primitive.zff`
 ff = ForceField.open('primitive.zff')
 ff.assign_charge(top)
 system = System(top, ff)
 
-# generate input files for LAMMPS, GROMACS and NAMD
+# Generate input files for LAMMPS, GROMACS and NAMD
 system.export_lammps()
 system.export_gromacs()
 system.export_namd()
 
-# generate OpenMM system and topology
+# Generate OpenMM system and topology
 omm_sys = system.to_omm_system()
 omm_top = top.to_omm_topology()
 ```
 
+__Important Note__:
+*The __primitive__ atom typing and force field used above are for demonstration purpose only and are __not__ well
+optimized for production use.*
+*For reliable simulation, please prepare you own `zft` and `zff` files or get them from a validated source.*
+
 ## Documentation
 
 https://mstk.readthedocs.io/en/latest/index.html
 
 ## TODO
 
 - [ ] Take bond order into consideration for force field assignment
-- [ ] Add frozen marker in ZFF and ZFP for force field optimization
-- [ ] Re-organize algorithms scattered in topology and analyzer modules
+- [ ] Add frozen marker in `ZFF` and `ZFP` for force field optimization
+- [ ] Refactor algorithms across `topology` and `analyzer` modules
+- [ ] Separate `ommhelper` module into its own package
+- [ ] Remove `analyzer` module
 
 ## Known issue
 
-`mstk` use `chemfiles` to write `XTC` trajectory. However, lastest `chemfiles` fails writing binary trajectory format
-under WSL 1. If you are using WSL 1, please install `chemfiles 0.10.2`
+`mstk` use `chemfiles` to handle `XTC` trajectory. Latest `chemfiles` fails writing binary trajectory format under WSL 1.
+If you are using WSL 1, please install `chemfiles 0.10.2`
 
 ```
-conda install chemfiles-lib=0.10.2 chemfiles-python=0.10.2
+conda install -c conda-forge chemfiles-lib=0.10.2 chemfiles-python=0.10.2
 ```
```

### Comparing `mstk-0.3.8/mstk.egg-info/SOURCES.txt` & `mstk-0.3.9/mstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/analyze-rdf.py` & `mstk-0.3.9/scripts/analyze-rdf.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/ffconv.py` & `mstk-0.3.9/scripts/ffconv.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/logplot.py` & `mstk-0.3.9/scripts/logplot.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/sim-build.py` & `mstk-0.3.9/scripts/sim-build.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/sim-export.py` & `mstk-0.3.9/scripts/sim-export.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         except Exception as e:
             logger.error('Failed exporting GROMACS')
             traceback.print_exc()
 
     if args.namd or args.all:
         logger.info('Exporting NAMD...')
         try:
-            system.export_namd(pdb_out='_namd-conf.pdb', psf_out='_namd-topol.psf', prm_out=None, pdb_atom_type=True)
+            system.export_namd(pdb_out='_namd-conf.pdb', psf_out='_namd-top.psf', prm_out=None)
         except Exception as e:
             logger.error('Failed exporting NAMD')
             traceback.print_exc()
 
     if args.openmm or args.all:
         logger.info('Exporting OpenMM...')
         try:
```

### Comparing `mstk-0.3.8/scripts/topconv.py` & `mstk-0.3.9/scripts/topconv.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/trjconv.py` & `mstk-0.3.9/scripts/trjconv.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/scripts/wham-pp.py` & `mstk-0.3.9/scripts/wham-pp.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.8/setup.py` & `mstk-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 dir_scripts = 'scripts'
 scripts = [os.path.join(dir_scripts, f) for f in os.listdir(dir_scripts)]
 
 setuptools.setup(
     name='mstk',
-    version='0.3.8',
+    version='0.3.9',
     author='Zheng Gong',
     author_email='z.gong@outlook.com',
     description='Molecular simulation toolkit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/z-gong/mstk',
     packages=setuptools.find_packages(),
```

