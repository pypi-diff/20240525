# Comparing `tmp/cogsworth-0.0.tar.gz` & `tmp/cogsworth-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsworth-0.0.tar", last modified: Mon May 29 19:34:50 2023, max compression
+gzip compressed data, was "cogsworth-1.0.0.tar", last modified: Sat May 25 02:10:29 2024, max compression
```

## Comparing `cogsworth-0.0.tar` & `cogsworth-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,43 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-29 19:34:49.994664 cogsworth-0.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2023-03-19 06:18:35.000000 cogsworth-0.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)      882 2023-05-29 19:34:49.994664 cogsworth-0.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      494 2023-05-29 19:34:06.000000 cogsworth-0.0/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-29 19:34:49.994664 cogsworth-0.0/cogsworth/
--rw-rw-r--   0 tom       (1000) tom       (1000)       97 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       20 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/_version.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    15391 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/classify.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4042 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/events.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20950 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/galaxy.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8051 2023-05-10 05:08:13.000000 cogsworth-0.0/cogsworth/kicks.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    13353 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/observables.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    47012 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/pop.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-29 19:34:49.994664 cogsworth-0.0/cogsworth/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/tests/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      478 2023-03-19 06:18:35.000000 cogsworth-0.0/cogsworth/tests/prep_data.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1774 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/tests/test_classify.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1704 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/tests/test_events.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5749 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/tests/test_galaxy.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1230 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/tests/test_observables.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7828 2023-05-28 18:17:07.000000 cogsworth-0.0/cogsworth/tests/test_pop.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-29 19:34:49.994664 cogsworth-0.0/cogsworth.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)      882 2023-05-29 19:34:49.000000 cogsworth-0.0/cogsworth.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      583 2023-05-29 19:34:49.000000 cogsworth-0.0/cogsworth.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-29 19:34:49.000000 cogsworth-0.0/cogsworth.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      248 2023-05-29 19:34:49.000000 cogsworth-0.0/cogsworth.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-05-29 19:34:49.000000 cogsworth-0.0/cogsworth.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1161 2023-05-29 19:34:49.994664 cogsworth-0.0/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)      453 2023-05-28 18:17:07.000000 cogsworth-0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:10:29.830574 cogsworth-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 02:10:20.000000 cogsworth-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-25 02:10:29.830574 cogsworth-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-25 02:10:20.000000 cogsworth-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:10:29.826574 cogsworth-1.0.0/cogsworth/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:10:29.826574 cogsworth-1.0.0/cogsworth/hydro/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/hydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/hydro/pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/hydro/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/hydro/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/hydro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/kicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14292 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68026 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40428 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/sfh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:10:29.830574 cogsworth-1.0.0/cogsworth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/optional_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_kicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/tests/test_pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-25 02:10:20.000000 cogsworth-1.0.0/cogsworth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:10:29.826574 cogsworth-1.0.0/cogsworth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-25 02:10:29.000000 cogsworth-1.0.0/cogsworth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 02:10:29.000000 cogsworth-1.0.0/cogsworth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:10:29.000000 cogsworth-1.0.0/cogsworth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-25 02:10:29.000000 cogsworth-1.0.0/cogsworth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 02:10:29.000000 cogsworth-1.0.0/cogsworth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-25 02:10:29.830574 cogsworth-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-25 02:10:21.000000 cogsworth-1.0.0/setup.py
```

### Comparing `cogsworth-0.0/LICENSE` & `cogsworth-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsworth-0.0/PKG-INFO` & `cogsworth-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: cogsworth
-Version: 0.0
+Version: 1.0.0
 Summary: A framework for performing self-consistent population synthesis and orbital integration
 Home-page: https://github.com/TomWagg/cogsworth
 Author: Tom Wagg
 Author-email: tomjwagg@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: extras
+Provides-Extra: observables
+Provides-Extra: actions
+Provides-Extra: lisa
+Provides-Extra: hydro
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 
 <h1 align="center">Cogsworth</h1>
-<p align="center">A Python package for self-consistently performing population synthesis and orbital integration</p>
+<p align="center">A Python package for performing self-consistent population synthesis and galactic dynamics simulations</p>
 <p align="center">
   <a href='https://cogsworth.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/cogsworth/badge/?version=latest' alt='Documentation Status' />
 </a>
   <br>
   <img width=500 src="https://user-images.githubusercontent.com/21990332/194442782-49afc013-2c53-4638-bcb7-c0970319c2bd.png">
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: cogsworth Version: 0.0 Summary: A framework for
+Metadata-Version: 2.1 Name: cogsworth Version: 1.0.0 Summary: A framework for
 performing self-consistent population synthesis and orbital integration Home-
 page: https://github.com/TomWagg/cogsworth Author: Tom Wagg Author-email:
 tomjwagg@gmail.com License: MIT Requires-Python: >=3.10 Description-Content-
-Type: text/markdown Provides-Extra: test Provides-Extra: docs License-File:
-LICENSE
+Type: text/markdown Provides-Extra: all Provides-Extra: extras Provides-Extra:
+observables Provides-Extra: actions Provides-Extra: lisa Provides-Extra: hydro
+Provides-Extra: test Provides-Extra: docs License-File: LICENSE
                             ************ CCooggsswwoorrtthh ************
-  A Python package for self-consistently performing population synthesis and
-                              orbital integration
+   A Python package for performing self-consistent population synthesis and
+                         galactic dynamics simulations
                             _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
  [https://user-images.githubusercontent.com/21990332/194442782-49afc013-2c53-
                           4638-bcb7-c0970319c2bd.png]
```

### Comparing `cogsworth-0.0/cogsworth/classify.py` & `cogsworth-1.0.0/cogsworth/classify.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,68 +4,64 @@
 import astropy.constants as const
 import gala.dynamics as gd
 
 __all__ = ["determine_final_classes", "list_classes", "get_eddington_rate", "get_eddington_lum",
            "get_schwarzchild_radius", "get_x_ray_lum"]
 
 
-def determine_final_classes(population=None, bpp=None, bcm=None, kick_info=None, orbits=None, potential=None):
+def determine_final_classes(population=None, bpp=None, kick_info=None, orbits=None, potential=None):
     """Determine the classes of each member of a population at the last point in the evolution (usually
     present day).
 
-    Either supply a Population class or each individual table separately
+    Either supply a :class:`~cogsworth.pop.Population` class or each individual table separately
 
     Parameters
     ----------
     population : :class:`~cogsworth.pop.Population`, optional
         A full population class created from the pop module, by default None
     bpp : :class:`~pandas.DataFrame`
         Evolutionary history of each binary
-    bcm : :class:`~pandas.DataFrame`
-        Final state of each binary
     initC : :class:`~pandas.DataFrame`
         Initial conditions for each binary
     kick_info : :class:`~pandas.DataFrame`
         Information about the kicks that occur for each binary
     orbits : `list` of :class:`~gala.dynamics.Orbit`
         The orbits of each binary within the galaxy. Disrupted binaries should have two entries
-        (for both stars).
-    galactic_potential : :class:`~gala.potential.potential.PotentialBase`, optional
+        (for both stars), where the secondary is appended in sequence to the full list.
+    galactic_potential : :class:`Potential <gala.potential.potential.PotentialBase>`, optional
         Galactic potential to use for evolving the orbits of binaries
 
     Returns
     -------
     classes : :class:`~pandas.DataFrame`
         A DataFrame with a boolean column for each class (see :meth:`list_classes`) and a row for each binary
 
     Raises
     ------
     ValueError
         If either `population` is None OR any another parameter is None
     """
     # ensure that there's enough input
-    if population is None and (bpp is None or bcm is None or kick_info is None
-                               or orbits is None or potential is None):
+    if population is None and (bpp is None or kick_info is None or orbits is None or potential is None):
         raise ValueError("Either `population` must be supplied or all other parameters")
 
     # split up the input so that I can use a single interface
     if population is not None:
-        bpp, bcm, kick_info, orbits, potential = population.bpp, population.bcm, population.kick_info,\
+        bpp, kick_info, orbits, potential = population.bpp, population.kick_info, \
             population.orbits, population.galactic_potential
 
     # get the binary indices and also reduce the tables to just the final row in each
     final_bpp = bpp[~bpp.index.duplicated(keep="last")]
-    final_bcm = bcm[~bcm.index.duplicated(keep="last")]
     final_kick_info = kick_info.sort_values(["bin_num", "star"]).drop_duplicates(subset="bin_num",
                                                                                  keep="last")
 
     # set up an empty dataframe
     columns = ["dco", "co-1", "co-2", "xrb", "walkaway-t-1", "walkaway-t-2", "runaway-t-1", "runaway-t-2",
                "walkaway-o-1", "walkaway-o-2", "runaway-o-1", "runaway-o-2", "widow-1", "widow-2",
-               "stellar-merger-co-1", "stellar-merger-co-2", "pisn-1", "pisn-2"]
+               "stellar-merger-co-1", "stellar-merger-co-2"]
     data = np.zeros(shape=(len(final_bpp), len(columns))).astype(bool)
     classes = pd.DataFrame(data=data, columns=columns)
 
     # match the index to the final bpp bin_nums
     classes.index = final_bpp["bin_num"].index
 
     # check the state of the binary
@@ -96,60 +92,55 @@
     classes["stellar-merger-co-1"] = merger & primary_is_bh_ns
     classes["stellar-merger-co-2"] = merger & secondary_is_bh_ns
     classes["xrb"] = bound & ((primary_is_bh_ns & secondary_is_star) | (secondary_is_bh_ns & primary_is_star))
 
     classes["widow-1"] = ~merger & primary_is_star & secondary_ever_bound_bh_ns
     classes["widow-2"] = ~merger & secondary_is_star & primary_ever_bound_bh_ns
 
-    classes["pisn-1"] = final_bcm["SN_1"].isin([6, 7])
-    classes["pisn-2"] = final_bcm["SN_2"].isin([6, 7])
-
     classes["walkaway-t-1"] = disrupted & (final_kick_info["vsys_1_total"] < 30.0) & primary_is_star
     classes["walkaway-t-2"] = disrupted & (final_kick_info["vsys_2_total"] < 30.0) & secondary_is_star
     classes["runaway-t-1"] = disrupted & (final_kick_info["vsys_1_total"] >= 30.0) & primary_is_star
     classes["runaway-t-2"] = disrupted & (final_kick_info["vsys_2_total"] >= 30.0) & secondary_is_star
 
     # calculate relative speeds for observed walk/runaways
     if disrupted.any():
-        rel_speed_1 = _get_rel_speed(orbits=orbits[disrupted], potential=potential, which_star=0)
-        rel_speed_2 = _get_rel_speed(orbits=orbits[disrupted], potential=potential, which_star=1)
+        rel_speed_1 = _get_rel_speed(orbits=orbits[:len(final_bpp)][disrupted], potential=potential)
+        rel_speed_2 = _get_rel_speed(orbits=orbits[len(final_bpp):], potential=potential)
 
         # set the classes based on the relative speeds (non-disrupted as all left as False by default)
         classes.loc[disrupted, "walkaway-o-1"] = (rel_speed_1 < 30.0) & primary_is_star[disrupted]
         classes.loc[disrupted, "walkaway-o-2"] = (rel_speed_2 < 30.0) & secondary_is_star[disrupted]
         classes.loc[disrupted, "runaway-o-1"] = (rel_speed_1 >= 30.0) & primary_is_star[disrupted]
         classes.loc[disrupted, "runaway-o-2"] = (rel_speed_2 >= 30.0) & secondary_is_star[disrupted]
 
     return classes
 
 
-def _get_rel_speed(orbits, potential, which_star):
+def _get_rel_speed(orbits, potential):
     """Calculate the relative speed of a set of stars at the end of their orbits compared to the circular
     velocity at their final positions (given a galactic potential)
 
     Parameters
     ----------
     orbits : `list`
         List of gala Orbits
     potential : :class:`gala.potential.potential.PotentialBase`
         The galactic potential used for finding the circular velocity
-    which_star : `int`
-        Index of which star to consider, either 0 or 1
 
     Returns
     -------
     rel_speed : `float`
         Relative speed in km / s
     """
     # get final positions and velocities
     posf = [None for _ in range(len(orbits))]
     velf = [None for _ in range(len(orbits))]
     for i, orbit in enumerate(orbits):
-        posf[i] = orbit[which_star][-1].pos.xyz.to(u.kpc).value
-        velf[i] = orbit[which_star][-1].vel.d_xyz.to(u.km / u.s)
+        posf[i] = orbit[-1].pos.xyz.to(u.kpc).value
+        velf[i] = orbit[-1].vel.d_xyz.to(u.km / u.s)
     posf *= u.kpc
     velf *= u.km / u.s
 
     # create gala phase space positions based on them
     wf = gd.PhaseSpacePosition(pos=posf.T, vel=velf.T)
 
     # calculate the circular velocities at those locations
@@ -219,19 +210,14 @@
             "condition": ("Any bound binary of two compact objects")
         },
         {
             "name": "sdIa",
             "full_name": "Single degenerate type Ia",
             "condition": ("Any disrupted binary that contains a massless remnant that was once a white dwarf")
         },
-        {
-            "name": "pisn",
-            "full_name": "Pair Instability Supernova",
-            "condition": ("Any binary that had a star with a pair instability supernova")
-        },
     ]
 
     print("Any class with a suffix '-1' or '-2' applies to only the primary or secondary")
     print("Available classes")
     print("-----------------")
     for c in classes:
         print(f'{c["full_name"]} ({c["name"]})')
```

### Comparing `cogsworth-0.0/cogsworth/kicks.py` & `cogsworth-1.0.0/cogsworth/kicks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 import numpy as np
 import gala.integrate as gi
 import gala.dynamics as gd
 import gala.potential as gp
 
 import astropy.coordinates as coords
 import astropy.units as u
-import astropy.constants as const
 
 __all__ = ["get_kick_differential", "integrate_orbit_with_events"]
 
 
-def get_kick_differential(delta_v_sys_xyz, m_1, m_2, a):
-    """Calculate the Differential from a combination of the natal kick, Blauuw kick and orbital motion.
+def get_kick_differential(delta_v_sys_xyz, phase=None, inclination=None):
+    """Calculate the :class:`~astropy.coordinates.CylindricalDifferential` from a combination of the natal
+    kick, Blauuw kick and orbital motion.
 
     Parameters
     ----------
     delta_v_sys_xyz : :class:`~astropy.units.Quantity` [velocity]
         Change in systemic velocity due to natal and Blauuw kicks in BSE :math:`(v_x, v_y, v_z)` frame
         (see Fig A1 of `Hurley+02 <https://ui.adsabs.harvard.edu/abs/2002MNRAS.329..897H/abstract>`_)
-    m_1 : :class:`~astropy.units.Quantity` [mass]
-        Primary mass
-    m_2 : :class:`~astropy.units.Quantity` [mass]
-        Secondary Mass
-    a : :class:`~astropy.units.Quantity` [length]
-        Binary separation
+    phase : `float`
+        Orbital phase angle in radians
+    inclination : `float`
+        Inclination to the Galactic plane in radians
 
     Returns
     -------
     kick_differential : :class:`~astropy.coordinates.CylindricalDifferential`
         Kick differential
     """
-    # TODO: Check whether this should be included but it seems not
-    # calculate the orbital velocity ASSUMING A CIRCULAR ORBIT
-    # if a.value > 0.0:
-    #     v_orb = np.sqrt(const.G * (m_1 + m_2) / a)
-
-    #     # adjust change in velocity by orbital motion of supernova star
-    #     delta_v_sys_xyz -= v_orb
-
     # orbital phase angle and inclination to Galactic plane
-    theta = np.random.uniform(0, 2 * np.pi)
-    phi = np.random.uniform(0, 2 * np.pi)
+    theta = np.random.uniform(0, 2 * np.pi) if phase is None else phase
+    phi = np.random.uniform(0, 2 * np.pi) if inclination is None else inclination
 
     # rotate BSE (v_x, v_y, v_z) into Galactocentric (v_X, v_Y, v_Z)
     v_X = delta_v_sys_xyz[0] * np.cos(theta) - delta_v_sys_xyz[1] * np.sin(theta) * np.cos(phi)\
         + delta_v_sys_xyz[2] * np.sin(theta) * np.sin(phi)
     v_Y = delta_v_sys_xyz[0] * np.sin(theta) + delta_v_sys_xyz[1] * np.cos(theta) * np.cos(phi)\
         - delta_v_sys_xyz[2] * np.cos(theta) * np.sin(phi)
     v_Z = delta_v_sys_xyz[1] * np.sin(phi) + delta_v_sys_xyz[2] * np.cos(phi)
@@ -52,27 +42,28 @@
     kick_differential = coords.CartesianDifferential(v_X, v_Y, v_Z)
 
     return kick_differential
 
 
 def integrate_orbit_with_events(w0, t1, t2, dt, potential=gp.MilkyWayPotential(), events=None,
                                 store_all=True, quiet=False):
-    """Integrate PhaseSpacePosition in a potential with events that occur at certain times
+    """Integrate :class:`~gala.dynamics.PhaseSpacePosition` in a 
+    :class:`Potential <gala.potential.potential.PotentialBase>` with events that occur at certain times
 
     Parameters
     ----------
     w0 : :class:`~gala.dynamics.PhaseSpacePosition`
         Initial phase space position
     t1 : :class:`~astropy.units.Quantity` [time]
         Integration start time
     t2 : :class:`~astropy.units.Quantity` [time]
         Integration end time
     dt : :class:`~astropy.units.Quantity` [time]
         Integration initial timestep size (integrator may adapt timesteps)
-    potential : :class:`~gala.potential.potential.PotentialBase`, optional
+    potential : :class:`Potential <gala.potential.potential.PotentialBase>`, optional
         Potential in which you which to integrate the orbits, by default the
         :class:`~gala.potential.potential.MilkyWayPotential`
     events : `varies`
         Events that occur during the orbit evolution (such as supernova resulting in kicks). If no events
         occur then set `events=None` (this will result in a simple call to `potential.integrate_orbit`). If
         this is a disrupted binary then supply a list of 2 lists of events. Each event list should contain
         the following parameters: `time`, `m_1`, `m_2`, `a`, `ecc`, `delta_v_sys_xyz` (and will be passed to
@@ -93,71 +84,70 @@
     if events is None:
         full_orbit = potential.integrate_orbit(w0, t1=t1, t2=t2, dt=dt, Integrator=gi.DOPRI853Integrator)
         # jettison everything but the final timestep if user says so
         if not store_all:
             full_orbit = full_orbit[-1:]
         return full_orbit
 
-    # if there are two lists (due to a disruption) then recursively call the function
-    elif isinstance(events[0], list):
-        assert len(events) == 2
-        return [integrate_orbit_with_events(w0=w0, potential=potential, events=events[i],
-                                            t1=t1, t2=t2, dt=dt, quiet=quiet, store_all=store_all)
-                for i in range(len(events))]
+    # allow two retries with smaller timesteps
     MAX_DT_RESIZE = 2
     for n in range(MAX_DT_RESIZE):
         try:
             success = False
 
             # work out what the timesteps would be without kicks
             timesteps = gi.parse_time_specification(units=[u.s], t1=t1, t2=t2, dt=dt) * u.s
 
-            # start the cursor at the smallest timestep
+            # start the cursor at the first timestep
             time_cursor = timesteps[0]
             current_w0 = w0
 
             # keep track of the orbit data throughout
             orbit_data = []
 
             # loop over the events
             for event in events:
                 # find the timesteps that occur before the kick
                 timestep_mask = (timesteps >= time_cursor) & (timesteps < (t1 + event["time"]))
 
-                # if any of them occur before the kick then do some integration
+                # integrate up to the moment of the event (if there are any timesteps before it)
                 if any(timestep_mask):
                     matching_timesteps = timesteps[timestep_mask]
 
                     # integrate the orbit over these timesteps
                     orbit = potential.integrate_orbit(current_w0, t=matching_timesteps,
                                                       Integrator=gi.DOPRI853Integrator)
 
-                    # save the orbit data
-                    orbit_data.append(orbit.data)
+                    # save the orbit data (minus the last timestep to avoid duplicates)
+                    orbit_data.append(orbit.data[:-1])
 
-                    # get new PhaseSpacePosition(s)
+                    # set new PhaseSpacePosition from the last timestep
                     current_w0 = orbit[-1]
 
-                # adjust the time
-                time_cursor = t1 + event["time"]
+                    # adjust the time to the last timestep
+                    time_cursor = matching_timesteps[-1]
+                else:           # pragma: no cover
+                    # otherwise skip forward to the event
+                    time_cursor = t1 + event["time"]
 
                 # calculate the kick differential
                 kick_differential = get_kick_differential(delta_v_sys_xyz=event["delta_v_sys_xyz"],
-                                                          m_1=event["m_1"], m_2=event["m_2"], a=event["a"])
+                                                          phase=event["phase"], inclination=event["inc"])
 
                 # update the velocity of the current PhaseSpacePosition
                 current_w0 = gd.PhaseSpacePosition(pos=current_w0.pos,
                                                    vel=current_w0.vel + kick_differential,
                                                    frame=current_w0.frame)
 
             # if we still have time left after the last event (very likely)
             if time_cursor < timesteps[-1]:
                 # evolve the rest of the orbit out
                 matching_timesteps = timesteps[timesteps >= time_cursor]
-                orbit = potential.integrate_orbit(current_w0, t=matching_timesteps, Integrator=gi.DOPRI853Integrator)
+                orbit = potential.integrate_orbit(current_w0, t=matching_timesteps,
+                                                  Integrator=gi.DOPRI853Integrator)
                 orbit_data.append(orbit.data)
 
             data = coords.concatenate_representations(orbit_data) if len(orbit_data) > 1 else orbit_data[0]
 
             full_orbit = gd.orbit.Orbit(pos=data.without_differentials(),
                                         vel=data.differentials["s"],
                                         t=timesteps.to(u.Myr))
```

### Comparing `cogsworth-0.0/cogsworth/observables.py` & `cogsworth-1.0.0/cogsworth/observables.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import numpy as np
 import pandas as pd
 import astropy.units as u
 import astropy.constants as const
-from dustmaps.bayestar import BayestarQuery
+from astropy.coordinates import SkyCoord
+from copy import copy
 
-# HACK around the isochrone import to ignore warnings about Holoview and Multinest
 import logging
-logging.getLogger("isochrones").setLevel("ERROR")
-from isochrones.mist.bc import MISTBolometricCorrectionGrid
-logging.getLogger("isochrones").setLevel("WARNING")
+from cogsworth.tests.optional_deps import check_dependencies
+
+import sys
+import os
 
 __all__ = ["get_log_g", "get_absolute_bol_mag", "get_apparent_mag", "get_absolute_mag", "add_mags",
            "get_extinction", "get_photometry"]
 
 
 def get_log_g(mass, radius):
     """Computes log of the surface gravity in cgs
@@ -174,14 +175,16 @@
         The coordinates at which you wish to calculate extinction values
 
     Returns
     -------
     Av : :class:`~numpy.ndarray`
         Visual extinction values for each set of coordinates
     """
+    assert check_dependencies("dustmaps")
+    from dustmaps.bayestar import BayestarQuery
 
     # following section performs reflections for coordinates below -30 deg declination
     # convert to galactic coordinates
     galactic = coords.galactic
 
     # try all possible reflections about the galactic plane
     for ref_l, ref_b in [(-1, 1), (1, -1), (-1, -1)]:
@@ -206,78 +209,120 @@
         # set the data back in the main coord object
         galactic.data.lon[too_low] = reflected.data.lon
         galactic.data.lat[too_low] = reflected.data.lat
 
         # clear the cache to ensure consistency
         galactic.cache.clear()
 
+    # briefly disable print statements to hide the messy output from dustmaps
+    sys.stdout = open(os.devnull, 'w')
+
     bayestar = BayestarQuery(max_samples=2, version='bayestar2019')
 
     # calculate the reddening due to dust
     ebv = bayestar(galactic, mode='random_sample')
 
+    # bring print statements back
+    sys.stdout = sys.__stdout__
+
     # convert this to a visual extinction
     Av = 3.3 * ebv
     return Av
 
 
-def get_photometry(final_bpp, final_coords, filters, ignore_extinction=False):
+def get_photometry(filters, population=None, final_bpp=None, final_pos=None, distances=None,
+                   ignore_extinction=False, assume_mw_galactocentric=False):
     """Computes photometry subject to dust extinction using the MIST boloemtric correction grid
 
     Parameters
     ----------
+    filters : `list` of `str`
+        Which filters to compute photometry for (e.g. ['J', 'H', 'K', 'G', 'BP', 'RP'])
+    population : :class:`~cogsworth.pop.Population`
+        The population for which to compute photometry (either supply this or a final_bpp and final_pos)
     final_bpp : :class:`~pandas.DataFrame`
         A dataset of COSMIC binaries at present day - must include these columns: ["sep", "metallicity"] and
         for each star it must have the columns ["teff", "lum", "mass", "rad", "kstar"]
-    final_coords : `tuple` of :class:`~astropy.coordinates.SkyCoord`
-        Final positions and velocities of the binaries at present day. First entry is for binaries or the
-        primary in a disrupted system, second entry is for secondaries in a disrupted system.
-    filters : `list` of `str`
-        Which filters to compute photometry for (e.g. ['J', 'H', 'K', 'G', 'BP', 'RP'])
+    final_pos : :class:`~astropy.quantity.Quantity`
+        Final positions of each system in the galactocentric frame.
+        The first `len(self)` entries of each are for bound binaries or primaries, then the final
+        `self.disrupted.sum()` entries are for disrupted secondaries. Any missing orbits (where orbit=None
+        will be set to `np.inf` for ease of masking.
     ignore_extinction : `bool`
         Whether to ignore extinction
 
     Returns
     -------
     photometry : :class:`~pandas.DataFrame`
         Photometry and extinction information for supplied COSMIC binaries in desired `filters`
     """
+    assert check_dependencies(["isochrones", "nose", "tables"])
+    # HACK around the isochrone import to ignore warnings about Holoview and Multinest
+    logging.getLogger("isochrones").setLevel("ERROR")
+    from isochrones.mist.bc import MISTBolometricCorrectionGrid
+    logging.getLogger("isochrones").setLevel("WARNING")
+
+    # check that the input is valid
+    if population is None and (final_bpp is None or final_pos is None):
+        raise ValueError("Either a population or final_bpp and final_pos must be supplied")
+    if distances is None and not assume_mw_galactocentric:
+        raise ValueError("Must supply either distances or have `assume_mw_galactocentric=True`")
+    if not ignore_extinction and not assume_mw_galactocentric:
+        raise ValueError("Cannot calculate extinction due to dust without `assume_mw_galactocentric=True`")
+
+    if population is not None:
+        final_bpp = population.final_bpp
+        final_pos = population.final_pos
+        disrupted = population.disrupted
+    else:
+        disrupted = final_bpp["sep"].values < 0.0
+
+    if assume_mw_galactocentric:
+        final_coords = SkyCoord(x=final_pos[:, 0], y=final_pos[:, 1], z=final_pos[:, 2],
+                                frame="galactocentric", unit=u.kpc, representation_type="cartesian")
+
     # set up empty photometry table
     photometry = pd.DataFrame()
-    disrupted = final_bpp["sep"].values < 0.0
 
     if not ignore_extinction:       # pragma: no cover
         # get extinction for bound binaries and primary of disrupted binaries
-        photometry['Av_1'] = get_extinction(final_coords[0])
+        photometry['Av_1'] = get_extinction(final_coords[:len(final_bpp)])
 
         # get extinction for secondaries of disrupted binaries (leave as np.inf otherwise)
-        photometry['Av_2'] = np.repeat(np.inf, len(final_coords[1]))
-        photometry.loc[disrupted, "Av_2"] = get_extinction(final_coords[1][disrupted])
+        photometry['Av_2'] = np.repeat(np.inf, len(final_bpp))
+        photometry.loc[disrupted, "Av_2"] = get_extinction(final_coords[len(final_bpp):])
 
         # ensure extinction remains in MIST grid range (<= 6) and is not NaN
         photometry.loc[photometry.Av_1 > 6, ['Av_1']] = 6
         photometry.loc[photometry.Av_2 > 6, ['Av_2']] = 6
         photometry = photometry.fillna(6)
     else:
-        photometry['Av_1'] = np.zeros(len(final_coords[0]))
-        photometry['Av_2'] = np.zeros(len(final_coords[0]))
+        photometry['Av_1'] = np.zeros(len(final_bpp))
+        photometry['Av_2'] = np.zeros(len(final_bpp))
 
     # get Fe/H using e.g. Bertelli+1994 Eq. 10 (assuming all stars have the solar abundance pattern)
     Z_sun = 0.0142
     FeH = np.log10(final_bpp["metallicity"].values / Z_sun)
 
     # set up MIST bolometric correction grid
     bc_grid = MISTBolometricCorrectionGrid(bands=filters)
     bc = {
         "app": [None, None],
         "abs": [None, None]
     }
 
+    if distances is None:
+        distances = final_coords.icrs.distance
+    primary_distances = distances[:len(final_bpp)]
+    # secondary distances are the same whilst bound but different when disrupted
+    secondary_distances = copy(primary_distances)
+    secondary_distances[disrupted] = distances[len(final_bpp):]
+
     # for each star in the (possibly disrupted/merged) binary
-    for ind in [1, 2]:
+    for ind, dist in zip([1, 2], [primary_distances, secondary_distances]):
         # calculate the surface gravity if necessary
         if f"log_g_{ind}" not in final_bpp:
             final_bpp.insert(len(final_bpp.columns), f"log_g_{ind}",
                              get_log_g(mass=final_bpp[f"mass_{ind}"].values * u.Msun,
                                        radius=final_bpp[f"rad_{ind}"].values * u.Rsun))
 
         # get the bolometric corrections from MIST isochrones
@@ -288,22 +333,17 @@
                                              final_bpp[f"log_g_{ind}"].values,
                                              FeH, np.zeros(len(final_bpp))], filters)
 
         # calculate the absolute bolometric magnitude and set any BH or massless remnants to invisible
         photometry[f"M_abs_{ind}"] = get_absolute_bol_mag(lum=final_bpp[f"lum_{ind}"].values * u.Lsun)
         photometry.loc[np.isin(final_bpp[f"kstar_{ind}"].values, [13, 14, 15]), f"M_abs_{ind}"] = np.inf
 
-        # work out the distance (if the system is bound always use the first `final_coords` SkyCoord)
-        distance = np.repeat(np.inf, len(final_bpp)) * u.kpc
-        distance[disrupted] = final_coords[ind - 1][disrupted].icrs.distance
-        distance[~disrupted] = final_coords[0][~disrupted].icrs.distance
-
         # convert the absolute magnitude to an apparent magnitude
         photometry[f"m_app_{ind}"] = get_apparent_mag(M_abs=photometry[f"M_abs_{ind}"].values,
-                                                      distance=distance)
+                                                      distance=dist)
 
     # go through each filter
     for i, filter in enumerate(filters):
         for prefix, mag_type in [("m", "app"), ("M", "abs")]:
             # apply the bolometric corrections to the apparent magnitude of each star
             filter_mags = [photometry[f"{prefix}_{mag_type}_{ind}"].values - bc[mag_type][ind - 1][:, i]
                            for ind in [1, 2]]
```

### Comparing `cogsworth-0.0/cogsworth/pop.py` & `cogsworth-1.0.0/cogsworth/pop.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 import warnings
 import numpy as np
 import astropy.units as u
 import astropy.coordinates as coords
 import h5py as h5
 import pandas as pd
 from tqdm import tqdm
-import healpy as hp
-import matplotlib.pyplot as plt
-
-from gaiaunlimited.selectionfunctions import DR3SelectionFunctionTCG
-from gaiaunlimited.utils import get_healpix_centers
+import yaml
+import logging
 
 from cosmic.sample.initialbinarytable import InitialBinaryTable
-from cosmic.sample.sampler.independent import Sample
 from cosmic.evolve import Evolve
+from cosmic.checkstate import set_checkstates
+from cosmic.utils import parse_inifile
 import gala.potential as gp
 import gala.dynamics as gd
+from gala.potential.potential.io import to_dict as potential_to_dict, from_dict as potential_from_dict
 
-from cogsworth import galaxy
+from cogsworth import sfh
 from cogsworth.kicks import integrate_orbit_with_events
 from cogsworth.events import identify_events
 from cogsworth.classify import determine_final_classes
 from cogsworth.observables import get_photometry
+from cogsworth.tests.optional_deps import check_dependencies
+from cogsworth.plot import plot_cartoon_evolution
+from cogsworth.utils import translate_COSMIC_tables
+
+from cogsworth.citations import CITATIONS
 
 __all__ = ["Population", "load"]
 
 
 class Population():
     """Class for creating and evolving populations of binaries throughout the Milky Way
 
@@ -41,32 +45,43 @@
         How many processes to run if you want multithreading, by default 8
     m1_cutoff : `float`, optional
         The minimum allowed primary mass, by default 0
     final_kstar1 : `list`, optional
         Desired final types for primary star, by default list(range(16))
     final_kstar2 : `list`, optional
         Desired final types for secondary star, by default list(range(16))
-    galaxy_model : :class:`~cogsworth.galaxy.Galaxy`, optional
-        A Galaxy class to use for sampling the initial galaxy parameters, by default
-        :class:`~cogsworth.galaxy.Frankel2018`
-    galactic_potential : :class:`~gala.potential.potential.PotentialBase`, optional
+    sfh_model : :class:`~cogsworth.sfh.StarFormationHistory`, optional
+        A StarFormationHistory class to use for sampling the initial galaxy parameters, by default
+        :class:`~cogsworth.sfh.Wagg2022`
+    sfh_params : `dict`, optional
+        Any additional parameters to pass to your chosen ``SFH model`` when it is initialised
+    galactic_potential : :class:`Potential <gala.potential.potential.PotentialBase>`, optional
         Galactic potential to use for evolving the orbits of binaries, by default
         :class:`~gala.potential.potential.MilkyWayPotential`
     v_dispersion : :class:`~astropy.units.Quantity` [velocity], optional
         Velocity dispersion to apply relative to the local circular velocity, by default 5*u.km/u.s
     max_ev_time : :class:`~astropy.units.Quantity` [time], optional
         Maximum evolution time for both COSMIC and Gala, by default 12.0*u.Gyr
     timestep_size : :class:`~astropy.units.Quantity` [time], optional
         Size of timesteps to use in galactic evolution, by default 1*u.Myr
     BSE_settings : `dict`, optional
-        Any BSE settings to pass to COSMIC
+        Any BSE settings to pass to COSMIC, superseded by `ini_file` if provided
+    ini_file : `str`, optional
+        Path to an ini file to use for the COSMIC stellar evolution, supersedes `BSE_settings` by default None
+    bcm_timestep_conditions : List of lists, optional
+        Any timestep conditions to pass to COSMIC evolution. This will affect the rows that are output in the
+        the BCM table, by default only the first and last timesteps are output. For more details check out the
+        `relevant COSMIC docs <https://cosmic-popsynth.github.io/COSMIC/examples/index.html#dynamically-set-time-resolution-for-bcm-array>`_
+    sampling_params : `dict`, optional
+        Any additional parameters to pass to the COSMIC sampling (see
+        :meth:`~cosmic.sample.sampler.independent.get_independent_sampler`)
     store_entire_orbits : `bool`, optional
         Whether to store the entire orbit for each binary, by default True. If not then only the final
         PhaseSpacePosition will be stored. This cuts down on both memory usage and disk space used if you
-        save the Population.
+        save the Population (as well as how long it takes to reload the data).
 
     Attributes
     ----------
     mass_singles : `float`
         Total mass in single stars needed to generate population
     mass_binaries : `float`
         Total mass in binaries needed to generate population
@@ -79,75 +94,85 @@
     bcm : :class:`~pandas.DataFrame`
         Final state of each binary
     initC : :class:`~pandas.DataFrame`
         Initial conditions for each binary
     kick_info : :class:`~pandas.DataFrame`
         Information about the kicks that occur for each binary
     orbits : `list` of :class:`~gala.dynamics.Orbit`
-        The orbits of each binary within the galaxy from its birth until :attr:`max_ev_time` with timesteps of
-        :attr:`timestep_size`. Note that disrupted binaries will have two entries (for both stars).
+        The orbits of each system within the galaxy from its birth until :attr:`max_ev_time` with timesteps of
+        :attr:`timestep_size`. This list will have length = `len(self) + self.disrupted.sum()`, where the
+        first section are for bound binaries and disrupted primaries and the last section are for disrupted
+        secondaries
     classes : `list`
         The classes associated with each produced binary (see :meth:`~cogsworth.classify.list_classes` for a
         list of available classes and their meanings)
-    final_coords : `tuple` of :class:`~astropy.coordinates.SkyCoord`
-        A SkyCoord object of the final positions of each binary in the galactocentric frame.
-        For bound binaries only the first SkyCoord is populated, for disrupted binaries each SkyCoord
-        corresponds to the individual components. Any missing orbits (where orbit=None or there is no
-        secondary component) will be set to `np.inf` for ease of masking.
+    final_pos, final_vel : :class:`~astropy.quantity.Quantity`
+        Final positions and velocities of each system in the galactocentric frame.
+        The first `len(self)` entries of each are for bound binaries or primaries, then the final
+        `self.disrupted.sum()` entries are for disrupted secondaries. Any missing orbits (where orbit=None
+        will be set to `np.inf` for ease of masking.
     final_bpp : :class:`~pandas.DataFrame`
         The final state of each binary (taken from the final entry in :attr:`bpp`)
     disrupted : :class:`~numpy.ndarray` of `bool`
         A mask on the binaries of whether they were disrupted
     observables : :class:`~pandas.DataFrame`
-        Observables associated with the final binaries. See `get_observables` for more details on the columns
-    bin_nums : :class:`~np.ndarray`
+        Observables associated with the final binaries. See `get_photometry` for more details on the columns
+    bin_nums : :class:`~numpy.ndarray`
         An array containing the unique COSMIC `bin_nums` of each binary in the population - these can be
         used an indices for the population
     """
     def __init__(self, n_binaries, processes=8, m1_cutoff=0, final_kstar1=list(range(16)),
-                 final_kstar2=list(range(16)), galaxy_model=galaxy.Frankel2018,
+                 final_kstar2=list(range(16)), sfh_model=sfh.Wagg2022, sfh_params={},
                  galactic_potential=gp.MilkyWayPotential(), v_dispersion=5 * u.km / u.s,
-                 max_ev_time=12.0*u.Gyr, timestep_size=1 * u.Myr, BSE_settings={}, store_entire_orbits=True):
+                 max_ev_time=12.0*u.Gyr, timestep_size=1 * u.Myr, BSE_settings={}, ini_file=None,
+                 sampling_params={}, bcm_timestep_conditions=[], store_entire_orbits=True):
 
-        # require a sensible number of binaries
-        if n_binaries <= 0:
-            raise ValueError("You need to input a *nonnegative* number of binaries")
+        # require a sensible number of binaries if you are not targetting total mass
+        if not ("sampling_target" in sampling_params and sampling_params["sampling_target"] == "total_mass"):
+            if n_binaries <= 0:
+                raise ValueError("You need to input a *nonnegative* number of binaries")
 
         self.n_binaries = n_binaries
         self.n_binaries_match = n_binaries
         self.processes = processes
         self.m1_cutoff = m1_cutoff
         self.final_kstar1 = final_kstar1
         self.final_kstar2 = final_kstar2
-        self.galaxy_model = galaxy_model
+        self.sfh_model = sfh_model
+        self.sfh_params = sfh_params
         self.galactic_potential = galactic_potential
         self.v_dispersion = v_dispersion
         self.max_ev_time = max_ev_time
         self.timestep_size = timestep_size
         self.pool = None
         self.store_entire_orbits = store_entire_orbits
 
+        self._file = None
         self._initial_binaries = None
+        self._initial_galaxy = None
         self._mass_singles = None
         self._mass_binaries = None
         self._n_singles_req = None
         self._n_bin_req = None
         self._bpp = None
         self._bcm = None
         self._initC = None
         self._kick_info = None
         self._orbits = None
         self._classes = None
-        self._final_coords = None
+        self._final_pos = None
+        self._final_vel = None
         self._final_bpp = None
         self._disrupted = None
         self._escaped = None
         self._observables = None
         self._bin_nums = None
 
+        self.__citations__ = ["cogsworth", "cosmic", "gala"]
+
         self.BSE_settings = {'xi': 1.0, 'bhflag': 1, 'neta': 0.5, 'windflag': 3, 'wdflag': 1, 'alpha1': 1.0,
                              'pts1': 0.001, 'pts3': 0.02, 'pts2': 0.01, 'epsnov': 0.001, 'hewind': 0.5,
                              'ck': 1000, 'bwind': 0.0, 'lambdaf': 0.0, 'mxns': 3.0, 'beta': -1.0, 'tflag': 1,
                              'acc2': 1.5, 'grflag': 1, 'remnantflag': 4, 'ceflag': 0, 'eddfac': 1.0,
                              'ifflag': 0, 'bconst': 3000, 'sigma': 265.0, 'gamma': -2.0, 'pisn': 45.0,
                              'natal_kick_array': [[-100.0, -100.0, -100.0, -100.0, 0.0],
                                                   [-100.0, -100.0, -100.0, -100.0, 0.0]], 'bhsigmafrac': 1.0,
@@ -157,113 +182,202 @@
                              'ecsn_mlow': 1.6, 'aic': 1, 'ussn': 0, 'sigmadiv': -20.0, 'qcflag': 5,
                              'eddlimflag': 0, 'fprimc_array': [2.0/21.0, 2.0/21.0, 2.0/21.0, 2.0/21.0,
                                                                2.0/21.0, 2.0/21.0, 2.0/21.0, 2.0/21.0,
                                                                2.0/21.0, 2.0/21.0, 2.0/21.0, 2.0/21.0,
                                                                2.0/21.0, 2.0/21.0, 2.0/21.0, 2.0/21.0],
                              'bhspinflag': 0, 'bhspinmag': 0.0, 'rejuv_fac': 1.0, 'rejuvflag': 0, 'htpmb': 1,
                              'ST_cr': 1, 'ST_tide': 1, 'bdecayfac': 1, 'rembar_massloss': 0.5, 'kickflag': 0,
-                             'zsun': 0.014, 'bhms_coll_flag': 0, 'don_lim': -1, 'acc_lim': -1, 'binfrac': 0.5}
-        self.BSE_settings.update(BSE_settings)
+                             'zsun': 0.014, 'bhms_coll_flag': 0, 'don_lim': -1, 'acc_lim': -1, 'binfrac': 0.5,
+                             'rtmsflag': 0, 'wd_mass_lim': 1}
+        self.BSE_settings.update(BSE_settings if ini_file is None else parse_inifile(ini_file)[0])
+
+        self.sampling_params = {'primary_model': 'kroupa01', 'ecc_model': 'sana12', 'porb_model': 'sana12',
+                                'qmin': -1, 'keep_singles': False}
+        self.sampling_params.update(sampling_params)
+        self.bcm_timestep_conditions = bcm_timestep_conditions
 
     def __repr__(self):
         if self._orbits is None:
             return (f"<{self.__class__.__name__} - {self.n_binaries} systems - "
                     f"galactic_potential={self.galactic_potential.__class__.__name__}, "
-                    f"SFH={self.galaxy_model.__name__}>")
+                    f"SFH={self.sfh_model.__name__}>")
         else:
             return (f"<{self.__class__.__name__} - {self.n_binaries_match} evolved systems - "
                     f"galactic_potential={self.galactic_potential.__class__.__name__}, "
-                    f"galaxy_model={self.galaxy_model.__name__}>")
+                    f"sfh_model={self.sfh_model.__name__}>")
 
     def __len__(self):
         return self.n_binaries_match
 
     def __getitem__(self, ind):
+        # convert any Pandas Series to numpy arrays
+        ind = ind.values if isinstance(ind, pd.Series) else ind
+
         # ensure indexing with the right type
-        if not isinstance(ind, (int, slice, list, np.ndarray, tuple)):
-            raise ValueError(("Can only index using an `int`, `list`, `ndarray` or `slice`, you supplied a "
-                              f"`{type(ind).__name__}`"))
+        ALLOWED_TYPES = (int, slice, list, np.ndarray, tuple)
+        if not isinstance(ind, ALLOWED_TYPES):
+            raise ValueError((f"Can only index using one of {[at.__name__ for at in ALLOWED_TYPES]}, "
+                              f"you supplied a '{type(ind).__name__}'"))
+
+        # check validity of indices for array-like types
+        if isinstance(ind, (list, tuple, np.ndarray)):
+            # check every element is a boolean (if so, convert to bin_nums after asserting length sensible)
+            if all(isinstance(x, (bool, np.bool_)) for x in ind):
+                assert len(ind) == len(self.bin_nums), "Boolean mask must be same length as the population"
+                ind = self.bin_nums[ind]
+            # otherwise ensure all elements are integers
+            else:
+                assert all(isinstance(x, (int, np.integer)) for x in ind), \
+                    "Can only index using integers or a boolean mask"
+                if len(np.unique(ind)) < len(ind):
+                    warnings.warn(("You have supplied duplicate indices, this will invalidate the "
+                                   "normalisation of the Population (e.g. mass_binaries will be wrong)"))
 
-        # create a list of bin nums from ind
+        # set up the bin_nums we are selecting
         bin_nums = ind
+
+        # turn ints into arrays and convert slices to exact bin_nums
         if isinstance(ind, int):
             bin_nums = [ind]
-        if isinstance(ind, slice):
-            bin_nums = list(range(ind.stop)[ind])
+        elif isinstance(ind, slice):
+            bin_nums = self.bin_nums[ind]
         bin_nums = np.asarray(bin_nums)
 
         # check that the bin_nums are all valid
-        possible_bin_nums = self.final_bpp["bin_num"]
-        check_nums = np.isin(bin_nums, possible_bin_nums)
+        check_nums = np.isin(bin_nums, self.bin_nums)
         if not check_nums.all():
             raise ValueError(("The index that you supplied includes a `bin_num` that does not exist. "
                               f"The first bin_num I couldn't find was {bin_nums[~check_nums][0]}"))
 
         # start a new population with the same parameters
         new_pop = self.__class__(n_binaries=len(bin_nums), processes=self.processes,
                                  m1_cutoff=self.m1_cutoff, final_kstar1=self.final_kstar1,
-                                 final_kstar2=self.final_kstar2, galaxy_model=self.galaxy_model,
-                                 galactic_potential=self.galactic_potential, v_dispersion=self.v_dispersion,
-                                 max_ev_time=self.max_ev_time, timestep_size=self.timestep_size,
-                                 BSE_settings=self.BSE_settings, store_entire_orbits=self.store_entire_orbits)
+                                 final_kstar2=self.final_kstar2, sfh_model=self.sfh_model,
+                                 sfh_params=self.sfh_params, galactic_potential=self.galactic_potential,
+                                 v_dispersion=self.v_dispersion, max_ev_time=self.max_ev_time,
+                                 timestep_size=self.timestep_size, BSE_settings=self.BSE_settings,
+                                 sampling_params=self.sampling_params,
+                                 store_entire_orbits=self.store_entire_orbits)
 
         # proxy for checking whether sampling has been done
         if self._mass_binaries is not None:
             new_pop._mass_binaries = self._mass_binaries
             new_pop._mass_singles = self._mass_singles
             new_pop._n_singles_req = self._n_singles_req
             new_pop._n_bin_req = self._n_bin_req
 
+        bin_num_to_ind = {num: i for i, num in enumerate(self.bin_nums)}
+        sort_idx = np.argsort(list(bin_num_to_ind.keys()))
+        idx = np.searchsorted(list(bin_num_to_ind.keys()), bin_nums, sorter=sort_idx)
+        inds = np.asarray(list(bin_num_to_ind.values()))[sort_idx][idx]
+
+        disrupted_bin_num_to_ind = {num: i for i, num in enumerate(self.bin_nums[self.disrupted])}
+        sort_idx = np.argsort(list(disrupted_bin_num_to_ind.keys()))
+        idx = np.searchsorted(list(disrupted_bin_num_to_ind.keys()),
+                              bin_nums[np.isin(bin_nums, self.bin_nums[self.disrupted])],
+                              sorter=sort_idx)
+        inds_with_disruptions = np.asarray(list(disrupted_bin_num_to_ind.values()))[sort_idx][idx] + len(self)
+        all_inds = np.concatenate((inds, inds_with_disruptions)).astype(int)
+
         if self._initial_galaxy is not None:
-            # since we are indexing on bin nums, need to convert that to actual indices
-            ind_range = np.arange(len(possible_bin_nums))
-            new_pop._initial_galaxy = self._initial_galaxy[ind_range[possible_bin_nums.isin(bin_nums)]]
+            new_pop._initial_galaxy = self._initial_galaxy[inds]
 
         # checking whether stellar evolution has been done
         if self._bpp is not None:
-            # copy over subsets of the stellar evolution tables when they aren't None
-            new_pop._bpp = self._bpp[self._bpp["bin_num"].isin(bin_nums)]
+            # copy over subsets of data when they aren't None
+            new_pop._bpp = self._bpp.loc[bin_nums]
             if self._bcm is not None:
-                new_pop._bcm = self._bcm[self._bcm["bin_num"].isin(bin_nums)]
+                new_pop._bcm = self._bcm.loc[bin_nums]
             if self._initC is not None:
-                new_pop._initC = self._initC[self._initC["bin_num"].isin(bin_nums)]
+                new_pop._initC = self._initC.loc[bin_nums]
             if self._kick_info is not None:
-                new_pop._kick_info = self._kick_info[self._kick_info["bin_num"].isin(bin_nums)]
-
-            # same sort of thing for later parameters
-            mask = self.final_bpp["bin_num"].isin(bin_nums).values
-            new_pop._final_bpp = self.final_bpp[mask]
-
-            if self._orbits is not None:
-                new_pop._orbits = self.orbits[mask]
+                new_pop._kick_info = self._kick_info.loc[bin_nums]
+            if self._final_bpp is not None:
+                new_pop._final_bpp = self._final_bpp.loc[bin_nums]
             if self._disrupted is not None:
-                new_pop._disrupted = self._disrupted[mask]
+                new_pop._disrupted = self._disrupted[inds]
             if self._classes is not None:
-                new_pop._classes = self._classes[mask]
-            if self._final_coords is not None:
-                new_pop._final_coords = [self._final_coords[i][mask] for i in range(2)]
-            if self._disrupted is not None:
-                new_pop._disrupted = self._disrupted[mask]
+                new_pop._classes = self._classes.iloc[inds]
             if self._observables is not None:
-                new_pop._observables = self._observables[mask]
+                new_pop._observables = self._observables.iloc[inds]
 
+            # same thing but for arrays with appended disrupted secondaries
+            if self._orbits is not None:
+                new_pop._orbits = self.orbits[all_inds]
+            if self._final_pos is not None:
+                new_pop._final_pos = self._final_pos[all_inds]
+            if self._final_vel is not None:
+                new_pop._final_vel = self._final_vel[all_inds]
         return new_pop
 
+    def get_citations(self, filename=None):
+        """Print the citations for the packages/papers used in the population"""
+        # ask users for a filename to save the bibtex to
+        if filename is None:
+            filename = input("Filename for generating a bibtex file (leave blank to just print to terminal): ")
+        filename = filename + ".bib" if not filename.endswith(".bib") and filename != "" else filename
+
+        sections = {
+            "general": "",
+            "sfh": r"The \texttt{cogsworth} population used a star formation history model based on the following papers",
+            "observables": "Population observables were estimated using dust maps and MIST isochrones",
+            "gaia": "Observability of systems with Gaia was predicted using an empirical selection function",
+            "legwork": "Calculation of LISA gravitational wave signatures was performed using LEGWORK",
+            "FIRE": "The initial conditions for the population were sampled from the FIRE simulations",
+        }
+
+        acknowledgement = r"This research made use of \texttt{cogsworth} and its dependencies"
+
+        # construct citation string
+        bibtex = []
+        for section in sections:
+            cite_tags = []
+            for citation in self.__citations__:
+                if citation in CITATIONS[section]:
+                    cite_tags.extend(CITATIONS[section][citation]["tags"])
+                    bibtex.append(CITATIONS[section][citation]["bibtex"])
+            if len(cite_tags) > 0:
+                cite_str = ",".join(cite_tags)
+                acknowledgement += sections[section] + r" \citep{" + cite_str + "}. "
+        bibtex_str = "\n\n".join(bibtex)
+
+        # print the acknowledgement
+        BOLD, RESET, GREEN = "\033[1m", "\033[0m", "\033[0;32m"
+        print("\nYou can paste this acknowledgement into the relevant section of your manuscript:")
+        print(f"{BOLD}{GREEN}{acknowledgement}{RESET}")
+
+        # either print bibtex to terminal or save to file
+        if filename != "":
+            print(f"The associated bibtex can be found in {filename}")
+            with open(filename, "w") as f:
+                f.write(bibtex_str)
+        else:
+            print("\nAnd paste this bibtex into your .bib file:")
+            print(f"{BOLD}{GREEN}{bibtex_str}{RESET}")
+        print("Good luck with the paper writing ◝(ᵔᵕᵔ)◜")
+
     @property
     def bin_nums(self):
         if self._bin_nums is None:
-            if self._bpp is not None:
-                self._bin_nums = self.final_bpp["bin_num"].unique()
+            if self._final_bpp is not None:
+                self._bin_nums = self._final_bpp["bin_num"].unique()
+            elif self._initC is not None:
+                self._bin_nums = self._initC["bin_num"].unique()
+            elif self._initial_binaries is not None:
+                self._bin_nums = np.unique(self._initial_binaries.index.values)
             else:
-                raise ValueError("You need to evolve binaries to get a list of `bin_nums`!")
+                raise ValueError("You need to first sample binaries to get a list of `bin_nums`!")
         return self._bin_nums
 
     @property
     def initial_galaxy(self):
-        if self._initial_galaxy is None:
+        if self._initial_galaxy is None and self._file is not None:
+            self._initial_galaxy = sfh.load(self._file, key="initial_galaxy")
+            self.sfh_model = self._initial_galaxy.__class__
+        elif self._initial_galaxy is None:
             self.sample_initial_binaries()
         return self._initial_galaxy
 
     @property
     def mass_singles(self):
         if self._mass_singles is None:
             self.sample_initial_binaries()
@@ -285,53 +399,106 @@
     def n_bin_req(self):
         if self._n_bin_req is None:
             self.sample_initial_binaries()
         return self._n_bin_req
 
     @property
     def bpp(self):
-        if self._bpp is None:
+        if self._bpp is None and self._file is not None:
+            self._bpp = pd.read_hdf(self._file, key="bpp")
+        elif self._bpp is None:
             self.perform_stellar_evolution()
         return self._bpp
 
     @property
     def bcm(self):
-        if self._bcm is None:
-            self.perform_stellar_evolution()
+        if self._bcm is None and self._file is not None:
+            has_bcm = None
+            with h5.File(self._file, "r") as f:
+                has_bcm = "bcm" in f
+            self._bcm = pd.read_hdf(self._file, key="bcm") if has_bcm else None
+        elif self._bcm is None:
+            if len(np.ravel(self.bcm_timestep_conditions)) == 0:        # pragma: no cover
+                logging.getLogger("cogsworth").warning(("cogsworth warning: You haven't set any timestep "
+                                                        "conditions for the BCM table, so it is not "
+                                                        "calculated. Set `bcm_timestep_conditions` to get a "
+                                                        "BCM table."))
+            else:
+                self.perform_stellar_evolution()
         return self._bcm
 
     @property
     def initC(self):
-        if self._initC is None:
+        if self._initC is None and self._file is not None:
+            self._initC = pd.read_hdf(self._file, key="initC")
+        elif self._initC is None:
             self.perform_stellar_evolution()
         return self._initC
 
     @property
     def kick_info(self):
+        if self._kick_info is None and self._file is not None:
+            self._kick_info = pd.read_hdf(self._file, key="kick_info")
         if self._kick_info is None:
             self.perform_stellar_evolution()
         return self._kick_info
 
     @property
     def orbits(self):
-        if self._orbits is None:
+        # if orbits are uncalculated and no file is provided then perform galactic orbit evolution
+        if self._orbits is None and self._file is None:
             self.perform_galactic_evolution()
+        # otherwise if orbits are uncalculated but a file is provided then load the orbits from the file
+        elif self._orbits is None:
+            # load the entire file into memory
+            with h5.File(self._file, "r") as f:
+                if "orbits" not in f:
+                    raise ValueError(f"No orbits found in population file ({self._file})")
+
+                offsets = f["orbits"]["offsets"][...]
+                pos, vel = f["orbits"]["pos"][...] * u.kpc, f["orbits"]["vel"][...] * u.km / u.s
+                t = f["orbits"]["t"][...] * u.Myr
+
+            # convert positions, velocities and times into a list of orbits
+            self._orbits = np.array([gd.Orbit(pos[:, offsets[i]:offsets[i + 1]],
+                                              vel[:, offsets[i]:offsets[i + 1]],
+                                              t[offsets[i]:offsets[i + 1]]) for i in range(len(offsets) - 1)])
+
+            # also calculate the final positions and velocities while you're at it
+            final_inds = offsets[1:] - 1
+            self._final_pos = pos[:, final_inds].T
+            self._final_vel = vel[:, final_inds].T
         return self._orbits
 
     @property
+    def primary_orbits(self):
+        return self.orbits[:len(self)]
+
+    @property
+    def secondary_orbits(self):
+        order = np.argsort(np.concatenate((self.bin_nums[~self.disrupted], self.bin_nums[self.disrupted])))
+        return np.concatenate((self.primary_orbits[~self.disrupted], self.orbits[len(self):]))[order] 
+
+    @property
     def classes(self):
         if self._classes is None:
             self._classes = determine_final_classes(population=self)
         return self._classes
 
     @property
-    def final_coords(self):
-        if self._final_coords is None:
-            self._final_coords = self.get_final_coords()
-        return self._final_coords
+    def final_pos(self):
+        if self._final_pos is None:
+            self._final_pos, self._final_vel = self._get_final_coords()
+        return self._final_pos
+
+    @property
+    def final_vel(self):
+        if self._final_vel is None:
+            self._final_pos, self._final_vel = self._get_final_coords()
+        return self._final_vel
 
     @property
     def final_bpp(self):
         if self._final_bpp is None:
             self._final_bpp = self.bpp.drop_duplicates(subset="bin_num", keep="last")
             self._final_bpp.insert(len(self._final_bpp.columns), "metallicity",
                                    self.initC["metallicity"].values)
@@ -345,36 +512,30 @@
                                & (self.final_bpp["sep"] < 0.0)
                                & self.final_bpp["bin_num"].isin(self.bpp[self.bpp["evol_type"] == 11.0]["bin_num"])).values
         return self._disrupted
 
     @property
     def escaped(self):
         if self._escaped is None:
-            self._escaped = [np.repeat(False, len(self)), np.repeat(False, len(self))]
+            self._escaped = np.repeat(False, len(self))
+
+            # get the current velocity
+            v_curr = np.sum(self.final_vel**2, axis=1)**(0.5)
 
-            # do it for all systems and then also for the secondaries of disrupted systems
-            for ind, mask in enumerate([np.repeat(True, len(self)), self.disrupted]):
-                # get the current velocity
-                v_curr = np.sum(self.final_coords[ind][mask].velocity.d_xyz**2, axis=0)**(0.5)
-
-                # get the escape velocity at the current position based on galactic potential
-                pos = np.asarray([self.final_coords[ind][mask].galactocentric.x.to(u.kpc),
-                                  self.final_coords[ind][mask].galactocentric.y.to(u.kpc),
-                                  self.final_coords[ind][mask].galactocentric.z.to(u.kpc)]) * u.kpc
-
-                # 0.5 * m * v_esc**2 = m * (-Phi)
-                v_esc = np.sqrt(-2 * self.galactic_potential(pos))
-                self._escaped[ind][mask] = v_curr >= v_esc
+            # 0.5 * m * v_esc**2 = m * (-Phi)
+            v_esc = np.sqrt(-2 * self.galactic_potential(self.final_pos.T))
+            self._escaped = v_curr >= v_esc
         return self._escaped
 
     @property
     def observables(self):
         if self._observables is None:
-            self._observables = self.get_observables()
-        return self._observables
+            print("Need to run `self.get_observables` before calling `self.observables`!")
+        else:
+            return self._observables
 
     def create_population(self, with_timing=True):
         """Create an entirely evolved population of binaries.
 
         This will sample the initial binaries and initial galaxy and then perform both the :py:mod:`cosmic`
         and :py:mod:`gala` evolution.
 
@@ -389,14 +550,17 @@
 
         self.sample_initial_binaries()
         if with_timing:
             print(f"Ended up with {self.n_binaries_match} binaries with m1 > {self.m1_cutoff} solar masses")
             print(f"[{time.time() - start:1.0e}s] Sample initial binaries")
             lap = time.time()
 
+        if self.bcm_timestep_conditions != []:
+            set_checkstates(self.bcm_timestep_conditions)
+
         self.pool = Pool(self.processes) if self.processes > 1 else None
         self.perform_stellar_evolution()
         if with_timing:
             print(f"[{time.time() - lap:1.1f}s] Evolve binaries (run COSMIC)")
             lap = time.time()
 
         self.perform_galactic_evolution(progress_bar=with_timing)
@@ -410,70 +574,91 @@
 
         if with_timing:
             print(f"Overall: {time.time() - start:1.1f}s")
 
     def sample_initial_galaxy(self):
         """Sample the initial galactic times, positions and velocities"""
         # initialise the initial galaxy class with correct number of binaries
-        self._initial_galaxy = self.galaxy_model(size=self.n_binaries_match)
+        self._initial_galaxy = self.sfh_model(size=self.n_binaries_match, **self.sfh_params)
+
+        # add relevant citations
+        self.__citations__.extend([c for c in self._initial_galaxy.__citations__ if c != "cogsworth"])
+
+        # if velocities are already set then just immediately return
+        if all(hasattr(self._initial_galaxy, attr) for attr in ["v_R", "v_T", "v_z"]):   # pragma: no cover
+            return
 
         # work out the initial velocities of each binary
         vel_units = u.km / u.s
 
         # calculate the Galactic circular velocity at the initial positions
-        v_circ = self.galactic_potential.circular_velocity(q=[self._initial_galaxy.positions.x,
-                                                              self._initial_galaxy.positions.y,
-                                                              self._initial_galaxy.positions.z]).to(vel_units)
+        v_circ = self.galactic_potential.circular_velocity(q=[self._initial_galaxy.x,
+                                                              self._initial_galaxy.y,
+                                                              self._initial_galaxy.z]).to(vel_units)
 
         # add some velocity dispersion
         v_R, v_T, v_z = np.random.normal([np.zeros_like(v_circ), v_circ, np.zeros_like(v_circ)],
                                          self.v_dispersion.to(vel_units) / np.sqrt(3),
                                          size=(3, self.n_binaries_match))
         v_R, v_T, v_z = v_R * vel_units, v_T * vel_units, v_z * vel_units
-        self._initial_galaxy._v_R = v_R
-        self._initial_galaxy._v_T = v_T
-        self._initial_galaxy._v_z = v_z
+        self._initial_galaxy.v_R = v_R
+        self._initial_galaxy.v_T = v_T
+        self._initial_galaxy.v_z = v_z
 
-    def sample_initial_binaries(self):
-        """Sample the initial binary parameters for the population"""
+    def sample_initial_binaries(self, initC=None, overwrite_initC_settings=True, reset_sampled_kicks=True):
+        """Sample the initial binary parameters for the population.
+
+        Alternatively, copy initial conditions from another population
+
+        Parameters
+        ----------
+        initC : :class:`~pandas.DataFrame`, optional
+            Initial conditions from a different Population, by default None (new sampling performed)
+        overwrite_initC_settings : `bool`, optional
+            Whether to overwrite initC settings in the case where the new population has a different set of
+            `BSE_settings`, by default True
+        reset_sampled_kicks : `bool`, optional
+            Whether to reset any sampled kicks in the population to ensure new ones are drawn, by default True
+        """
         self._bin_nums = None
 
-        # overwrite the binary fraction is the user just wants single stars
-        binfrac = self.BSE_settings["binfrac"] if self.BSE_settings["binfrac"] != 0.0 else 1.0
-        self._initial_binaries, self._mass_singles, self._mass_binaries, self._n_singles_req,\
-            self._n_bin_req = InitialBinaryTable.sampler('independent',
-                                                         self.final_kstar1, self.final_kstar2,
-                                                         binfrac_model=binfrac,
-                                                         primary_model='kroupa01', ecc_model='sana12',
-                                                         porb_model='sana12', qmin=-1,
-                                                         SF_start=self.max_ev_time.to(u.Myr).value,
-                                                         SF_duration=0.0, met=0.02, size=self.n_binaries)
-
-        # check if the user just wants single stars instead of binaries
-        if self.BSE_settings["binfrac"] == 0.0:
-            mass_1, mass_tot = Sample().sample_primary(primary_model="kroupa01",
-                                                       size=len(self._initial_binaries))
-            self._initial_binaries["mass_1"] = mass_1
-            self._initial_binaries["mass0_1"] = mass_1
-            self._initial_binaries["kstar_1"] = np.where(mass_1 > 0.7, 1, 0)
-            self._initial_binaries["kstar_2"] = np.zeros(len(self._initial_binaries))
-            self._initial_binaries["mass_2"] = np.zeros(len(self._initial_binaries))
-            self._initial_binaries["mass0_2"] = np.zeros(len(self._initial_binaries))
-            self._initial_binaries["porb"] = np.zeros(len(self._initial_binaries))
-            self._initial_binaries["sep"] = np.zeros(len(self._initial_binaries))
-            self._initial_binaries["ecc"] = np.zeros(len(self._initial_binaries))
-
-            self._mass_singles = mass_tot
-            self._mass_binaries = 0.0
-            self._n_singles_req = self.n_binaries
-            self._n_bin_req = 0
+        # if an initC table is provided then use that instead of sampling
+        if initC is not None:
+            self._initial_binaries = copy(initC)
+
+            # if we are allowed to overwrite setting then replace columns
+            if overwrite_initC_settings:
+                for key in self.BSE_settings:
+                    if key in self._initial_binaries:
+                        self._initial_binaries[key] = self.BSE_settings[key]
+
+            # reset sampled kicks if desired
+            if reset_sampled_kicks:
+                cols = ["natal_kick_1", "phi_1", "theta_1", "natal_kick_2", "phi_2", "theta_2"]
+                for col in cols:
+                    self._initial_binaries[col] = -100.0
+        else:
+            if self.BSE_settings["binfrac"] == 0.0 and not self.sampling_params["keep_singles"]:
+                raise ValueError(("You've chosen a binary fraction of 0.0 but set `keep_singles=False` (in "
+                                  "self.sampling_params), so you'll draw 0 samples...I don't think you "
+                                  "wanted to do that?"))
+            self._initial_binaries, self._mass_singles, self._mass_binaries, self._n_singles_req, \
+                self._n_bin_req = InitialBinaryTable.sampler('independent',
+                                                             self.final_kstar1, self.final_kstar2,
+                                                             binfrac_model=self.BSE_settings["binfrac"],
+                                                             SF_start=self.max_ev_time.to(u.Myr).value,
+                                                             SF_duration=0.0, met=0.02, size=self.n_binaries,
+                                                             **self.sampling_params)
 
         # apply the mass cutoff
         self._initial_binaries = self._initial_binaries[self._initial_binaries["mass_1"] >= self.m1_cutoff]
 
+        # reset index to match new `bin_num`s
+        self._initial_binaries.reset_index(inplace=True)
+
         # count how many binaries actually match the criteria (may be larger than `n_binaries` due to sampler)
         self.n_binaries_match = len(self._initial_binaries)
 
         # check that any binaries remain
         if self.n_binaries_match == 0:
             raise ValueError(("Your choice of `m1_cutoff` resulted in all samples being thrown out. Consider"
                               " a larger sample size or a less stringent mass cut"))
@@ -493,14 +678,17 @@
         # delete any cached variables
         self._final_bpp = None
         self._observables = None
         self._bin_nums = None
         self._disrupted = None
         self._escaped = None
 
+        if self.bcm_timestep_conditions != []:
+            set_checkstates(self.bcm_timestep_conditions)
+
         # if no initial binaries have been sampled then we need to create some
         if self._initial_binaries is None and self._initC is None:
             print("Warning: Initial binaries not yet sampled, performing sampling now.")
             self.sample_initial_binaries()
 
         # if initC exists then we can use that instead of initial binaries
         elif self._initial_binaries is None:
@@ -512,107 +700,129 @@
 
         # catch any warnings about overwrites
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", message=".*initial binary table is being overwritten.*")
             warnings.filterwarnings("ignore", message=".*to a different value than assumed in the mlwind.*")
 
             # perform the evolution!
-            self._bpp, self._bcm, self._initC,\
+            self._bpp, bcm, self._initC, \
                 self._kick_info = Evolve.evolve(initialbinarytable=self._initial_binaries,
-                                                BSEDict=self.BSE_settings, pool=self.pool)
+                                                BSEDict=self.BSE_settings, pool=self.pool,
+                                                timestep_conditions=self.bcm_timestep_conditions)
+
+            # only save BCM when it has interesting timesteps
+            if self.bcm_timestep_conditions != []:
+                self._bcm = bcm
 
         if no_pool_existed:
             self.pool.close()
             self.pool.join()
             self.pool = None
 
         # check if there are any NaNs in the final bpp table rows or the kick_info
         nans = np.isnan(self.final_bpp["sep"])
         kick_info_nans = np.isnan(self._kick_info["delta_vsysx_1"])
 
         # if we detect NaNs
         if nans.any() or kick_info_nans.any():      # pragma: no cover
             # make sure the user knows bad things have happened
-            print("WARNING! PANIC! THE SKY THE FALLING!")
-            print("------------------------------------")
-            print("(NaNs detected)")
+            logging.getLogger("cogsworth").warning("NaNs detected in COSMIC evolution")
 
             # store the bad things for later
             nan_bin_nums = np.unique(np.concatenate((self.final_bpp[nans]["bin_num"].values,
                                                      self._kick_info[kick_info_nans]["bin_num"].values)))
             self._bpp[self._bpp["bin_num"].isin(nan_bin_nums)].to_hdf("nans.h5", key="bpp")
             self._initC[self._initC["bin_num"].isin(nan_bin_nums)].to_hdf("nans.h5", key="initC")
             self._kick_info[self._kick_info["bin_num"].isin(nan_bin_nums)].to_hdf("nans.h5", key="kick_info")
 
             # update the population to delete any bad binaries
             n_nan = len(nan_bin_nums)
             self.n_binaries_match -= n_nan
             self._bpp = self._bpp[~self._bpp["bin_num"].isin(nan_bin_nums)]
-            self._bcm = self._bcm[~self._bcm["bin_num"].isin(nan_bin_nums)]
+
+            if self._bcm is not None:
+                self._bcm = self._bcm[~self._bcm["bin_num"].isin(nan_bin_nums)]
             self._kick_info = self._kick_info[~self._kick_info["bin_num"].isin(nan_bin_nums)]
             self._initC = self._initC[~self._initC["bin_num"].isin(nan_bin_nums)]
 
             not_nan = ~self.final_bpp["bin_num"].isin(nan_bin_nums)
             self._initial_galaxy._tau = self._initial_galaxy._tau[not_nan]
             self._initial_galaxy._Z = self._initial_galaxy._Z[not_nan]
-            self._initial_galaxy._positions = self._initial_galaxy._positions[not_nan]
-            self._initial_galaxy._v_R = self._initial_galaxy._v_R[not_nan]
-            self._initial_galaxy._v_T = self._initial_galaxy._v_T[not_nan]
-            self._initial_galaxy._v_z = self._initial_galaxy._v_z[not_nan]
-            self._initial_galaxy._which_comp = self._initial_galaxy._which_comp[not_nan]
+            self._initial_galaxy._x = self._initial_galaxy._x[not_nan]
+            self._initial_galaxy._y = self._initial_galaxy._y[not_nan]
+            self._initial_galaxy._z = self._initial_galaxy._z[not_nan]
+
+            for attr in ["v_R", "v_T", "v_z", "_which_comp"]:
+                if hasattr(self._initial_galaxy, attr):
+                    setattr(self._initial_galaxy, attr, getattr(self._initial_galaxy, attr)[not_nan])
             self._initial_galaxy._size -= n_nan
 
             # reset final bpp
             self._final_bpp = None
 
-            print(f"WARNING: {n_nan} bad binaries removed from tables - but normalisation may be off")
-            print("I've added the offending binaries to the `nan.h5` file, do with them what you will")
+            logging.getLogger("cogsworth").warning((f"{n_nan} bad binaries removed from tables - but "
+                                                    "normalisation may be off. I've added the offending "
+                                                    "binaries to a `nan.h5` file with their initC, bpp, "
+                                                    "and kick_info tables"))
 
     def perform_galactic_evolution(self, quiet=False, progress_bar=True):
         """Use :py:mod:`gala` to perform the orbital integration for each evolved binary
 
         Parameters
         ----------
         quiet : `bool`, optional
             Whether to silence any warnings about failing orbits, by default False
         """
-        # delete any cached variables
-        self._final_coords = None
+        # delete any cached variables that are based on orbits
+        self._final_pos = None
+        self._final_vel = None
         self._observables = None
 
-        # turn the drawn coordinates into an astropy representation
-        rep = self.initial_galaxy.positions.represent_as("cylindrical")
-
-        # create differentials based on the velocities (dimensionless angles allows radians conversion)
-        with u.set_enabled_equivalencies(u.dimensionless_angles()):
-            dif = coords.CylindricalDifferential(self.initial_galaxy._v_R,
-                                                 (self.initial_galaxy._v_T
-                                                  / rep.rho).to(u.rad / u.Gyr),
-                                                 self.initial_galaxy._v_z)
+        v_phi = (self.initial_galaxy.v_T / self.initial_galaxy.rho)
+        v_X = (self.initial_galaxy.v_R * np.cos(self.initial_galaxy.phi)
+               - self.initial_galaxy.rho * np.sin(self.initial_galaxy.phi) * v_phi)
+        v_Y = (self.initial_galaxy.v_R * np.sin(self.initial_galaxy.phi)
+               + self.initial_galaxy.rho * np.cos(self.initial_galaxy.phi) * v_phi)
 
         # combine the representation and differentials into a Gala PhaseSpacePosition
-        w0s = gd.PhaseSpacePosition(rep.with_differentials(dif))
+        w0s = gd.PhaseSpacePosition(pos=[a.to(u.kpc).value for a in [self.initial_galaxy.x,
+                                                                     self.initial_galaxy.y,
+                                                                     self.initial_galaxy.z]] * u.kpc,
+                                    vel=[a.to(u.km/u.s).value for a in [v_X, v_Y,
+                                                                        self.initial_galaxy.v_z]] * u.km/u.s)
+
+        # randomly drawn phase and inclination angles as necessary
+        for col in ["phase_sn_1", "phase_sn_2", "inc_sn_1", "inc_sn_2"]:
+            if col not in self.initC:
+                self.initC[col] = np.random.uniform(0, 2 * np.pi, len(self.initC))
 
         # identify the pertinent events in the evolution
-        events = identify_events(full_bpp=self.bpp, full_kick_info=self.kick_info)
+        primary_events, secondary_events = identify_events(p=self)
 
         # if we want to use multiprocessing
         if self.pool is not None or self.processes > 1:
             # track whether a pool already existed
             pool_existed = self.pool is not None
 
             # if not, create one
             if not pool_existed:
                 self.pool = Pool(self.processes)
 
-            # setup arguments and evolve the orbits from birth until present day
-            args = [(w0s[i], self.max_ev_time - self.initial_galaxy.tau[i], self.max_ev_time,
-                     copy(self.timestep_size), self.galactic_potential,
-                     events[i], self.store_entire_orbits, quiet) for i in range(self.n_binaries_match)]
+            # setup arguments to combine primary and secondaries into a single list
+            primary_args = [(w0s[i], self.max_ev_time - self.initial_galaxy.tau[i], self.max_ev_time,
+                             copy(self.timestep_size), self.galactic_potential,
+                             primary_events[i], self.store_entire_orbits, quiet)
+                            for i in range(self.n_binaries_match)]
+            secondary_args = [(w0s[i], self.max_ev_time - self.initial_galaxy.tau[i], self.max_ev_time,
+                               copy(self.timestep_size), self.galactic_potential,
+                               secondary_events[i], self.store_entire_orbits, quiet)
+                              for i in range(self.n_binaries_match) if secondary_events[i] is not None]
+            args = primary_args + secondary_args
 
+            # evolve the orbits from birth until present day
             if progress_bar:
                 orbits = self.pool.starmap(integrate_orbit_with_events,
                                            tqdm(args, total=self.n_binaries_match))
             else:
                 orbits = self.pool.starmap(integrate_orbit_with_events, args)
 
             # if a pool didn't exist before then close the one just created
@@ -623,79 +833,103 @@
         else:
             # otherwise just use a for loop to evolve the orbits from birth until present day
             orbits = []
             for i in range(self.n_binaries_match):
                 orbits.append(integrate_orbit_with_events(w0=w0s[i], potential=self.galactic_potential,
                                                           t1=self.max_ev_time - self.initial_galaxy.tau[i],
                                                           t2=self.max_ev_time, dt=copy(self.timestep_size),
-                                                          events=events[i], quiet=quiet,
+                                                          events=primary_events[i], quiet=quiet,
+                                                          store_all=self.store_entire_orbits))
+            for i in range(self.n_binaries_match):
+                if secondary_events[i] is None:
+                    continue
+                orbits.append(integrate_orbit_with_events(w0=w0s[i], potential=self.galactic_potential,
+                                                          t1=self.max_ev_time - self.initial_galaxy.tau[i],
+                                                          t2=self.max_ev_time, dt=copy(self.timestep_size),
+                                                          events=secondary_events[i], quiet=quiet,
                                                           store_all=self.store_entire_orbits))
 
+        # check for bad orbits
+        bad_orbits = np.array([orbit is None for orbit in orbits])
+
+        # if there are any bad orbits then warn the user and remove them from the population
+        if any(bad_orbits):             # pragma: no cover
+            warnings.warn(f"{bad_orbits.sum()} bad orbit(s) detected, removing them from the population" +
+                          " (initial conditions for these systems were saved to `bad_orbits.h5` file)")
+            bad_bin_nums = np.concatenate((self.bin_nums, self.bin_nums[self.disrupted]))[bad_orbits]
+
+            # save the bad orbits population
+            self.initC.loc[bad_bin_nums].to_hdf("bad_orbits.h5", key="initC")
+            self.bpp.loc[bad_bin_nums].to_hdf("bad_orbits.h5", key="bpp")
+            self.kick_info.loc[bad_bin_nums].to_hdf("bad_orbits.h5", key="kick_info")
+            self.initial_galaxy[np.isin(self.bin_nums, bad_bin_nums)].save("bad_orbits.h5", key="sfh")
+
+            # mask them out from the main population
+            new_self = self[~np.isin(self.bin_nums, bad_bin_nums)]
+            self.__dict__.update(new_self.__dict__)
+
+            orbits = np.array(orbits, dtype="object")[~bad_orbits]
+
         self._orbits = np.array(orbits, dtype="object")
 
-    def get_final_coords(self):
+    def _get_final_coords(self):
         """Get the final coordinates of each binary (or each component in disrupted binaries)
 
         Returns
         -------
-        final_coords : `tuple` of :class:`~astropy.coordinates.SkyCoord`
-            A SkyCoord object of the final positions of each binary in the galactocentric frame.
-            For bound binaries only the first SkyCoord is populated, for disrupted binaries each SkyCoord
-            corresponds to the individual components. Any missing orbits (where orbit=None or there is no
-            secondary component) will be set to `np.inf` for ease of masking.
-        """
-        # pool all of the orbits into a single numpy array
-        final_kinematics = np.ones((len(self.orbits), 2, 6)) * np.inf
-        for i, orbit in enumerate(self.orbits):
-            # check if the orbit is missing
-            if orbit is None:
-                print("Warning: Detected `None` orbit, entering coordinates as `np.inf`")
-
-            # check if it has been disrupted
-            elif isinstance(orbit, list):
-                final_kinematics[i, 0, :3] = orbit[0][-1].pos.xyz.to(u.kpc).value
-                final_kinematics[i, 1, :3] = orbit[1][-1].pos.xyz.to(u.kpc).value
-                final_kinematics[i, 0, 3:] = orbit[0][-1].vel.d_xyz.to(u.km / u.s)
-                final_kinematics[i, 1, 3:] = orbit[1][-1].vel.d_xyz.to(u.km / u.s)
-
-            # otherwise just save the system in the primary
-            else:
-                final_kinematics[i, 0, :3] = orbit[-1].pos.xyz.to(u.kpc).value
-                final_kinematics[i, 0, 3:] = orbit[-1].vel.d_xyz.to(u.km / u.s)
-
-        # turn the array into two SkyCoords
-        final_coords = [coords.SkyCoord(x=final_kinematics[:, i, 0] * u.kpc,
-                                        y=final_kinematics[:, i, 1] * u.kpc,
-                                        z=final_kinematics[:, i, 2] * u.kpc,
-                                        v_x=final_kinematics[:, i, 3] * u.km / u.s,
-                                        v_y=final_kinematics[:, i, 4] * u.km / u.s,
-                                        v_z=final_kinematics[:, i, 5] * u.km / u.s,
-                                        frame="galactocentric") for i in [0, 1]]
-        return final_coords[0], final_coords[1]
+        final_pos, final_vel : :class:`~astropy.quantity.Quantity`
+            Final positions and velocities of each system in the galactocentric frame.
+            The first `len(self)` entries of each are for bound binaries or primaries, then the final
+            `self.disrupted.sum()` entries are for disrupted secondaries. Any missing orbits (where orbit=None
+            will be set to `np.inf` for ease of masking.
+        """
+        if self._file is not None:
+            with h5.File(self._file, "r") as f:
+                offsets = f["orbits"]["offsets"][...]
+                pos, vel = f["orbits"]["pos"][...] * u.kpc, f["orbits"]["vel"][...] * u.km / u.s
+
+            final_inds = offsets[1:] - 1
+
+            self._final_pos = pos[:, final_inds].T
+            self._final_vel = vel[:, final_inds].T
+            del pos, vel
+        else:
+            # pool all of the orbits into a single numpy array
+            self._final_pos = np.ones((len(self.orbits), 3)) * np.inf
+            self._final_vel = np.ones((len(self.orbits), 3)) * np.inf
+            for i, orbit in enumerate(self.orbits):
+                # check if the orbit is missing
+                if orbit is None:
+                    print("Warning: Detected `None` orbit, entering coordinates as `np.inf`")
+                else:
+                    self._final_pos[i] = orbit[-1].pos.xyz.to(u.kpc).value
+                    self._final_vel[i] = orbit[-1].vel.d_xyz.to(u.km / u.s).value
+            self._final_pos *= u.kpc
+            self._final_vel *= u.km / u.s
+        return self._final_pos, self._final_vel
 
-    def get_observables(self, filters=['J', 'H', 'K', 'G', 'BP', 'RP'], ignore_extinction=False):
+    def get_observables(self, **kwargs):
         """Get observables associated with the binaries at present day.
 
         These include: extinction due to dust, absolute and apparent bolometric magnitudes for each star,
         apparent magnitudes in each filter and observed temperature and surface gravity for each binary.
 
         For bound binaries and stellar mergers, only the column `{filter}_app_1` is relevant. For
         disrupted binaries, `{filter}_app_1` is for the primary star and `{filter}_app_2` is for
         the secondary star.
 
         Parameters
         ----------
-        filters : `list`, optional
-            Which filters to compute observables for, by default ['J', 'H', 'K', 'G', 'BP', 'RP']
-        ignore_extinction : `bool`
-            Whether to ignore extinction
+        **kwargs to pass to :func:`~cogsworth.observables.get_photometry`
         """
-        return get_photometry(self.final_bpp, self.final_coords, filters, ignore_extinction=ignore_extinction)
+        self.__citations__.extend(["MIST", "MESA", "bayestar2019"])
+        self._observables = get_photometry(population=self, **kwargs)
+        return self._observables
 
-    def get_gaia_observed_bin_nums(self):
+    def get_gaia_observed_bin_nums(self, ra=None, dec=None):
         """Get a list of ``bin_nums`` of systems that are bright enough to be observed by Gaia.
 
         This is calculated based on the Gaia selection function provided by :mod:`gaiaunlimited`. This
         function returns a **random sample** of systems where systems are included in the observed subset
         with a probability given by Gaia's completeness at their location.
 
         E.g. if Gaia's completeness is 0 for a source of a given magnitude and location then it will never be
@@ -707,30 +941,35 @@
         primary_observed : :class:`~numpy.ndarray`
             A list of binary numbers (that can be used in tables like :attr:`final_bpp`) for which the
             bound binary/disrupted primary would be observed
         secondary_observed : :class:`~numpy.ndarray`
             A list of binary numbers (that can be used in tables like :attr:`final_bpp`) for which the
             disrupted secondary would be observed
         """
+        assert check_dependencies("gaiaunlimited")
+        from gaiaunlimited.selectionfunctions import DR3SelectionFunctionTCG
+        from gaiaunlimited.utils import get_healpix_centers
+
+        self.__citations__.append("gaia-selection-function")
         # get coordinates of the centres of the healpix pixels in a nside=2**7
         coords_of_centers = get_healpix_centers(7)
 
         # get the Gaia selection function for this healpix order
         dr3sf = DR3SelectionFunctionTCG()
 
         # work out the index of each pixel for every binary
-        pix_inds = self.get_healpix_inds(nside=128)
+        pix_inds = self.get_healpix_inds(ra=ra, dec=dec, nside=128)
 
         # loop over first (all bound binaries & primaries from disrupted binaries)
         # and then (secondaries from disrupted binaries)
         observed = []
-        all_bin_nums = self.final_bpp["bin_num"].values
-        for pix, g_mags, bin_nums in zip(pix_inds, [self.observables["G_app_1"].values,
-                                                    self.observables["G_app_2"][self.disrupted].values],
-                                         [all_bin_nums, all_bin_nums[self.disrupted]]):
+        for pix, g_mags, bin_nums in zip([pix_inds[:len(self)], pix_inds[len(self):]],
+                                         [self.observables["G_app_1"].values,
+                                          self.observables["G_app_2"][self.disrupted].values],
+                                         [self.bin_nums, self.bin_nums[self.disrupted]]):
             # get the coordinates of the corresponding pixels
             comp_coords = coords_of_centers[pix]
 
             # ensure any NaNs in the magnitudes are just set to super faint
             g_mags = np.nan_to_num(g_mags, nan=1000)
             g_mags = g_mags.value if hasattr(g_mags, 'unit') else g_mags
 
@@ -747,42 +986,91 @@
                 observed_bin_nums = bin_nums[np.random.uniform(size=len(completeness)) < completeness]
 
             observed.append(observed_bin_nums)
 
         primary_observed, secondary_observed = observed
         return primary_observed, secondary_observed
 
-    def get_healpix_inds(self, nside=128):
+    def get_final_mw_skycoord(self):
+        """Get the final positions and velocities as an astropy SkyCoord object
+
+        ..warning::
+
+            This function assumes the final positions and velocities are in the MW galactocentric frame"""
+        return coords.SkyCoord(x=self.final_pos[:, 0], y=self.final_pos[:, 1], z=self.final_pos[:, 2],
+                               v_x=self.final_vel[:, 0], v_y=self.final_vel[:, 1], v_z=self.final_vel[:, 2],
+                               representation_type="cartesian", unit=u.kpc, frame="galactocentric")
+
+    def plot_sky_locations(self, fig=None, ax=None, show=True, show_galactic_plane=True, **kwargs):
+        """Plot the final positions of the binaries in the Milky Way galactocentric frame"""
+        assert check_dependencies(["healpy", "matplotlib"])
+        import matplotlib.pyplot as plt
+
+        # get the final positions and velocities
+        final_coords = self.get_final_mw_skycoord().icrs
+
+        # plot the positions
+        if fig is None or ax is None:
+            fig, ax = plt.subplots()
+
+        # plot the galactic plane if desired
+        if show_galactic_plane:
+            galactic_plane = coords.SkyCoord(l=np.linspace(1e-10, 2 * np.pi, 10000), b=np.zeros(10000),
+                                             unit="rad", frame="galactic").transform_to("icrs")
+            in_order = np.argsort(galactic_plane.ra.value)
+            ax.plot(galactic_plane.ra.value[in_order], galactic_plane.dec.value[in_order],
+                    label="Galactic Plane", color="black" if ax.get_facecolor() == (1,1,1,0) else "white",
+                    linestyle="dotted")
+
+        ax.scatter(final_coords.ra.value, final_coords.dec.value, **kwargs)
+        ax.set(xlabel="Right Ascension [deg]", ylabel="Declination [deg]")
+        ax.legend()
+
+        if show:
+            plt.show()
+        return fig, ax
+
+    def get_healpix_inds(self, ra=None, dec=None, nside=128):
         """Get the indices of the healpix pixels that each binary is in
 
         Parameters
         ----------
+        ra : `float` or `str`
+            Either the right ascension of the system in radians or "auto" to automatically calculate assuming
+            Milky Way galactocentric coordinates
+        dec : `float` or `str`
+            Either the declination of the system in radians or "auto" to automatically calculate assuming
+            Milky Way galactocentric coordinates
         nside : `int`, optional
             Healpix nside parameter, by default 128
 
         Returns
         -------
         pix : :class:`~numpy.ndarray`
-            The indices for the bound binaries/primaries of disrupted binaries
-            (corresponds to ``self.final_coords[0]``)
-        disrupted_pix : :class:`~numpy.ndarray`
-            The indices for the secondaries of disrupted binaries
-            (corresponds to ``self.final_coords[1][self.disrupted]``)
+            The indices for each system
         """
+        assert check_dependencies("healpy")
+        import healpy as hp
+
+        if ra is None or dec is None:
+            raise ValueError("You must provide both `ra` and `dec`, or set them to 'auto'")
+        if ra == "auto" or dec == "auto":
+            final_coords = self.get_final_mw_skycoord()
+            ra = final_coords.icrs.ra.to(u.rad).value
+            dec = final_coords.icrs.dec.to(u.rad).value
+
         # get the coordinates in right format
-        colatitudes = [np.pi/2 - self.final_coords[i].icrs.dec.to(u.rad).value for i in [0, 1]]
-        longitudes = [self.final_coords[i].icrs.ra.to(u.rad).value for i in [0, 1]]
+        colatitudes = np.pi / 2 - dec
+        longitudes = ra
 
         # find the pixels for each bound binary/primary and for each disrupted secondary
-        pix = hp.ang2pix(nside, nest=True, theta=colatitudes[0], phi=longitudes[0])
-        disrupted_pix = hp.ang2pix(nside, nest=True,
-                                   theta=colatitudes[1][self.disrupted], phi=longitudes[1][self.disrupted])
-        return pix, disrupted_pix
+        pix = hp.ang2pix(nside, nest=True, theta=colatitudes, phi=longitudes)
+        return pix
 
-    def plot_map(self, nside=128, coord="C",
+    def plot_map(self, ra=None, dec=None, nside=128, coord="C",
                  cmap="magma", norm="log", unit=None, show=True, **mollview_kwargs):
         r"""Plot a healpix map of the final positions of all binaries in population
 
         Parameters
         ----------
         nside : `int`, optional
             Healpix nside parameter, by default 128
@@ -798,21 +1086,25 @@
             if ``norm==log`` and ":math:`N_{\rm binaries}`" if ``norm==linear``
         show : `bool`, optional
             Whether to immediately show the plot, by default True
         **mollview_kwargs
             Any additional arguments that you want to pass to healpy's
             `mollview <https://healpy.readthedocs.io/en/latest/generated/healpy.visufunc.mollview.html>`_
         """
-        pix, disrupted_pix = self.get_healpix_inds(nside=nside)
+        assert check_dependencies(["healpy", "matplotlib"])
+        import healpy as hp
+        import matplotlib.pyplot as plt
+
+        pix = self.get_healpix_inds(ra=ra, dec=dec, nside=nside)
 
         # initialise an empty map
         m = np.zeros(hp.nside2npix(nside))
 
         # count the unique pixel values and how many sources are in each
-        inds, counts = np.unique(np.concatenate([pix, disrupted_pix]), return_counts=True)
+        inds, counts = np.unique(pix, return_counts=True)
 
         # apply a log if desired
         if norm == "log":
             counts = np.log10(counts)
 
         # fill in the map
         m[inds] = counts
@@ -831,22 +1123,94 @@
         # create a mollview plot
         hp.mollview(m, nest=True, cmap=cmap, coord=coord, unit=unit, **mollview_kwargs)
 
         # show it if the user wants
         if show:
             plt.show()
 
-    def save(self, file_name, overwrite=False):
-        """Save a Population to disk
+    def translate_tables(self, **kwargs):
+        """Translate the COSMIC BSE tables to human readable format
+
+        Parameters
+        ----------
+
+        **kwargs : `various`
+            Any arguments to pass to :func:`~cogsworth.utils.translate_COSMIC_tables`
+        """
+        with pd.option_context('mode.chained_assignment', None):
+            self._bpp = translate_COSMIC_tables(self._bpp, **kwargs)
+            self._final_bpp = translate_COSMIC_tables(self._final_bpp, **kwargs)
 
-        This will produce 4 files:
-            - An HDF5 file containing most of the data
-            - A .npy file containing the orbits
-            - A .txt file detailing the Galactic potential used
-            - A .txt file detailing the initial galaxy model used
+            if self._bcm is not None:
+                kwargs.update({"evol_type": False})
+                self._bcm = translate_COSMIC_tables(self._bcm, **kwargs)
+
+    def plot_cartoon_binary(self, bin_num, **kwargs):
+        """Plot a cartoon of the evolution of a single binary
+
+        Parameters
+        ----------
+        bin_num : `int`
+            Which binary to plot
+        **kwargs : `various`
+            Keyword arguments to pass, see :func:`~cogsworth.plot.plot_cartoon_evolution` for options
+
+        Returns
+        -------
+        fig, ax : :class:`~matplotlib.pyplot.figure`, :class:`~matplotlib.pyplot.axis`
+            Figure and axis of the plot
+        """
+        return plot_cartoon_evolution(self.bpp, bin_num, **kwargs)
+
+    def to_legwork_sources(self, distances=None, assume_mw_galactocentric=False):
+        """Convert the final state of the population to a LEGWORK Source class (only including bound binaries)
+
+        Parameters
+        ----------
+        distances : :class:`np.ndarray`, optional
+            Custom distance to each source, by default None
+        assume_mw_galactocentric : `bool`, optional
+            Assume population is in Milky Way and galactocentric coordinate system - such that distances can
+            be calculated assuming the present location of the Earth, by default False
+
+        Returns
+        -------
+        sources : :class:`~legwork.sources.Source`
+            LEGWORK sources
+
+        Raises
+        ------
+        ValueError
+            When distances aren't provided and assume_mw_galactocentric=False
+        """
+        assert check_dependencies(["legwork"])
+        import legwork as lw
+        self.__citations__.append("legwork")
+
+        # calculate distances as necessary
+        if distances is None and not assume_mw_galactocentric:
+            raise ValueError("Must either provide distances or set assume_mw_galactocentric=True")
+        elif distances is None:
+            final_coords = coords.SkyCoord(x=self.final_pos[:, 0], y=self.final_pos[:, 1],
+                                           z=self.final_pos[:, 2], frame="galactocentric", unit=u.kpc,
+                                           representation_type="cartesian")
+            distances = final_coords.icrs.distance[:len(self)]
+
+        # mask on only bound binaries
+        binaries = self.final_bpp["sep"] > 0.0
+
+        # construct LEGWORK sources
+        return lw.source.Source(m_1=self.final_bpp["mass_1"].values[binaries] * u.Msun,
+                                m_2=self.final_bpp["mass_2"].values[binaries] * u.Msun,
+                                a=self.final_bpp["sep"].values[binaries] * u.Rsun,
+                                ecc=self.final_bpp["ecc"].values[binaries],
+                                dist=distances[binaries], interpolate_g=binaries.sum() > 1000)
+
+    def save(self, file_name, overwrite=False):
+        """Save a Population to disk as an HDF5 file.
 
         Parameters
         ----------
         file_name : `str`
             A file name to use. Either no file extension or ".h5".
         overwrite : `bool`, optional
             Whether to overwrite any existing files, by default False
@@ -861,91 +1225,147 @@
         if os.path.isfile(file_name):
             if overwrite:
                 os.remove(file_name)
             else:
                 raise FileExistsError((f"{file_name} already exists. Set `overwrite=True` to overwrite "
                                        "the file."))
         self.bpp.to_hdf(file_name, key="bpp")
-        self.bcm.to_hdf(file_name, key="bcm")
+
+        if self._bcm is not None:
+            self._bcm.to_hdf(file_name, key="bcm")
         self.initC.to_hdf(file_name, key="initC")
         self.kick_info.to_hdf(file_name, key="kick_info")
 
-        self.galactic_potential.save(file_name.replace('.h5', '-potential.txt'))
+        with h5.File(file_name, "a") as f:
+            f.attrs["potential_dict"] = yaml.dump(potential_to_dict(self.galactic_potential),
+                                                  default_flow_style=None)
         self.initial_galaxy.save(file_name, key="initial_galaxy")
-        np.save(file_name.replace(".h5", "-orbits.npy"), np.array(self.orbits, dtype="object"))
+
+        # save the orbits if they have been calculated/loaded
+        if self._orbits is not None:
+            # go through the orbits calculate their lengths (and therefore offsets in the file)
+            orbit_lengths = [len(orbit.pos) for orbit in self.orbits]
+            orbit_lengths_total = sum(orbit_lengths)
+            offsets = np.insert(np.cumsum(orbit_lengths), 0, 0)
+
+            # start some empty arrays to store the data
+            orbits_data = {"offsets": offsets,
+                           "pos": np.zeros((3, orbit_lengths_total)),
+                           "vel": np.zeros((3, orbit_lengths_total)),
+                           "t": np.zeros(orbit_lengths_total)}
+
+            # save each orbit to the arrays with the same units
+            for i, orbit in enumerate(self.orbits):
+                orbits_data["pos"][:, offsets[i]:offsets[i + 1]] = orbit.pos.xyz.to(u.kpc).value
+                orbits_data["vel"][:, offsets[i]:offsets[i + 1]] = orbit.vel.d_xyz.to(u.km / u.s).value
+                orbits_data["t"][offsets[i]:offsets[i + 1]] = orbit.t.to(u.Myr).value
+
+            # save the orbits arrays to the file
+            with h5.File(file_name, "a") as file:
+                orbits = file.create_group("orbits")
+                for key in orbits_data:
+                    orbits[key] = orbits_data[key]
 
         with h5.File(file_name, "a") as file:
             numeric_params = np.array([self.n_binaries, self.n_binaries_match, self.processes, self.m1_cutoff,
                                        self.v_dispersion.to(u.km / u.s).value,
                                        self.max_ev_time.to(u.Gyr).value, self.timestep_size.to(u.Myr).value,
                                        self.mass_singles, self.mass_binaries, self.n_singles_req,
                                        self.n_bin_req])
             num_par = file.create_dataset("numeric_params", data=numeric_params)
             num_par.attrs["store_entire_orbits"] = self.store_entire_orbits
 
-            k_stars = np.array([self.final_kstar1, self.final_kstar2])
-            file.create_dataset("k_stars", data=k_stars)
+            num_par.attrs["final_kstar1"] = self.final_kstar1
+            num_par.attrs["final_kstar2"] = self.final_kstar2
+            num_par.attrs["timestep_conditions"] = self.bcm_timestep_conditions
 
             # save BSE settings
             d = file.create_dataset("BSE_settings", data=[])
             for key in self.BSE_settings:
                 d.attrs[key] = self.BSE_settings[key]
 
+            # save sampling params
+            d = file.create_dataset("sampling_params", data=[])
+            for key in self.sampling_params:
+                d.attrs[key] = self.sampling_params[key]
 
-def load(file_name):
+
+def load(file_name, parts=["initial_binaries", "initial_galaxy", "stellar_evolution"]):
     """Load a Population from a series of files
 
     Parameters
     ----------
     file_name : `str`
         Base name of the files to use. Should either have no file extension or ".h5"
+    parts : `list`, optional
+        Which parts of the Population to load immediately, the rest are loaded as necessary. Any of
+        ["initial_binaries", "initial_galaxy", "stellar_evolution", "galactic_orbits"], by default
+        ["initial_binaries", "initial_galaxy", "stellar_evolution"]
 
     Returns
     -------
     pop : `Population`
         The loaded Population
     """
     if file_name[-3:] != ".h5":
         file_name += ".h5"
 
     BSE_settings = {}
+    sampling_params = {}
     with h5.File(file_name, "r") as file:
+        if "numeric_params" not in file.keys():
+            raise ValueError((f"{file_name} is not a Population file, "
+                             "perhaps you meant to use `cogsworth.sfh.load`?"))
         numeric_params = file["numeric_params"][...]
-        k_stars = file["k_stars"][...]
 
         store_entire_orbits = file["numeric_params"].attrs["store_entire_orbits"]
+        final_kstars = [file["numeric_params"].attrs["final_kstar1"],
+                        file["numeric_params"].attrs["final_kstar2"]]
+        bcm_tc = file["numeric_params"].attrs["timestep_conditions"]
 
         # load in BSE settings
         for key in file["BSE_settings"].attrs:
             BSE_settings[key] = file["BSE_settings"].attrs[key]
 
-    initial_galaxy = galaxy.load(file_name, key="initial_galaxy")
-    galactic_potential = gp.potential.load(file_name.replace('.h5', '-potential.txt'))
+        # load in sampling params
+        for key in file["sampling_params"].attrs:
+            sampling_params[key] = file["sampling_params"].attrs[key]
+
+    with h5.File(file_name, 'r') as f:
+        galactic_potential = potential_from_dict(yaml.load(f.attrs["potential_dict"], Loader=yaml.Loader))
 
     p = Population(n_binaries=int(numeric_params[0]), processes=int(numeric_params[2]),
-                   m1_cutoff=numeric_params[3], final_kstar1=k_stars[0], final_kstar2=k_stars[1],
-                   galaxy_model=initial_galaxy.__class__, galactic_potential=galactic_potential,
+                   m1_cutoff=numeric_params[3], final_kstar1=final_kstars[0], final_kstar2=final_kstars[1],
+                   sfh_model=sfh.StarFormationHistory, galactic_potential=galactic_potential,
                    v_dispersion=numeric_params[4] * u.km / u.s, max_ev_time=numeric_params[5] * u.Gyr,
                    timestep_size=numeric_params[6] * u.Myr, BSE_settings=BSE_settings,
-                   store_entire_orbits=store_entire_orbits)
+                   sampling_params=sampling_params, store_entire_orbits=store_entire_orbits,
+                   bcm_timestep_conditions=bcm_tc)
 
+    p._file = file_name
     p.n_binaries_match = int(numeric_params[1])
     p._mass_singles = numeric_params[7]
     p._mass_binaries = numeric_params[8]
     p._n_singles_req = numeric_params[9]
     p._n_bin_req = numeric_params[10]
 
-    p._initial_galaxy = initial_galaxy
-
-    p._bpp = pd.read_hdf(file_name, key="bpp")
-    p._bcm = pd.read_hdf(file_name, key="bcm")
-    p._initC = pd.read_hdf(file_name, key="initC")
-    p._kick_info = pd.read_hdf(file_name, key="kick_info")
+    # load parts as necessary
+    if "initial_binaries" in parts:
+        p.initC
+
+    if "initial_galaxy" in parts:
+        p.initial_galaxy
+
+    if "stellar_evolution" in parts:
+        p.kick_info
+        p.bcm
+        p.bpp
 
-    p._orbits = np.load(file_name.replace(".h5", "-orbits.npy"), allow_pickle=True)
+    if "galactic_orbits" in parts:
+        p.orbits
 
     return p
 
 
 class EvolvedPopulation(Population):
     def __init__(self, n_binaries, mass_singles=None, mass_binaries=None, n_singles_req=None, n_bin_req=None,
                  bpp=None, bcm=None, initC=None, kick_info=None, **pop_kwargs):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cogsworth-0.0/cogsworth/tests/test_classify.py` & `cogsworth-1.0.0/cogsworth/tests/test_classify.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,22 +28,23 @@
         except Exception as e:
             print(e)
             it_broke = True
         self.assertFalse(it_broke)
 
     def test_x_rays(self):
         """Test x-ray luminosity calculation"""
-        p = cogsworth.pop.Population(10, final_kstar1=[13, 14])
+        p = cogsworth.pop.Population(10, final_kstar1=[13, 14], bcm_timestep_conditions=[['dtp=100000.0']])
         bcm = p.bcm.drop_duplicates(subset="bin_num", keep='last')
         it_broke = False
         try:
             cogsworth.classify.get_x_ray_lum(bcm["mass_1"].values * u.Msun, bcm["rad_1"].values * u.Rsun,
-                                          bcm["deltam_1"].values * u.Msun / u.yr, bcm["porb"].values * u.day,
-                                          bcm["kstar_1"].values,
-                                          bcm["mass_2"].values * u.Msun, bcm["RRLO_2"].values)
+                                             bcm["deltam_1"].values * u.Msun / u.yr,
+                                             bcm["porb"].values * u.day,
+                                             bcm["kstar_1"].values,
+                                             bcm["mass_2"].values * u.Msun, bcm["RRLO_2"].values)
         except Exception as e:
             print(e)
             it_broke = True
         self.assertFalse(it_broke)
 
         it_broke = False
         try:
```

### Comparing `cogsworth-0.0/cogsworth/tests/test_events.py` & `cogsworth-1.0.0/cogsworth/tests/test_events.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,46 +3,54 @@
 import pandas as pd
 
 
 class Test(unittest.TestCase):
     def test_various_events(self):
         """Ensure functions work for different kinds of events
 
-        I'm going to use fake bpp and kick_info tables for this. There will have four binaries
+        I'm going to use fake bpp and kick_info tables for this. There will be four binaries
             - One with no events
             - One with a bound binary and a kick
             - One with a disruption from the first SN
             - One with a disruption from the second SN
         """
 
         bpp_dict = {
-            "mass_1": [1, 10, 20, 20, 20],
-            "mass_2": [1, 10, 20, 20, 20],
-            "tphys": [0, 0, 0, 0, 1],
-            "sep": [10, 10, 10, 10, 10],
-            "ecc": [0, 0, 0, 0, 0.1],
-            "evol_type": [-1, 15, 15, 15, 16],
-            "bin_num": [1, 2, 3, 4, 4],
+            "mass_1": [1, 10, 20, 1.4, 20, 20, 8],
+            "mass_2": [1, 10, 20, 20, 20, 20, 1.4],
+            "tphys": [0, 0, 0, 1, 0, 1, 2],
+            "sep": [10, 10, 10, -1.0, 10, 10, -1.0],
+            "ecc": [0, 0, 0, -1.0, 0, 0.1, -1.0],
+            "evol_type": [-1, 15, 15, 11, 15, 16, 11],
+            "bin_num": [0, 1, 2, 2, 3, 3, 3],
         }
         bpp = pd.DataFrame(data=bpp_dict)
         bpp.set_index("bin_num", drop=False, inplace=True)
 
         kick_info_dict = {
             "star": [0, 1, 1, 1, 2],
             "disrupted": [0, 0, 1, 0, 1],
             "delta_vsysx_1": [0, 0, 0, 0, 0],
             "delta_vsysy_1": [0, 0, 0, 0, 0],
             "delta_vsysz_1": [0, 0, 0, 0, 0],
             "delta_vsysx_2": [0, 0, 0, 0, 0],
             "delta_vsysy_2": [0, 0, 0, 0, 0],
             "delta_vsysz_2": [0, 0, 0, 0, 0],
-            "bin_num": [1, 2, 3, 4, 4],
+            "bin_num": [0, 1, 2, 3, 3],
         }
         kick_info = pd.DataFrame(data=kick_info_dict)
         kick_info.set_index("bin_num", drop=False, inplace=True)
 
-        events = cogsworth.events.identify_events(bpp, kick_info)
-
-        self.assertTrue(events[0] is None)
-        self.assertTrue(len(events[1]) == 1)
-        self.assertTrue(len(events[2]) == 2)
-        self.assertTrue(len(events[3]) == 2)
+        p = cogsworth.pop.Population(4)
+        p._bpp = bpp
+        p._kick_info = kick_info
+        p._initC = pd.DataFrame(data={"metallicity": [1e-2, 1e-2, 1e-2, 1e-2]})
+        p.final_bpp
+
+        primary_events, secondary_events = cogsworth.events.identify_events(p)
+
+        self.assertTrue(len(primary_events) == 4)
+        self.assertTrue(len(secondary_events) == 4)
+        self.assertTrue(primary_events[0] is None)
+        self.assertTrue(secondary_events[1] is None)
+        self.assertTrue(secondary_events[2] is not None)
+        self.assertTrue(len(secondary_events[3]) > len(secondary_events[2]))
```

### Comparing `cogsworth-0.0/cogsworth/tests/test_galaxy.py` & `cogsworth-1.0.0/cogsworth/tests/test_galaxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import unittest
-import cogsworth.galaxy as galaxy
+import cogsworth.sfh as sfh
 import os
 
 
 class Test(unittest.TestCase):
     def test_basic_class(self):
         """Check that base class can't be used alone"""
 
-        g = galaxy.Galaxy(size=10000, components=[""], component_masses=[1],
-                          immediately_sample=False)
+        g = sfh.StarFormationHistory(size=10000, components=[""], component_masses=[1],
+                                     immediately_sample=False)
         it_broke = False
         try:
             g.draw_lookback_times()
         except NotImplementedError:
             it_broke = True
         self.assertTrue(it_broke)
 
@@ -43,74 +43,80 @@
             g.get_metallicity()
         except NotImplementedError:
             it_broke = True
         self.assertTrue(it_broke)
 
     def test_bad_inputs(self):
         """Ensure the classes fail with bad input"""
-        g = galaxy.Frankel2018(size=None, immediately_sample=False)
+        g = sfh.Wagg2022(size=None, immediately_sample=False)
         it_broke = False
         try:
             g.sample()
         except ValueError:
             it_broke = True
         self.assertTrue(it_broke)
 
-        g = galaxy.Frankel2018(size=100, components=None, component_masses=None,
-                               immediately_sample=False)
+        g = sfh.Wagg2022(size=100, components=None, component_masses=None, immediately_sample=False)
         it_broke = False
         try:
             g.sample()
         except ValueError:
             it_broke = True
         self.assertTrue(it_broke)
 
     def test_valid_ranges(self):
         """Check that the drawn variables have valid ranges"""
-        g = galaxy.Frankel2018(size=10000)
+        g = sfh.Wagg2022(size=10000)
 
         self.assertTrue((g.tau.min() >= 0) & (g.tau.max() <= g.galaxy_age))
         self.assertTrue(g.Z.min() >= 0.0)
 
     def test_io(self):
         """Check that a galaxy can be saved and re-loaded"""
-        g = galaxy.Frankel2018(size=10000)
+        g = sfh.Wagg2022(size=10000)
 
         g.save("testing-galaxy-io")
 
-        g_loaded = galaxy.load("testing-galaxy-io")
+        g_loaded = sfh.load("testing-galaxy-io")
 
         self.assertTrue(np.all(g.tau == g_loaded.tau))
-        self.assertTrue(np.all(g.positions.icrs.distance == g_loaded.positions.icrs.distance))
+        self.assertTrue(np.all(g.rho == g_loaded.rho))
+        self.assertTrue(np.all(g.z == g_loaded.z))
 
         os.remove("testing-galaxy-io.h5")
-        os.remove("testing-galaxy-io-galaxy-params.txt")
 
     def test_getters(self):
         """Test getting attributes"""
         it_broke = False
         try:
-            g = galaxy.Frankel2018(size=10, immediately_sample=False)
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
+            len(g)
             g.components
             g.component_masses
             g.tau
-            g = galaxy.Frankel2018(size=10, immediately_sample=False)
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
             g.Z
-            g = galaxy.Frankel2018(size=10, immediately_sample=False)
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
+            g.x
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
+            g.y
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
+            g.z
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
             g.positions
-            g = galaxy.Frankel2018(size=10, immediately_sample=False)
+            g = sfh.Wagg2022(size=10, immediately_sample=False)
             g.which_comp
         except Exception as e:
             print(e)
             it_broke = True
         self.assertFalse(it_broke)
 
     def test_setters(self):
         """Test setting attributes"""
-        g = galaxy.Frankel2018(size=10000, immediately_sample=False)
+        g = sfh.Wagg2022(size=10000, immediately_sample=False)
         g.size = 100
         self.assertTrue(g.size == 100)
 
         # make sure it crashes for invalid inputs
         it_broke = False
         try:
             g.size = -1
@@ -124,33 +130,33 @@
         except ValueError:
             it_broke = True
         self.assertTrue(it_broke)
 
     def test_custom_galaxy(self):
         """Test saving a custom galaxy class"""
 
-        class Custom(galaxy.Frankel2018):
+        class Custom(sfh.Wagg2022):
             def __init__(self, size, components=["low_alpha_disc"], component_masses=[1], **kwargs):
                 super().__init__(size, components, component_masses, **kwargs)
 
         g = Custom(size=100)
 
         g.save("testing-galaxy-custom")
 
-        g_loaded = galaxy.load("testing-galaxy-custom")
+        g_loaded = sfh.load("testing-galaxy-custom")
 
         self.assertTrue(np.all(g.tau == g_loaded.tau))
-        self.assertTrue(np.all(g.positions.icrs.distance == g_loaded.positions.icrs.distance))
+        self.assertTrue(np.all(g.rho == g_loaded.rho))
+        self.assertTrue(np.all(g.z == g_loaded.z))
 
         os.remove("testing-galaxy-custom.h5")
-        os.remove("testing-galaxy-custom-galaxy-params.txt")
 
     def test_plot(self):
         """Test plotting capabilities"""
-        g = galaxy.Frankel2018(size=1000)
+        g = sfh.Wagg2022(size=1000)
 
         it_broke = False
         try:
             g.plot(component="low_alpha_disc", xlim=(-20, 20), ylim=(-20, 20), zlim=(-7, 7), show=False)
             g.plot(coordinates="cylindrical", component="low_alpha_disc", show=False)
         except Exception as e:
             print(e)
@@ -162,15 +168,15 @@
             g.plot(coordinates="nonsense")
         except ValueError:
             it_broke = True
         self.assertTrue(it_broke)
 
     def test_indexing(self):
         """Ensure that indexing works correctly (reprs too)"""
-        g = galaxy.Frankel2018(size=10)
+        g = sfh.Wagg2022(size=10)
         print(g)
 
         # make sure it fails for strings
         it_worked = True
         try:
             g["absolute nonsense mate"]
         except ValueError:
```

### Comparing `cogsworth-0.0/cogsworth.egg-info/PKG-INFO` & `cogsworth-1.0.0/cogsworth.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: cogsworth
-Version: 0.0
+Version: 1.0.0
 Summary: A framework for performing self-consistent population synthesis and orbital integration
 Home-page: https://github.com/TomWagg/cogsworth
 Author: Tom Wagg
 Author-email: tomjwagg@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: extras
+Provides-Extra: observables
+Provides-Extra: actions
+Provides-Extra: lisa
+Provides-Extra: hydro
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 
 <h1 align="center">Cogsworth</h1>
-<p align="center">A Python package for self-consistently performing population synthesis and orbital integration</p>
+<p align="center">A Python package for performing self-consistent population synthesis and galactic dynamics simulations</p>
 <p align="center">
   <a href='https://cogsworth.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/cogsworth/badge/?version=latest' alt='Documentation Status' />
 </a>
   <br>
   <img width=500 src="https://user-images.githubusercontent.com/21990332/194442782-49afc013-2c53-4638-bcb7-c0970319c2bd.png">
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: cogsworth Version: 0.0 Summary: A framework for
+Metadata-Version: 2.1 Name: cogsworth Version: 1.0.0 Summary: A framework for
 performing self-consistent population synthesis and orbital integration Home-
 page: https://github.com/TomWagg/cogsworth Author: Tom Wagg Author-email:
 tomjwagg@gmail.com License: MIT Requires-Python: >=3.10 Description-Content-
-Type: text/markdown Provides-Extra: test Provides-Extra: docs License-File:
-LICENSE
+Type: text/markdown Provides-Extra: all Provides-Extra: extras Provides-Extra:
+observables Provides-Extra: actions Provides-Extra: lisa Provides-Extra: hydro
+Provides-Extra: test Provides-Extra: docs License-File: LICENSE
                             ************ CCooggsswwoorrtthh ************
-  A Python package for self-consistently performing population synthesis and
-                              orbital integration
+   A Python package for performing self-consistent population synthesis and
+                         galactic dynamics simulations
                             _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
  [https://user-images.githubusercontent.com/21990332/194442782-49afc013-2c53-
                           4638-bcb7-c0970319c2bd.png]
```

### Comparing `cogsworth-0.0/setup.cfg` & `cogsworth-1.0.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -12,39 +12,77 @@
 [options]
 python_requires = >=3.10
 packages = find:
 install_requires = 
 	numpy == 1.23
 	numba == 0.57
 	pip
-	matplotlib
-	astropy
-	scipy >= 1.7.3
-	pandas
-	gala >= 1.6
-	cosmic-popsynth >= 3.4.7
-	nose
-	tables
-	isochrones @ git+https://github.com/TomWagg/isochrones.git
-	dustmaps
-	healpy
-	gaiaunlimited >= 0.2.0
+	matplotlib >= 3.7
+	astropy >= 5.0, < 6.0
+	scipy >= 1.8
+	pandas >= 2.1
+	gala >= 1.7
+	cosmic-popsynth >= 3.4.10
 
 [options.package_data]
 * = *.npy, *.npz
 
 [options.extras_require]
+all = 
+	%(observables)s
+	%(actions)s
+	%(test)s
+	%(docs)s
+extras = 
+	%(observables)s
+	%(actions)s
+	%(hydro)s
+	%(lisa)s
+observables = 
+	nose
+	tables
+	isochrones
+	dustmaps
+	healpy
+	gaiaunlimited >= 0.2.0
+actions = 
+	agama
+lisa = 
+	legwork >= 0.4.6
+hydro = 
+	pynbody
 test = 
+	%(observables)s
+	%(lisa)s
+	%(hydro)s
 	pytest
+	flake8
+	coverage
+	pytest-xdist
+	nbmake
+	pytest-cov
 docs = 
-	sphinx
-	matplotlib
+	%(observables)s
+	%(hydro)s
+	sphinx<7.2
+	matplotlib<3.9
+	nbsphinx>=0.8.6
+	numpydoc
+	pydata-sphinx-theme
+	sphinx_automodapi
+	sphinxcontrib.bibtex
+	IPython
+	ipykernel
+	sphinx_copybutton
+	sphinx-gallery>=0.13.0
+	sphinx-design>=0.4.1
+	sphinx_togglebutton
 
 [tool:pytest]
-addopts = --cov-report xml:cov.xml --cov cogsworth
+addopts = --cov-report xml:cov.xml --cov cogsworth -n='auto'
 testpaths = "cogsworth"
 
 [coverage:run]
 omit = 
 	cogsworth/tests/*
 	cogsworth/__init__.py
 	setup.py
```

