# Comparing `tmp/piqp-0.2.4.tar.gz` & `tmp/piqp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqp-0.2.4.tar", last modified: Mon Dec 25 18:53:42 2023, max compression
+gzip compressed data, was "piqp-0.3.0.tar", last modified: Fri May 24 14:44:18 2024, max compression
```

## Comparing `piqp-0.2.4.tar` & `piqp-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:53:42.967286 piqp-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-25 18:53:34.000000 piqp-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2023-12-25 18:53:42.967286 piqp-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2023-12-25 18:53:34.000000 piqp-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:53:42.963286 piqp-0.2.4/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:53:42.963286 piqp-0.2.4/interfaces/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:53:42.967286 piqp-0.2.4/interfaces/python/piqp/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-25 18:53:34.000000 piqp-0.2.4/interfaces/python/piqp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 18:53:42.967286 piqp-0.2.4/piqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2023-12-25 18:53:42.000000 piqp-0.2.4/piqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-25 18:53:42.000000 piqp-0.2.4/piqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 18:53:42.000000 piqp-0.2.4/piqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 18:53:42.000000 piqp-0.2.4/piqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 18:53:42.000000 piqp-0.2.4/piqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-25 18:53:42.000000 piqp-0.2.4/piqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-25 18:53:34.000000 piqp-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-25 18:53:42.967286 piqp-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-12-25 18:53:34.000000 piqp-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:44:18.142638 piqp-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-24 14:44:13.000000 piqp-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-24 14:44:18.142638 piqp-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-24 14:44:13.000000 piqp-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:44:18.138638 piqp-0.3.0/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:44:18.138638 piqp-0.3.0/interfaces/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:44:18.142638 piqp-0.3.0/interfaces/python/piqp/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 14:44:13.000000 piqp-0.3.0/interfaces/python/piqp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:44:18.142638 piqp-0.3.0/piqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-24 14:44:18.000000 piqp-0.3.0/piqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 14:44:18.000000 piqp-0.3.0/piqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:44:18.000000 piqp-0.3.0/piqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:44:17.000000 piqp-0.3.0/piqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 14:44:18.000000 piqp-0.3.0/piqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 14:44:18.000000 piqp-0.3.0/piqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-24 14:44:13.000000 piqp-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 14:44:18.142638 piqp-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-24 14:44:13.000000 piqp-0.3.0/setup.py
```

### Comparing `piqp-0.2.4/LICENSE` & `piqp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piqp-0.2.4/PKG-INFO` & `piqp-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.2.4
+Version: 0.3.0
 Summary: A Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: numpy; extra == "test"
 Requires-Dist: scipy; extra == "test"
 
 # PIQP
 
-[![DOI](https://img.shields.io/badge/DOI-10.48550/arXiv.2304.00290-green.svg)](https://doi.org/10.48550/arXiv.2304.00290)
+[![DOI](https://img.shields.io/badge/DOI-10.1109/CDC49753.2023.10383915-green.svg)](https://doi.org/10.1109/CDC49753.2023.10383915)
 [![Preprint](https://img.shields.io/badge/Preprint-arXiv-blue.svg)](https://arxiv.org/abs/2304.00290)
 [![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40__180545)-90e3dc.svg)](https://nccr-automation.ch/)
 
 [![Docs](https://img.shields.io/badge/Docs-available-brightgreen.svg)](https://predict-epfl.github.io/piqp/)
 ![License](https://img.shields.io/badge/License-BSD--2--Clause-brightgreen.svg)
 [![PyPI - downloads](https://img.shields.io/pypi/dm/piqp.svg?label=PyPI%20downloads)](https://pypi.org/project/piqp/)
 [![Conda - downloads](https://img.shields.io/conda/dn/conda-forge/piqp.svg?label=Conda%20downloads)](https://anaconda.org/conda-forge/piqp)
@@ -77,19 +77,23 @@
 * [OSQP](https://github.com/osqp/osqp): The C and Matlab interface is inspired by OSQP.
 * [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs): Parts of the iterative refinement scheme are inspired by Clarabel's implementation.
 
 ## Citing our Work
 
 If you found PIQP useful in your scientific work, we encourage you to cite our accompanying paper:
 ```
-@misc{schwan2023,
-    author = {Schwan, Roland and Jiang, Yuning and Kuhn, Daniel and Jones, Colin N.},
-    title = {PIQP: A Proximal Interior-Point Quadratic Programming Solver},
-    year = {2023},
-    eprint = {arXiv:2304.00290},
+@INPROCEEDINGS{schwan2023piqp,
+  author={Schwan, Roland and Jiang, Yuning and Kuhn, Daniel and Jones, Colin N.},
+  booktitle={2023 62nd IEEE Conference on Decision and Control (CDC)}, 
+  title={{PIQP}: A Proximal Interior-Point Quadratic Programming Solver}, 
+  year={2023},
+  volume={},
+  number={},
+  pages={1088-1093},
+  doi={10.1109/CDC49753.2023.10383915}
 }
 ```
 The benchmarks are available in the following repo: [piqp_benchmarks](https://github.com/PREDICT-EPFL/piqp_benchmarks)
 
 ## License
 
 PIQP is licensed under the BSD 2-Clause License.
```

### Comparing `piqp-0.2.4/README.md` & `piqp-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PIQP
 
-[![DOI](https://img.shields.io/badge/DOI-10.48550/arXiv.2304.00290-green.svg)](https://doi.org/10.48550/arXiv.2304.00290)
+[![DOI](https://img.shields.io/badge/DOI-10.1109/CDC49753.2023.10383915-green.svg)](https://doi.org/10.1109/CDC49753.2023.10383915)
 [![Preprint](https://img.shields.io/badge/Preprint-arXiv-blue.svg)](https://arxiv.org/abs/2304.00290)
 [![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40__180545)-90e3dc.svg)](https://nccr-automation.ch/)
 
 [![Docs](https://img.shields.io/badge/Docs-available-brightgreen.svg)](https://predict-epfl.github.io/piqp/)
 ![License](https://img.shields.io/badge/License-BSD--2--Clause-brightgreen.svg)
 [![PyPI - downloads](https://img.shields.io/pypi/dm/piqp.svg?label=PyPI%20downloads)](https://pypi.org/project/piqp/)
 [![Conda - downloads](https://img.shields.io/conda/dn/conda-forge/piqp.svg?label=Conda%20downloads)](https://anaconda.org/conda-forge/piqp)
@@ -61,19 +61,23 @@
 * [OSQP](https://github.com/osqp/osqp): The C and Matlab interface is inspired by OSQP.
 * [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs): Parts of the iterative refinement scheme are inspired by Clarabel's implementation.
 
 ## Citing our Work
 
 If you found PIQP useful in your scientific work, we encourage you to cite our accompanying paper:
 ```
-@misc{schwan2023,
-    author = {Schwan, Roland and Jiang, Yuning and Kuhn, Daniel and Jones, Colin N.},
-    title = {PIQP: A Proximal Interior-Point Quadratic Programming Solver},
-    year = {2023},
-    eprint = {arXiv:2304.00290},
+@INPROCEEDINGS{schwan2023piqp,
+  author={Schwan, Roland and Jiang, Yuning and Kuhn, Daniel and Jones, Colin N.},
+  booktitle={2023 62nd IEEE Conference on Decision and Control (CDC)}, 
+  title={{PIQP}: A Proximal Interior-Point Quadratic Programming Solver}, 
+  year={2023},
+  volume={},
+  number={},
+  pages={1088-1093},
+  doi={10.1109/CDC49753.2023.10383915}
 }
 ```
 The benchmarks are available in the following repo: [piqp_benchmarks](https://github.com/PREDICT-EPFL/piqp_benchmarks)
 
 ## License
 
 PIQP is licensed under the BSD 2-Clause License.
```

### Comparing `piqp-0.2.4/interfaces/python/piqp/__init__.py` & `piqp-0.3.0/interfaces/python/piqp/__init__.py`

 * *Files identical despite different names*

### Comparing `piqp-0.2.4/piqp.egg-info/PKG-INFO` & `piqp-0.3.0/piqp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.2.4
+Version: 0.3.0
 Summary: A Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: numpy; extra == "test"
 Requires-Dist: scipy; extra == "test"
 
 # PIQP
 
-[![DOI](https://img.shields.io/badge/DOI-10.48550/arXiv.2304.00290-green.svg)](https://doi.org/10.48550/arXiv.2304.00290)
+[![DOI](https://img.shields.io/badge/DOI-10.1109/CDC49753.2023.10383915-green.svg)](https://doi.org/10.1109/CDC49753.2023.10383915)
 [![Preprint](https://img.shields.io/badge/Preprint-arXiv-blue.svg)](https://arxiv.org/abs/2304.00290)
 [![Funding](https://img.shields.io/badge/Grant-NCCR%20Automation%20(51NF40__180545)-90e3dc.svg)](https://nccr-automation.ch/)
 
 [![Docs](https://img.shields.io/badge/Docs-available-brightgreen.svg)](https://predict-epfl.github.io/piqp/)
 ![License](https://img.shields.io/badge/License-BSD--2--Clause-brightgreen.svg)
 [![PyPI - downloads](https://img.shields.io/pypi/dm/piqp.svg?label=PyPI%20downloads)](https://pypi.org/project/piqp/)
 [![Conda - downloads](https://img.shields.io/conda/dn/conda-forge/piqp.svg?label=Conda%20downloads)](https://anaconda.org/conda-forge/piqp)
@@ -77,19 +77,23 @@
 * [OSQP](https://github.com/osqp/osqp): The C and Matlab interface is inspired by OSQP.
 * [Clarabel](https://github.com/oxfordcontrol/Clarabel.rs): Parts of the iterative refinement scheme are inspired by Clarabel's implementation.
 
 ## Citing our Work
 
 If you found PIQP useful in your scientific work, we encourage you to cite our accompanying paper:
 ```
-@misc{schwan2023,
-    author = {Schwan, Roland and Jiang, Yuning and Kuhn, Daniel and Jones, Colin N.},
-    title = {PIQP: A Proximal Interior-Point Quadratic Programming Solver},
-    year = {2023},
-    eprint = {arXiv:2304.00290},
+@INPROCEEDINGS{schwan2023piqp,
+  author={Schwan, Roland and Jiang, Yuning and Kuhn, Daniel and Jones, Colin N.},
+  booktitle={2023 62nd IEEE Conference on Decision and Control (CDC)}, 
+  title={{PIQP}: A Proximal Interior-Point Quadratic Programming Solver}, 
+  year={2023},
+  volume={},
+  number={},
+  pages={1088-1093},
+  doi={10.1109/CDC49753.2023.10383915}
 }
 ```
 The benchmarks are available in the following repo: [piqp_benchmarks](https://github.com/PREDICT-EPFL/piqp_benchmarks)
 
 ## License
 
 PIQP is licensed under the BSD 2-Clause License.
```

### Comparing `piqp-0.2.4/pyproject.toml` & `piqp-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piqp-0.2.4/setup.py` & `piqp-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         cmake_args = [
             f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={extdir}{os.sep}",
             f"-DPYTHON_EXECUTABLE={sys.executable}",
             f"-DCMAKE_BUILD_TYPE={cfg}",  # not used on MSVC, but no harm
             f"-DBUILD_PYTHON_INTERFACE=ON",
             f"-DBUILD_C_INTERFACE=OFF",
             f"-DBUILD_TESTS=OFF",
+            f"-DBUILD_EXAMPLES=OFF",
             f"-DBUILD_BENCHMARKS=OFF",
             f"-DCMAKE_POSITION_INDEPENDENT_CODE:BOOL=true"
         ]
         build_args = []
         # Adding CMake arguments set as environment variable
         # (needed e.g. to build for ARM OSx on conda-forge)
         if "CMAKE_ARGS" in os.environ:
@@ -138,15 +139,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="piqp",
-    version="0.2.4",
+    version="0.3.0",
     url='https://github.com/PREDICT-EPFL/piqp',
     author="Roland Schwan",
     author_email="roland.schwan@epfl.ch",
     license='BSD-2-Clause',
     description="A Proximal Interior Point Quadratic Programming solver",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

