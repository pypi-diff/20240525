# Comparing `tmp/symmetria-0.0.2.tar.gz` & `tmp/symmetria-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symmetria-0.0.2.tar", last modified: Fri May 24 14:11:14 2024, max compression
+gzip compressed data, was "symmetria-0.0.3.tar", last modified: Sat May 25 16:15:15 2024, max compression
```

## Comparing `symmetria-0.0.2.tar` & `symmetria-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:11:14.346781 symmetria-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 14:10:50.000000 symmetria-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-05-24 14:11:14.346781 symmetria-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-24 14:10:50.000000 symmetria-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-24 14:10:50.000000 symmetria-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 14:11:14.346781 symmetria-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:11:14.342781 symmetria-0.0.2/symmetria/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:11:14.342781 symmetria-0.0.2/symmetria/elements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/elements/_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23956 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/elements/cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25289 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/elements/cycle_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    26996 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/elements/permutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:11:14.342781 symmetria-0.0.2/symmetria/groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:10:50.000000 symmetria-0.0.2/symmetria/groups/symmetric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:11:14.342781 symmetria-0.0.2/symmetria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-05-24 14:11:14.000000 symmetria-0.0.2/symmetria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-24 14:11:14.000000 symmetria-0.0.2/symmetria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:11:14.000000 symmetria-0.0.2/symmetria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 14:11:14.000000 symmetria-0.0.2/symmetria.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-24 14:11:14.000000 symmetria-0.0.2/symmetria.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 14:11:14.000000 symmetria-0.0.2/symmetria.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:11:14.342781 symmetria-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-05-24 14:10:50.000000 symmetria-0.0.2/tests/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.400738 symmetria-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 16:15:05.000000 symmetria-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-25 16:15:15.400738 symmetria-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-25 16:15:05.000000 symmetria-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-25 16:15:05.000000 symmetria-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:15:15.400738 symmetria-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27101 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/cycle_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/elements/permutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:05.000000 symmetria-0.0.3/symmetria/groups/symmetric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/symmetria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 16:15:15.000000 symmetria-0.0.3/symmetria.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:15:15.396738 symmetria-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-25 16:15:05.000000 symmetria-0.0.3/tests/test_factory.py
```

### Comparing `symmetria-0.0.2/LICENSE.txt` & `symmetria-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symmetria-0.0.2/PKG-INFO` & `symmetria-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmetria
-Version: 0.0.2
+Version: 0.0.3
 Summary: Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements.
 Author: Vasco Schiavo
 Maintainer: Vasco Schiavo
 Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria
 Project-URL: Documentation, https://symmetria.readthedocs.io/en/latest/
 Keywords: math,mathematics,symmetry,permutation
@@ -43,16 +43,15 @@
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://symmetria.readthedocs.io/en/latest/"><img src="./docs/source/_static/symmetria.png" width="200" align="right" /></a>
 
-**Welcome to symmetria**
-------------------------
+<span style="font-size:1.9em;">**Welcome to symmetria**</span>
 
 Symmetria provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements.
 
 - 📦 - installable via pip
 - 🐍 - compatible with Python **3.9**, **3.10**, **3.11** and **3.12**
 - 👍 - intuitive **API**
@@ -107,15 +106,15 @@
 ```
 
 You can now represent your permutation in various formats:
 
 ```python
 print(permutation)                      # (1, 3, 4, 5, 2, 6)
 print(permutation.cycle_notation())     # (1)(2 3 4 5)(6)
-print(permutation.one_line_notation()   # 134526
+print(permutation.one_line_notation())  # 134526
 ```
 
 Permutations can be compared between them and are easy to manipulate.
 
 ```python
 if permutation:
     print("The permutation is different from the identity.")
@@ -126,22 +125,26 @@
 print(permutation * permutation)
 ```
 
 Furthermore, we can decompose a permutation into its cycle decomposition
 (`CycleDecomposition`) and compute its order and support.
 
 ```python
-permuttation.cycle_decomposition()
+permutation.cycle_decomposition()
 # returns CycleDecomposition(Cycle(1), Cycle(2, 3, 4, 5), Cycle(6))
 permutation.order()  # 4
 permutation.support()  # {2, 3, 4, 5}
 permutation.is_derangement()  # True
 ```
 
 ## Overview
 
-| Overview |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|---|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Open Source** | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| **CI/CD** | ![tests](https://github.com/VascSch92/symmetria/actions/workflows/tests.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/symmetria/badge/?version=latest)](https://symmetria.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                        |
-| **Code** | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/ashtral/ruff)                                                                                                                                                                                                                                                                                                                   |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Statistics**    | ![Static Badge](https://img.shields.io/badge/symmetria-blue?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Issues**        | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                             |
+| **Pull Requests** | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                       |                                           
+| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md)                                                                                                                                                                                                                                                                                                                                                                                       |
+| **DOCS**          | ![Read the Docs](https://img.shields.io/readthedocs/symmetria?logo=readthedocs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                    
+| **CI/CD**         | ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/badge.svg)                                                                                                                                                                                                                                                                                                                                                                |
+| **Code**          | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/astral-sh/ruff)                                                                                                                                                                                                                                                                                                                              |
+| **Downloads**     | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/symmetria) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: symmetria Version: 0.0.2 Summary: Symmetria
+Metadata-Version: 2.1 Name: symmetria Version: 0.0.3 Summary: Symmetria
 provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements. Author: Vasco Schiavo Maintainer:
 Vasco Schiavo Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria Project-URL:
 Documentation, https://symmetria.readthedocs.io/en/latest/ Keywords:
 math,mathematics,symmetry,permutation Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Developers Classifier: Intended
@@ -22,71 +22,86 @@
 "docs" Requires-Dist: nbsphinx>=0.8.6; extra == "docs" Requires-Dist: numpydoc;
 extra == "docs" Requires-Dist: sphinx-rtd-theme; extra == "docs" Requires-Dist:
 sphinx_book_theme; extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra
 == "docs" Requires-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist:
 sphinx-issues<5.0.0; extra == "docs" Requires-Dist: sphinx-gallery<0.17.0;
 extra == "docs" Requires-Dist: sphinx-panels; extra == "docs" Requires-Dist:
 tabulate; extra == "docs" _[_._/_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_s_y_m_m_e_t_r_i_a_._p_n_g_]**Welcome to
-symmetria** ------------------------ Symmetria provides an intuitive, thorough,
-and comprehensive framework for interacting with the symmetric group and its
-elements. - ð¦ - installable via pip - ð - compatible with Python **3.9**,
-**3.10**, **3.11** and **3.12** - ð - intuitive **API** - ð§® - a lot of
-functionalities already implemented - â - 100% of test coverage You can give
-a look at how to work with symmetria in the section [quickstart](#quickstart),
-or you can directly visit the [docs](https://symmetria.readthedocs.io/en/
-latest/). An interesting list of all the functionalities implemented by
-symmetria can be found [here](https://symmetria.readthedocs.io/en/latest/pages/
-API_reference/elements/index.html). Pull requests are welcome. For major
-changes, please open an issue first to discuss what you would like to change,
-and give a look to the [contribution guidelines](https://github.com/VascoSch92/
-symmetria/blob/main/CONTRIBUTING.md). ## Installation Symmetria can be
-comfortably installed from PyPI using the command ```bash pip install symmetria
-``` or directly from the source GitHub code with ```bash pip install git+https:
-//github.com/VascoSch92/symmetria@xxx ``` where `xxx` is the name of the branch
-or the tag you would like to install. You can check that `symmetria` was
-successfully installed by typing the command ```bash symmetria --version ``` ##
-Quickstart Let's get started with symmetria. First and foremost, we can import
-the `Permutation` class from `symmetria`. The Permutation class serves as the
-fundamental class for working with elements of the symmetric group,
-representing permutations as bijective maps. Additionally, you can utilize the
-`Cycle` class and `CycleDecomposition` class to work with cycle permutations
-and permutations represented as cycle decompositions, respectively. ```python
-from symmetria import Permutation permutation = Permutation(1, 3, 4, 5, 2, 6)
-``` You can now represent your permutation in various formats: ```python print
-(permutation) # (1, 3, 4, 5, 2, 6) print(permutation.cycle_notation()) # (1)(2
-3 4 5)(6) print(permutation.one_line_notation() # 134526 ``` Permutations can
-be compared between them and are easy to manipulate. ```python if permutation:
-print("The permutation is different from the identity.") if permutation ==
-Permutation(1, 2, 3, 4, 5, 6): print("The permutation is equal to the
-identity.") if len(permutation) == 6: print("The permutation acts on 6
-elements.") print(permutation * permutation) ``` Furthermore, we can decompose
-a permutation into its cycle decomposition (`CycleDecomposition`) and compute
-its order and support. ```python permuttation.cycle_decomposition() # returns
+symmetria** Symmetria provides an intuitive, thorough, and comprehensive
+framework for interacting with the symmetric group and its elements. - ð¦ -
+installable via pip - ð - compatible with Python **3.9**, **3.10**, **3.11**
+and **3.12** - ð - intuitive **API** - ð§® - a lot of functionalities
+already implemented - â - 100% of test coverage You can give a look at how to
+work with symmetria in the section [quickstart](#quickstart), or you can
+directly visit the [docs](https://symmetria.readthedocs.io/en/latest/). An
+interesting list of all the functionalities implemented by symmetria can be
+found [here](https://symmetria.readthedocs.io/en/latest/pages/API_reference/
+elements/index.html). Pull requests are welcome. For major changes, please open
+an issue first to discuss what you would like to change, and give a look to the
+[contribution guidelines](https://github.com/VascoSch92/symmetria/blob/main/
+CONTRIBUTING.md). ## Installation Symmetria can be comfortably installed from
+PyPI using the command ```bash pip install symmetria ``` or directly from the
+source GitHub code with ```bash pip install git+https://github.com/VascoSch92/
+symmetria@xxx ``` where `xxx` is the name of the branch or the tag you would
+like to install. You can check that `symmetria` was successfully installed by
+typing the command ```bash symmetria --version ``` ## Quickstart Let's get
+started with symmetria. First and foremost, we can import the `Permutation`
+class from `symmetria`. The Permutation class serves as the fundamental class
+for working with elements of the symmetric group, representing permutations as
+bijective maps. Additionally, you can utilize the `Cycle` class and
+`CycleDecomposition` class to work with cycle permutations and permutations
+represented as cycle decompositions, respectively. ```python from symmetria
+import Permutation permutation = Permutation(1, 3, 4, 5, 2, 6) ``` You can now
+represent your permutation in various formats: ```python print(permutation) #
+(1, 3, 4, 5, 2, 6) print(permutation.cycle_notation()) # (1)(2 3 4 5)(6) print
+(permutation.one_line_notation()) # 134526 ``` Permutations can be compared
+between them and are easy to manipulate. ```python if permutation: print("The
+permutation is different from the identity.") if permutation == Permutation(1,
+2, 3, 4, 5, 6): print("The permutation is equal to the identity.") if len
+(permutation) == 6: print("The permutation acts on 6 elements.") print
+(permutation * permutation) ``` Furthermore, we can decompose a permutation
+into its cycle decomposition (`CycleDecomposition`) and compute its order and
+support. ```python permutation.cycle_decomposition() # returns
 CycleDecomposition(Cycle(1), Cycle(2, 3, 4, 5), Cycle(6)) permutation.order() #
 4 permutation.support() # {2, 3, 4, 5} permutation.is_derangement() # True ```
-## Overview | Overview | | |---|-----------------------------------------------
+## Overview | **Statistics** | ![Static Badge](https://img.shields.io/badge/
+symmetria-blue?style=for-the-badge) | |-------------------|--------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------| | **Open Source** | [![MIT](https://img.shields.io/badge/License-
-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) | |
-**CI/CD** | ![tests](https://github.com/VascSch92/symmetria/actions/workflows/
-tests.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/
-symmetria/badge/?version=latest)](https://symmetria.readthedocs.io/en/latest/
-?badge=latest) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
+--------------------------------------------------| | **Repository** | ![GitHub
+Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria) ![GitHub
+forks](https://img.shields.io/github/forks/VascoSch92/symmetria) | | **Issues**
+| ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/
+VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull
+Requests](https://img.shields.io/github/issues-closed/VascoSch92/
+symmetria?logo=GitHub&color=green) | | **Pull Requests** | ![GitHub Issues or
+Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/
+symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
+img.shields.io/github/issues-pr-closed/VascoSch92/
+symmetria?logo=GitHub&color=green) | | **Open Source** | [![MIT](https://
+img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/
+symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-
+ð-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/
+CONTRIBUTING.md) | | **DOCS** | ![Read the Docs](https://img.shields.io/
+readthedocs/symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://
+github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests]
+(https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/
+badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/
+release.yml/badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
 symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-
 versions](https://img.shields.io/pypi/pyversions/symmetria)](https://
 www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-
-8A2BE2.svg)](https://github.com/ashtral/ruff) | | **Downloads** | [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+8A2BE2.svg)](https://github.com/astral-sh/ruff) | | **Downloads** | [!
+[Downloads](https://static.pepy.tech/personalized-badge/
 symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
+(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
+(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
-(pypi))](https://pepy.tech/project/skpro) |
+(pypi))](https://pepy.tech/project/symmetria) |
```

### Comparing `symmetria-0.0.2/README.md` & `symmetria-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 <a href="https://symmetria.readthedocs.io/en/latest/"><img src="./docs/source/_static/symmetria.png" width="200" align="right" /></a>
 
-**Welcome to symmetria**
-------------------------
+<span style="font-size:1.9em;">**Welcome to symmetria**</span>
 
 Symmetria provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements.
 
 - 📦 - installable via pip
 - 🐍 - compatible with Python **3.9**, **3.10**, **3.11** and **3.12**
 - 👍 - intuitive **API**
@@ -60,15 +59,15 @@
 ```
 
 You can now represent your permutation in various formats:
 
 ```python
 print(permutation)                      # (1, 3, 4, 5, 2, 6)
 print(permutation.cycle_notation())     # (1)(2 3 4 5)(6)
-print(permutation.one_line_notation()   # 134526
+print(permutation.one_line_notation())  # 134526
 ```
 
 Permutations can be compared between them and are easy to manipulate.
 
 ```python
 if permutation:
     print("The permutation is different from the identity.")
@@ -79,22 +78,26 @@
 print(permutation * permutation)
 ```
 
 Furthermore, we can decompose a permutation into its cycle decomposition
 (`CycleDecomposition`) and compute its order and support.
 
 ```python
-permuttation.cycle_decomposition()
+permutation.cycle_decomposition()
 # returns CycleDecomposition(Cycle(1), Cycle(2, 3, 4, 5), Cycle(6))
 permutation.order()  # 4
 permutation.support()  # {2, 3, 4, 5}
 permutation.is_derangement()  # True
 ```
 
 ## Overview
 
-| Overview |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|---|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Open Source** | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| **CI/CD** | ![tests](https://github.com/VascSch92/symmetria/actions/workflows/tests.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/symmetria/badge/?version=latest)](https://symmetria.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                        |
-| **Code** | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/ashtral/ruff)                                                                                                                                                                                                                                                                                                                   |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Statistics**    | ![Static Badge](https://img.shields.io/badge/symmetria-blue?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Issues**        | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                             |
+| **Pull Requests** | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                       |                                           
+| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md)                                                                                                                                                                                                                                                                                                                                                                                       |
+| **DOCS**          | ![Read the Docs](https://img.shields.io/readthedocs/symmetria?logo=readthedocs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                    
+| **CI/CD**         | ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/badge.svg)                                                                                                                                                                                                                                                                                                                                                                |
+| **Code**          | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/astral-sh/ruff)                                                                                                                                                                                                                                                                                                                              |
+| **Downloads**     | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/symmetria) |
```

#### html2text {}

```diff
@@ -1,65 +1,80 @@
-_[_._/_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_s_y_m_m_e_t_r_i_a_._p_n_g_]**Welcome to symmetria** -----------------
-------- Symmetria provides an intuitive, thorough, and comprehensive framework
-for interacting with the symmetric group and its elements. - ð¦ - installable
-via pip - ð - compatible with Python **3.9**, **3.10**, **3.11** and
-**3.12** - ð - intuitive **API** - ð§® - a lot of functionalities already
-implemented - â - 100% of test coverage You can give a look at how to work
-with symmetria in the section [quickstart](#quickstart), or you can directly
-visit the [docs](https://symmetria.readthedocs.io/en/latest/). An interesting
-list of all the functionalities implemented by symmetria can be found [here]
-(https://symmetria.readthedocs.io/en/latest/pages/API_reference/elements/
-index.html). Pull requests are welcome. For major changes, please open an issue
-first to discuss what you would like to change, and give a look to the
-[contribution guidelines](https://github.com/VascoSch92/symmetria/blob/main/
-CONTRIBUTING.md). ## Installation Symmetria can be comfortably installed from
-PyPI using the command ```bash pip install symmetria ``` or directly from the
-source GitHub code with ```bash pip install git+https://github.com/VascoSch92/
-symmetria@xxx ``` where `xxx` is the name of the branch or the tag you would
-like to install. You can check that `symmetria` was successfully installed by
-typing the command ```bash symmetria --version ``` ## Quickstart Let's get
-started with symmetria. First and foremost, we can import the `Permutation`
-class from `symmetria`. The Permutation class serves as the fundamental class
-for working with elements of the symmetric group, representing permutations as
-bijective maps. Additionally, you can utilize the `Cycle` class and
-`CycleDecomposition` class to work with cycle permutations and permutations
-represented as cycle decompositions, respectively. ```python from symmetria
-import Permutation permutation = Permutation(1, 3, 4, 5, 2, 6) ``` You can now
-represent your permutation in various formats: ```python print(permutation) #
-(1, 3, 4, 5, 2, 6) print(permutation.cycle_notation()) # (1)(2 3 4 5)(6) print
-(permutation.one_line_notation() # 134526 ``` Permutations can be compared
+_[_._/_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_s_y_m_m_e_t_r_i_a_._p_n_g_]**Welcome to symmetria** Symmetria
+provides an intuitive, thorough, and comprehensive framework for interacting
+with the symmetric group and its elements. - ð¦ - installable via pip - ð
+- compatible with Python **3.9**, **3.10**, **3.11** and **3.12** - ð -
+intuitive **API** - ð§® - a lot of functionalities already implemented - â -
+100% of test coverage You can give a look at how to work with symmetria in the
+section [quickstart](#quickstart), or you can directly visit the [docs](https:/
+/symmetria.readthedocs.io/en/latest/). An interesting list of all the
+functionalities implemented by symmetria can be found [here](https://
+symmetria.readthedocs.io/en/latest/pages/API_reference/elements/index.html).
+Pull requests are welcome. For major changes, please open an issue first to
+discuss what you would like to change, and give a look to the [contribution
+guidelines](https://github.com/VascoSch92/symmetria/blob/main/CONTRIBUTING.md).
+## Installation Symmetria can be comfortably installed from PyPI using the
+command ```bash pip install symmetria ``` or directly from the source GitHub
+code with ```bash pip install git+https://github.com/VascoSch92/symmetria@xxx
+``` where `xxx` is the name of the branch or the tag you would like to install.
+You can check that `symmetria` was successfully installed by typing the command
+```bash symmetria --version ``` ## Quickstart Let's get started with symmetria.
+First and foremost, we can import the `Permutation` class from `symmetria`. The
+Permutation class serves as the fundamental class for working with elements of
+the symmetric group, representing permutations as bijective maps. Additionally,
+you can utilize the `Cycle` class and `CycleDecomposition` class to work with
+cycle permutations and permutations represented as cycle decompositions,
+respectively. ```python from symmetria import Permutation permutation =
+Permutation(1, 3, 4, 5, 2, 6) ``` You can now represent your permutation in
+various formats: ```python print(permutation) # (1, 3, 4, 5, 2, 6) print
+(permutation.cycle_notation()) # (1)(2 3 4 5)(6) print
+(permutation.one_line_notation()) # 134526 ``` Permutations can be compared
 between them and are easy to manipulate. ```python if permutation: print("The
 permutation is different from the identity.") if permutation == Permutation(1,
 2, 3, 4, 5, 6): print("The permutation is equal to the identity.") if len
 (permutation) == 6: print("The permutation acts on 6 elements.") print
 (permutation * permutation) ``` Furthermore, we can decompose a permutation
 into its cycle decomposition (`CycleDecomposition`) and compute its order and
-support. ```python permuttation.cycle_decomposition() # returns
+support. ```python permutation.cycle_decomposition() # returns
 CycleDecomposition(Cycle(1), Cycle(2, 3, 4, 5), Cycle(6)) permutation.order() #
 4 permutation.support() # {2, 3, 4, 5} permutation.is_derangement() # True ```
-## Overview | Overview | | |---|-----------------------------------------------
+## Overview | **Statistics** | ![Static Badge](https://img.shields.io/badge/
+symmetria-blue?style=for-the-badge) | |-------------------|--------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------| | **Open Source** | [![MIT](https://img.shields.io/badge/License-
-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) | |
-**CI/CD** | ![tests](https://github.com/VascSch92/symmetria/actions/workflows/
-tests.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/
-symmetria/badge/?version=latest)](https://symmetria.readthedocs.io/en/latest/
-?badge=latest) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
+--------------------------------------------------| | **Repository** | ![GitHub
+Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria) ![GitHub
+forks](https://img.shields.io/github/forks/VascoSch92/symmetria) | | **Issues**
+| ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/
+VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull
+Requests](https://img.shields.io/github/issues-closed/VascoSch92/
+symmetria?logo=GitHub&color=green) | | **Pull Requests** | ![GitHub Issues or
+Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/
+symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
+img.shields.io/github/issues-pr-closed/VascoSch92/
+symmetria?logo=GitHub&color=green) | | **Open Source** | [![MIT](https://
+img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/
+symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-
+ð-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/
+CONTRIBUTING.md) | | **DOCS** | ![Read the Docs](https://img.shields.io/
+readthedocs/symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://
+github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests]
+(https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/
+badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/
+release.yml/badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
 symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-
 versions](https://img.shields.io/pypi/pyversions/symmetria)](https://
 www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-
-8A2BE2.svg)](https://github.com/ashtral/ruff) | | **Downloads** | [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+8A2BE2.svg)](https://github.com/astral-sh/ruff) | | **Downloads** | [!
+[Downloads](https://static.pepy.tech/personalized-badge/
 symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
+(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
+(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
-(pypi))](https://pepy.tech/project/skpro) |
+(pypi))](https://pepy.tech/project/symmetria) |
```

### Comparing `symmetria-0.0.2/pyproject.toml` & `symmetria-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "symmetria"
-version = "0.0.2"
+version = "0.0.3"
 description = "Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements."
 authors = [
     {name = "Vasco Schiavo"},
 ]
 maintainers = [
     {name = "Vasco Schiavo"},
 ]
```

### Comparing `symmetria-0.0.2/symmetria/__init__.py` & `symmetria-0.0.3/symmetria/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from symmetria.elements.cycle import Cycle
 from symmetria.elements.permutation import Permutation
 from symmetria.elements.cycle_decomposition import CycleDecomposition
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __all__ = ["__version__", "Permutation", "Cycle", "CycleDecomposition"]
 
 
 def _log_version() -> None:
     """Private method which take a command line argument and log the version of `symmetria`."""
     if len(sys.argv) == 0 or len(sys.argv) == 1:
         raise Exception("No command provided.")
```

### Comparing `symmetria-0.0.2/symmetria/elements/_interface.py` & `symmetria-0.0.3/symmetria/elements/_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,18 @@
 
     @abstractmethod
     def inverse(self) -> "_Element":
         """Return the inverse of the permutation object."""
         raise NotImplementedError
 
     @abstractmethod
+    def is_conjugate(self, other: "_Element") -> bool:
+        """Return True if self and other are conjugate."""
+
+    @abstractmethod
     def is_derangement(self) -> bool:
         """Return if the element is a derangement or not."""
         raise NotImplementedError
 
     @abstractmethod
     def is_even(self) -> bool:
         """Return if the element is even or not."""
```

### Comparing `symmetria-0.0.2/symmetria/elements/cycle.py` & `symmetria-0.0.3/symmetria/elements/cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 import symmetria.elements.cycle_decomposition
 from symmetria.elements._interface import _Element
 
 __all__ = ["Cycle"]
 
 
 class Cycle(_Element):
-    r"""The ``Cycle`` class represents the cycles element of a symmetric group.
+    r"""The ``Cycle`` class represents the cycle elements of a symmetric group.
 
     Recall that a cycle is a permutation that rearranges the elements of a finite set in a circular fashion, i.e.,
     moves each element to the position of the next element in a cycle manner, with the last element being moved to the
     position of the first element.
 
     To define a cycle, you need to provide its cycle notation.
 
-    For example, to define the cycle :math:`\sigma \in S_3` given by :math:`\sigma(1)=3, \sigma(2)=1`, and
-    :math:`\sigma (3)=2`, you should write ``Cycle(1, 3, 2)``.
+    For example, to define the cycle :math:`\sigma \in S_3` given by :math:`\sigma(1)=3`, :math:`\sigma(2)=1` and
+    :math:`\sigma(3)=2`, you should write ``Cycle(1, 3, 2)``
 
     .. note:: A cycle can have different representations. For example, the cycle ``Cycle(1, 3, 2)`` can be also
-        written ``Cycle(2, 1, 3)``. By convention here, a cycle start always with the smaller number.
+        written ``Cycle(2, 1, 3)``.
+
+        By convention, a cycle start always with the smaller number. Don't panic, you can define a
+        cycle in the way you like the most, but then it will be stored following the above convention.
 
     :param cycle: Set of integers representing the cycle notation of the cycle.
     :type cycle: int
 
     :raises ValueError: If there is an integer in the provided cycle which is not strictly positive.
 
     :example:
@@ -450,14 +453,24 @@
             >>> Cycle(1, 3, 4, 2).inverse()
             Cycle(1, 2, 4, 3)
             >>> Cycle(2, 3, 1, 5, 4).inverse()
             Cycle(1, 3, 2, 4, 5)
         """
         return Cycle(*self.elements[::-1])
 
+    def is_conjugate(self, other: "Cycle") -> bool:
+        """
+        :raise NotImplementedError: The method `is_conjugate` is not implemented for cycles.
+            This is because cycles are just building blocks for permutations.
+        """
+        raise NotImplementedError(
+            "Method `is_conjugate` is not implemented for cycles. \n"
+            "Convert the cycle into a `Permutation` or a `CycleDecomposition`."
+        )
+
     def is_derangement(self) -> bool:
         r"""Check if the cycle is a derangement.
 
         Recall that a permutation :math:`\sigma` is called a derangement if it has no fixed points, i.e.,
         :math:`\sigma(x) \neq x` for every :math:`x` in the permutation domain.
 
         By definition, a cycle is a derangement if and only if it is not the identity cycle.
```

### Comparing `symmetria-0.0.2/symmetria/elements/cycle_decomposition.py` & `symmetria-0.0.3/symmetria/elements/cycle_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,21 @@
     number of cycles thanks to the `Cycle Decomposition Theorem for Permutations`.
 
     To define a permutation as a cycle decomposition, you need to provide its cycles.
 
     For example, to define the permutation given by the cycles: ``Cycle(2, 1)`` and ``Cycle(4, 3)``, you should write
     ``CycleDecomposition(Cycle(2, 1), Cycle(4, 3))``.
 
+    .. note::
+        By convention, a cycle decomposition starts always with the
+        smaller cycle, i.e., the cycle with the smallest element, and is increasing.
+
+        This is because a cycle decomposition can have different representations. Don't panic, you can write the
+        cycle decomposition in the way you like the most, but then it will be stored following the above convention.
+
     :param cycle: Cycle factors of the permutation.
     :type cycle: Cycle
 
     :raises ValueError: If there are two or more cycles with non-disjoint support.
     :raises ValueError: If there are missing cycles in the decomposition.
 
     :example:
@@ -443,14 +450,45 @@
             >>> CycleDecomposition(Cycle(1, 2, 3)).inverse()
             CycleDecomposition(Cycle(1, 3, 2))
             >>> CycleDecomposition(Cycle(1, 2), Cycle(3, 4)).inverse()
             CycleDecomposition(Cycle(1, 2), Cycle(3, 4))
         """
         return CycleDecomposition(*[cycle.inverse() for cycle in self])
 
+    def is_conjugate(self, other: "CycleDecomposition") -> bool:
+        r"""Check if two cycle decompositions are conjugated.
+
+        Recall that two permutations :math:`\sigma, \quad \tau \in S_n`, for some :math:`n \in \mathbb{N}`, are said to
+        be conjugated if there is :math:`\gamma \in S_n` such that :math:`\gamma\sigma\gamma^{-1} = \tau`.
+
+        :param other: a cycle decomposition
+        :type other: CycleDecomposition
+
+        :return: True if self and other are conjugated, False otherwise.
+        :rtype: bool
+
+        :example:
+            >>> from symmetria import Cycle, CycleDecomposition
+            ...
+            >>> cycle_dec = CycleDecomposition(Cycle(1, 2, 3))
+            >>> cycle_dec.is_conjugate(cycle_dec)
+            True
+            >>> cycle_dec_a = CycleDecomposition(Cycle(1, 3, 2, 5, 4))
+            >>> cycle_dec_b = CycleDecomposition(Cycle(1, 4, 3, 5, 2))
+            >>> cycle_dec_a.is_conjugate(cycle_dec_b)
+            True
+            >>> cycle_dec_a = CycleDecomposition(Cycle(1, 2), Cycle(3, 4))
+            >>> cycle_dec_b = CycleDecomposition(Cycle(1), Cycle(3, 2, 4))
+            >>> cycle_dec_a.is_conjugate(cycle_dec_b)
+            False
+        """
+        if isinstance(other, CycleDecomposition) is False:
+            raise TypeError(f"Method `is_conjugate` not implemented for type {type}.")
+        return self.cycle_type() == other.cycle_type()
+
     def is_derangement(self) -> bool:
         r"""Check if the cycle decomposition is a derangement.
 
         Recall that a permutation :math:`\sigma` is called a derangement if it has no fixed points, i.e.,
         :math:`\sigma(x) \neq x` for every :math:`x` in the permutation domain.
 
         :return: True if the permutation is a derangement, False otherwise.
```

### Comparing `symmetria-0.0.2/symmetria/elements/permutation.py` & `symmetria-0.0.3/symmetria/elements/permutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,15 +398,16 @@
         :example:
             >>> from symmetria import Cycle, CycleDecomposition, Permutation
             ...
             >>> Permutation(1, 2, 3).equivalent(Permutation(1, 2, 3))
             True
             >>> Permutation(3, 1, 2).equivalent(Cycle(1, 3, 2))
             True
-            >>> Permutation(2, 1, 4, 3).equivalent(CycleDecomposition(Cycle(1, 2), Cycle(3, 4)))
+            >>> cycle_decomp = CycleDecomposition(Cycle(1, 2), Cycle(3, 4))
+            >>> Permutation(2, 1, 4, 3).equivalent(cycle_decomp)
             True
         """
         if isinstance(other, Permutation):
             return self == other
         elif isinstance(other, symmetria.elements.cycle.Cycle):
             return self == Permutation.from_cycle(other)
         elif isinstance(other, symmetria.elements.cycle_decomposition.CycleDecomposition):
@@ -504,14 +505,42 @@
             >>> Permutation(1, 3, 4, 2).inverse()
             Permutation(1, 4, 2, 3)
             >>> Permutation(2, 3, 1, 5, 4).inverse()
             Permutation(3, 1, 2, 5, 4)
         """
         return Permutation.from_dict({item: key for key, item in self.map.items()})
 
+    def is_conjugate(self, other: "Permutation") -> bool:
+        r"""Check if two permutations are conjugated.
+
+        Recall that two permutations :math:`\sigma, \quad \tau \in S_n`, for some :math:`n \in \mathbb{N}`, are said to
+        be conjugated if there is :math:`\gamma \in S_n` such that :math:`\gamma\sigma\gamma^{-1} = \tau`.
+
+        :param other: a permutation
+        :type other: Permutation
+
+        :return: True if self and other are conjugated, False otherwise.
+        :rtype: bool
+
+        :example:
+            >>> from symmetria import Permutation
+            ...
+            >>> Permutation(1, 2, 3).is_conjugate(Permutation(1, 2, 3))
+            True
+            >>> Permutation(1, 2, 3).is_conjugate(Permutation(3, 2, 1))
+            False
+            >>> permutation_a = Permutation(3, 2, 5, 4, 1)
+            >>> permutation_b = Permutation(5, 2, 1, 4, 3)
+            >>> permutation_a.is_conjugate(permutation_b)
+            True
+        """
+        if isinstance(other, Permutation) is False:
+            raise TypeError(f"Method `is_conjugate` not implemented for type {type}.")
+        return self.cycle_type() == other.cycle_type()
+
     def is_derangement(self) -> bool:
         r"""Check if the permutation is a derangement.
 
         Recall that a permutation :math:`\sigma` is called a derangement if it has no fixed points, i.e.,
         :math:`\sigma(x) \neq x` for every :math:`x` in the permutation domain.
 
         :return: True if the permutation is a derangement, False otherwise.
```

### Comparing `symmetria-0.0.2/symmetria.egg-info/PKG-INFO` & `symmetria-0.0.3/symmetria.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symmetria
-Version: 0.0.2
+Version: 0.0.3
 Summary: Symmetria provides an intuitive, thorough, and comprehensive framework for interacting with the symmetric group and its elements.
 Author: Vasco Schiavo
 Maintainer: Vasco Schiavo
 Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria
 Project-URL: Documentation, https://symmetria.readthedocs.io/en/latest/
 Keywords: math,mathematics,symmetry,permutation
@@ -43,16 +43,15 @@
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://symmetria.readthedocs.io/en/latest/"><img src="./docs/source/_static/symmetria.png" width="200" align="right" /></a>
 
-**Welcome to symmetria**
-------------------------
+<span style="font-size:1.9em;">**Welcome to symmetria**</span>
 
 Symmetria provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements.
 
 - 📦 - installable via pip
 - 🐍 - compatible with Python **3.9**, **3.10**, **3.11** and **3.12**
 - 👍 - intuitive **API**
@@ -107,15 +106,15 @@
 ```
 
 You can now represent your permutation in various formats:
 
 ```python
 print(permutation)                      # (1, 3, 4, 5, 2, 6)
 print(permutation.cycle_notation())     # (1)(2 3 4 5)(6)
-print(permutation.one_line_notation()   # 134526
+print(permutation.one_line_notation())  # 134526
 ```
 
 Permutations can be compared between them and are easy to manipulate.
 
 ```python
 if permutation:
     print("The permutation is different from the identity.")
@@ -126,22 +125,26 @@
 print(permutation * permutation)
 ```
 
 Furthermore, we can decompose a permutation into its cycle decomposition
 (`CycleDecomposition`) and compute its order and support.
 
 ```python
-permuttation.cycle_decomposition()
+permutation.cycle_decomposition()
 # returns CycleDecomposition(Cycle(1), Cycle(2, 3, 4, 5), Cycle(6))
 permutation.order()  # 4
 permutation.support()  # {2, 3, 4, 5}
 permutation.is_derangement()  # True
 ```
 
 ## Overview
 
-| Overview |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|---|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Open Source** | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| **CI/CD** | ![tests](https://github.com/VascSch92/symmetria/actions/workflows/tests.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/symmetria/badge/?version=latest)](https://symmetria.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                        |
-| **Code** | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/ashtral/ruff)                                                                                                                                                                                                                                                                                                                   |
-| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Statistics**    | ![Static Badge](https://img.shields.io/badge/symmetria-blue?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Repository**    | ![GitHub Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria)  ![GitHub forks](https://img.shields.io/github/forks/VascoSch92/symmetria)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Issues**        | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                             |
+| **Pull Requests** | ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr-closed/VascoSch92/symmetria?logo=GitHub&color=green)                                                                                                                                                                                                                                                                                                                                                                                       |                                           
+| **Open Source**   | [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-😃-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/CONTRIBUTING.md)                                                                                                                                                                                                                                                                                                                                                                                       |
+| **DOCS**          | ![Read the Docs](https://img.shields.io/readthedocs/symmetria?logo=readthedocs)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |                                                                                                                                                    
+| **CI/CD**         | ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/release.yml/badge.svg)                                                                                                                                                                                                                                                                                                                                                                |
+| **Code**          | [![!pypi](https://img.shields.io/pypi/v/symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-versions](https://img.shields.io/pypi/pyversions/symmetria)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-8A2BE2.svg)](https://github.com/astral-sh/ruff)                                                                                                                                                                                                                                                                                                                              |
+| **Downloads**     | [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://static.pepy.tech/personalized-badge/symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/symmetria) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: symmetria Version: 0.0.2 Summary: Symmetria
+Metadata-Version: 2.1 Name: symmetria Version: 0.0.3 Summary: Symmetria
 provides an intuitive, thorough, and comprehensive framework for interacting
 with the symmetric group and its elements. Author: Vasco Schiavo Maintainer:
 Vasco Schiavo Project-URL: Homepage, https://github.com/VascoSch92/symmetria
 Project-URL: Repository, https://github.com/VascoSch92/symmetria Project-URL:
 Documentation, https://symmetria.readthedocs.io/en/latest/ Keywords:
 math,mathematics,symmetry,permutation Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Developers Classifier: Intended
@@ -22,71 +22,86 @@
 "docs" Requires-Dist: nbsphinx>=0.8.6; extra == "docs" Requires-Dist: numpydoc;
 extra == "docs" Requires-Dist: sphinx-rtd-theme; extra == "docs" Requires-Dist:
 sphinx_book_theme; extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra
 == "docs" Requires-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist:
 sphinx-issues<5.0.0; extra == "docs" Requires-Dist: sphinx-gallery<0.17.0;
 extra == "docs" Requires-Dist: sphinx-panels; extra == "docs" Requires-Dist:
 tabulate; extra == "docs" _[_._/_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_s_y_m_m_e_t_r_i_a_._p_n_g_]**Welcome to
-symmetria** ------------------------ Symmetria provides an intuitive, thorough,
-and comprehensive framework for interacting with the symmetric group and its
-elements. - ð¦ - installable via pip - ð - compatible with Python **3.9**,
-**3.10**, **3.11** and **3.12** - ð - intuitive **API** - ð§® - a lot of
-functionalities already implemented - â - 100% of test coverage You can give
-a look at how to work with symmetria in the section [quickstart](#quickstart),
-or you can directly visit the [docs](https://symmetria.readthedocs.io/en/
-latest/). An interesting list of all the functionalities implemented by
-symmetria can be found [here](https://symmetria.readthedocs.io/en/latest/pages/
-API_reference/elements/index.html). Pull requests are welcome. For major
-changes, please open an issue first to discuss what you would like to change,
-and give a look to the [contribution guidelines](https://github.com/VascoSch92/
-symmetria/blob/main/CONTRIBUTING.md). ## Installation Symmetria can be
-comfortably installed from PyPI using the command ```bash pip install symmetria
-``` or directly from the source GitHub code with ```bash pip install git+https:
-//github.com/VascoSch92/symmetria@xxx ``` where `xxx` is the name of the branch
-or the tag you would like to install. You can check that `symmetria` was
-successfully installed by typing the command ```bash symmetria --version ``` ##
-Quickstart Let's get started with symmetria. First and foremost, we can import
-the `Permutation` class from `symmetria`. The Permutation class serves as the
-fundamental class for working with elements of the symmetric group,
-representing permutations as bijective maps. Additionally, you can utilize the
-`Cycle` class and `CycleDecomposition` class to work with cycle permutations
-and permutations represented as cycle decompositions, respectively. ```python
-from symmetria import Permutation permutation = Permutation(1, 3, 4, 5, 2, 6)
-``` You can now represent your permutation in various formats: ```python print
-(permutation) # (1, 3, 4, 5, 2, 6) print(permutation.cycle_notation()) # (1)(2
-3 4 5)(6) print(permutation.one_line_notation() # 134526 ``` Permutations can
-be compared between them and are easy to manipulate. ```python if permutation:
-print("The permutation is different from the identity.") if permutation ==
-Permutation(1, 2, 3, 4, 5, 6): print("The permutation is equal to the
-identity.") if len(permutation) == 6: print("The permutation acts on 6
-elements.") print(permutation * permutation) ``` Furthermore, we can decompose
-a permutation into its cycle decomposition (`CycleDecomposition`) and compute
-its order and support. ```python permuttation.cycle_decomposition() # returns
+symmetria** Symmetria provides an intuitive, thorough, and comprehensive
+framework for interacting with the symmetric group and its elements. - ð¦ -
+installable via pip - ð - compatible with Python **3.9**, **3.10**, **3.11**
+and **3.12** - ð - intuitive **API** - ð§® - a lot of functionalities
+already implemented - â - 100% of test coverage You can give a look at how to
+work with symmetria in the section [quickstart](#quickstart), or you can
+directly visit the [docs](https://symmetria.readthedocs.io/en/latest/). An
+interesting list of all the functionalities implemented by symmetria can be
+found [here](https://symmetria.readthedocs.io/en/latest/pages/API_reference/
+elements/index.html). Pull requests are welcome. For major changes, please open
+an issue first to discuss what you would like to change, and give a look to the
+[contribution guidelines](https://github.com/VascoSch92/symmetria/blob/main/
+CONTRIBUTING.md). ## Installation Symmetria can be comfortably installed from
+PyPI using the command ```bash pip install symmetria ``` or directly from the
+source GitHub code with ```bash pip install git+https://github.com/VascoSch92/
+symmetria@xxx ``` where `xxx` is the name of the branch or the tag you would
+like to install. You can check that `symmetria` was successfully installed by
+typing the command ```bash symmetria --version ``` ## Quickstart Let's get
+started with symmetria. First and foremost, we can import the `Permutation`
+class from `symmetria`. The Permutation class serves as the fundamental class
+for working with elements of the symmetric group, representing permutations as
+bijective maps. Additionally, you can utilize the `Cycle` class and
+`CycleDecomposition` class to work with cycle permutations and permutations
+represented as cycle decompositions, respectively. ```python from symmetria
+import Permutation permutation = Permutation(1, 3, 4, 5, 2, 6) ``` You can now
+represent your permutation in various formats: ```python print(permutation) #
+(1, 3, 4, 5, 2, 6) print(permutation.cycle_notation()) # (1)(2 3 4 5)(6) print
+(permutation.one_line_notation()) # 134526 ``` Permutations can be compared
+between them and are easy to manipulate. ```python if permutation: print("The
+permutation is different from the identity.") if permutation == Permutation(1,
+2, 3, 4, 5, 6): print("The permutation is equal to the identity.") if len
+(permutation) == 6: print("The permutation acts on 6 elements.") print
+(permutation * permutation) ``` Furthermore, we can decompose a permutation
+into its cycle decomposition (`CycleDecomposition`) and compute its order and
+support. ```python permutation.cycle_decomposition() # returns
 CycleDecomposition(Cycle(1), Cycle(2, 3, 4, 5), Cycle(6)) permutation.order() #
 4 permutation.support() # {2, 3, 4, 5} permutation.is_derangement() # True ```
-## Overview | Overview | | |---|-----------------------------------------------
+## Overview | **Statistics** | ![Static Badge](https://img.shields.io/badge/
+symmetria-blue?style=for-the-badge) | |-------------------|--------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------| | **Open Source** | [![MIT](https://img.shields.io/badge/License-
-MIT-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/LICENSE) | |
-**CI/CD** | ![tests](https://github.com/VascSch92/symmetria/actions/workflows/
-tests.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/
-symmetria/badge/?version=latest)](https://symmetria.readthedocs.io/en/latest/
-?badge=latest) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
+--------------------------------------------------| | **Repository** | ![GitHub
+Repo stars](https://img.shields.io/github/stars/VascoSch92/symmetria) ![GitHub
+forks](https://img.shields.io/github/forks/VascoSch92/symmetria) | | **Issues**
+| ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/
+VascoSch92/symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull
+Requests](https://img.shields.io/github/issues-closed/VascoSch92/
+symmetria?logo=GitHub&color=green) | | **Pull Requests** | ![GitHub Issues or
+Pull Requests](https://img.shields.io/github/issues-pr/VascoSch92/
+symmetria?logo=GitHub&color=yellow) ![GitHub Issues or Pull Requests](https://
+img.shields.io/github/issues-pr-closed/VascoSch92/
+symmetria?logo=GitHub&color=green) | | **Open Source** | [![MIT](https://
+img.shields.io/badge/License-MIT-blue.svg)](https://github.com/VascSch92/
+symmetria/blob/main/LICENSE) [![MIT](https://img.shields.io/badge/Contributing-
+ð-blue.svg)](https://github.com/VascSch92/symmetria/blob/main/
+CONTRIBUTING.md) | | **DOCS** | ![Read the Docs](https://img.shields.io/
+readthedocs/symmetria?logo=readthedocs) | | **CI/CD** | ![tests](https://
+github.com/VascoSch92/symmetria/actions/workflows/tests.yml/badge.svg) ![tests]
+(https://github.com/VascoSch92/symmetria/actions/workflows/code-style.yml/
+badge.svg) ![tests](https://github.com/VascoSch92/symmetria/actions/workflows/
+release.yml/badge.svg) | | **Code** | [![!pypi](https://img.shields.io/pypi/v/
 symmetria?color=orange)](https://pypi.org/project/symmetria/) [![!python-
 versions](https://img.shields.io/pypi/pyversions/symmetria)](https://
 www.python.org/) [![!black](https://img.shields.io/badge/code%20style-ruff-
-8A2BE2.svg)](https://github.com/ashtral/ruff) | | **Downloads** | [![Downloads]
-(https://static.pepy.tech/personalized-badge/
+8A2BE2.svg)](https://github.com/astral-sh/ruff) | | **Downloads** | [!
+[Downloads](https://static.pepy.tech/personalized-badge/
 symmetria?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
+(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 symmetria?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
-(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
+(pypi))](https://pepy.tech/project/symmetria) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 symmetria?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
-(pypi))](https://pepy.tech/project/skpro) |
+(pypi))](https://pepy.tech/project/symmetria) |
```

### Comparing `symmetria-0.0.2/tests/test_factory.py` & `symmetria-0.0.3/tests/test_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,22 @@
 def validate_inverse(item: Any, expected_value: Any) -> None:
     if item.inverse() != expected_value:
         raise ValueError(
             f"The expression `{item.rep()}.inverse()` must evaluate {expected_value}, but got {item.inverse()}."
         )
 
 
+def validate_is_conjugate(item: Any, other: Any, expected_value: bool) -> None:
+    if item.is_conjugate(other) is not expected_value:
+        raise ValueError(
+            f"The expression `{item.rep()}.is_conjugate({other.rep()})` must evaluate {expected_value}, "
+            f"but got {item.is_conjugate(other)}."
+        )
+
+
 def validate_is_derangement(item: Any, expected_value: bool) -> None:
     if item.is_derangement() is not expected_value:
         raise ValueError(
             f"The expression `{item.rep()}.is_derangement()` must evaluate {expected_value}, "
             f"but got {item.is_derangement()}."
         )
```

