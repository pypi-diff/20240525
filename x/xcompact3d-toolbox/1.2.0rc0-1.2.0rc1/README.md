# Comparing `tmp/xcompact3d_toolbox-1.2.0rc0.tar.gz` & `tmp/xcompact3d_toolbox-1.2.0rc1.tar.gz`

## Comparing `xcompact3d_toolbox-1.2.0rc0.tar` & `xcompact3d_toolbox-1.2.0rc1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/readthedocs.yaml
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/ruff_defaults.toml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/sonar-project.properties
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/towncrier.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.github/dependabot.yml
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.github/workflows/1-prepare-release.yaml
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.github/workflows/2-tag-release.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.github/workflows/check-links.yaml
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.vscode/extensions.json
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.vscode/settings.json
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/Docstrings.rst
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/_config.yml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/_toc.yml
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/index.rst
--rw-r--r--   0        0        0    32149 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/logo.png
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/news.md
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/references.bib
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/requirements.txt
--rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Axisymmetric_flow.ipynb
--rw-r--r--   0        0        0    59507 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Axisymmetric_flow.jpg
--rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Cylinder.ipynb
--rw-r--r--   0        0        0    13917 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Heat-exchanger.ipynb
--rw-r--r--   0        0        0   175669 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Heat-exchanger.jpg
--rw-r--r--   0        0        0    14002 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Square.ipynb
--rw-r--r--   0        0        0    72271 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/examples/Square.svg
--rw-r--r--   0        0        0    26763 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/tutorial/computing_and_plotting.ipynb
--rw-r--r--   0        0        0    32635 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/tutorial/io.ipynb
--rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/docs/tutorial/parameters.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/test_genepsi.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/test_stretched_derivatives.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/input.i3d
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/nobjx.dat
--rw-r--r--   0        0        0    15093 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/nobjy.dat
--rw-r--r--   0        0        0   109005 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/nobjz.dat
--rw-r--r--   0        0        0    29250 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/nxifpif.dat
--rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/nyifpif.dat
--rw-r--r--   0        0        0   419250 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/nzifpif.dat
--rw-r--r--   0        0        0    28665 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/xixf.dat
--rw-r--r--   0        0        0    56889 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/yiyf.dat
--rw-r--r--   0        0        0   410865 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/zizf.dat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/__init__.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/test_array.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/test_derivatives.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/test_io.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/test_mesh.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/test_parameters.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/test_sandbox.py
--rw-r--r--   0        0        0    25802 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/snapshots_istret_0.xdmf
--rw-r--r--   0        0        0    26535 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/snapshots_istret_1.xdmf
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_1_0.75_.dat
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_1_1_.dat
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_1_4_.dat
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_2_0.75_.dat
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_2_1_.dat
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_2_4_.dat
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_3_0.75_.dat
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_3_1_.dat
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_3_4_.dat
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/_version.py
--rw-r--r--   0        0        0    13997 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/array.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/derive.py
--rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/genepsi.py
--rw-r--r--   0        0        0    14460 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/gui.py
--rw-r--r--   0        0        0    47739 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/io.py
--rw-r--r--   0        0        0    28005 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/mesh.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/param.py
--rw-r--r--   0        0        0    45163 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/py.typed
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/sandbox.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/tutorial.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/LICENSE
--rw-r--r--   0        0        0    15570 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/README.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/hatch.toml
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/ruff_defaults.toml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/sonar-project.properties
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/towncrier.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.github/workflows/1-prepare-release.yaml
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.github/workflows/2-tag-release.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.github/workflows/check-links.yaml
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.vscode/extensions.json
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/changelog.d/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/Docstrings.rst
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/_config.yml
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/_toc.yml
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/index.rst
+-rw-r--r--   0        0        0    32149 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/logo.png
+-rw-r--r--   0        0        0    16086 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/news.md
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/references.bib
+-rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/requirements.txt
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Axisymmetric_flow.ipynb
+-rw-r--r--   0        0        0    59507 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Axisymmetric_flow.jpg
+-rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Cylinder.ipynb
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Heat-exchanger.ipynb
+-rw-r--r--   0        0        0   175669 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Heat-exchanger.jpg
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Square.ipynb
+-rw-r--r--   0        0        0    72271 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/examples/Square.svg
+-rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/tutorial/computing_and_plotting.ipynb
+-rw-r--r--   0        0        0    32595 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/tutorial/io.ipynb
+-rw-r--r--   0        0        0    20492 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/docs/tutorial/parameters.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/test_genepsi.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/test_stretched_derivatives.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/input.i3d
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/nobjx.dat
+-rw-r--r--   0        0        0    15093 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/nobjy.dat
+-rw-r--r--   0        0        0   109005 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/nobjz.dat
+-rw-r--r--   0        0        0    29250 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/nxifpif.dat
+-rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/nyifpif.dat
+-rw-r--r--   0        0        0   419250 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/nzifpif.dat
+-rw-r--r--   0        0        0    28665 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/xixf.dat
+-rw-r--r--   0        0        0    56889 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/yiyf.dat
+-rw-r--r--   0        0        0   410865 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/zizf.dat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/test_array.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/test_derivatives.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/test_io.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/test_mesh.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/test_parameters.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/test_sandbox.py
+-rw-r--r--   0        0        0    25802 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/snapshots_istret_0.xdmf
+-rw-r--r--   0        0        0    26535 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/snapshots_istret_1.xdmf
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_1_0.75_.dat
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_1_1_.dat
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_1_4_.dat
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_2_0.75_.dat
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_2_1_.dat
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_2_4_.dat
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_3_0.75_.dat
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_3_1_.dat
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_3_4_.dat
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/_version.py
+-rw-r--r--   0        0        0    13997 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/array.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/derive.py
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/genepsi.py
+-rw-r--r--   0        0        0    14460 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/gui.py
+-rw-r--r--   0        0        0    47739 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/io.py
+-rw-r--r--   0        0        0    28005 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/mesh.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/param.py
+-rw-r--r--   0        0        0    45163 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/py.typed
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/sandbox.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/tutorial.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/LICENSE
+-rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/README.md
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/hatch.toml
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 xcompact3d_toolbox-1.2.0rc1/PKG-INFO
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/.pre-commit-config.yaml` & `xcompact3d_toolbox-1.2.0rc1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 default_language_version:
   python: python
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-json
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1
+    rev: v0.4.4
     hooks:
       # Run the linter.
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: [--fix]
       # Run the formatter.
       - id: ruff-format
         types_or: [python, pyi, jupyter]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.8.0"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         exclude: docs/conf.py
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/ruff_defaults.toml` & `xcompact3d_toolbox-1.2.0rc1/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/towncrier.toml` & `xcompact3d_toolbox-1.2.0rc1/towncrier.toml`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/.github/workflows/1-prepare-release.yaml` & `xcompact3d_toolbox-1.2.0rc1/.github/workflows/1-prepare-release.yaml`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/.github/workflows/2-tag-release.yaml` & `xcompact3d_toolbox-1.2.0rc1/.github/workflows/2-tag-release.yaml`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/.github/workflows/ci.yaml` & `xcompact3d_toolbox-1.2.0rc1/.github/workflows/ci.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,21 @@
 concurrency:
   group: "${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}"
   cancel-in-progress: true
 
 jobs:
   test:
     strategy:
+      fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        exclude:
+          - os: macos-latest
+            python-version: "3.8"
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
@@ -59,16 +63,18 @@
       - name: Download coverage data
         uses: actions/download-artifact@v4
         with:
           pattern: coverage-*
           merge-multiple: true
       - name: Set project version
         run: |
+          REF=${{ github.ref }}
           if [[ "${{ github.ref_type }}" == "tag" ]]; then
-            echo "sonar.projectVersion=${{ github.ref }}" >> sonar-project.properties
+            TAG_NAME=${REF#refs/tags/}
+            echo "sonar.projectVersion=$TAG_NAME" >> sonar-project.properties
           fi
       - name: SonarCloud Scan
         uses: SonarSource/sonarcloud-github-action@master
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # Needed to get PR information, if any
           SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}
 
@@ -112,13 +118,7 @@
       - uses: actions/download-artifact@v4
         with:
           name: built-bdist
           path: dist
 
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
-
-      - uses: ncipollo/release-action@v1
-        with:
-          draft: true
-          skipIfReleaseExists: true
-          generateReleaseNotes: true
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/.github/workflows/docs.yaml` & `xcompact3d_toolbox-1.2.0rc1/.github/workflows/docs.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -48,11 +48,11 @@
       - uses: actions/download-artifact@v4
         with:
           path: build/
           name: documentation
 
       # Push the book's HTML to github-pages
       - name: GitHub Pages action
-        uses: peaceiris/actions-gh-pages@v3.9.3
+        uses: peaceiris/actions-gh-pages@v4.0.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: build/_build/html
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/.vscode/settings.json` & `xcompact3d_toolbox-1.2.0rc1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/Docstrings.rst` & `xcompact3d_toolbox-1.2.0rc1/docs/Docstrings.rst`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/_config.yml` & `xcompact3d_toolbox-1.2.0rc1/docs/_config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
   use_edit_page_button: true
   use_issues_button: true
   use_repository_button: true
 
 launch_buttons:
   notebook_interface: "jupyterlab"
   binderhub_url: "https://mybinder.org"
-  colab_url: "https://colab.research.google.com"
 
 sphinx:
   extra_extensions:
     - nbsphinx
     - sphinx.ext.autodoc
     - sphinx.ext.intersphinx
     - sphinx.ext.mathjax
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/_toc.yml` & `xcompact3d_toolbox-1.2.0rc1/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/index.rst` & `xcompact3d_toolbox-1.2.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/logo.png` & `xcompact3d_toolbox-1.2.0rc1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/news.md` & `xcompact3d_toolbox-1.2.0rc1/docs/news.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Intended Effort Versioning](https://jacobtomlinson.dev/effver/) (EffVer for short).
 The changes for the upcoming release can be found in [changelog.d](https://github.com/fschuch/xcompact3d_toolbox/tree/main/changelog.d/).
 
 <!-- WARNING: This file is auto-generated. Do not manually update this file. -->
 
 <!-- towncrier release notes start -->
 
+## [1.2.0rc1](https://github.com/fschuch/xcompact3d_toolbox/releases/tag/v1.2.0rc1) - 2024-05-24<!-- markdown-link-check-disable-line -->
+
+### Documentation
+
+- Migrated documentation hosting from readthedocs to GitHub Pages
+
 ## [1.2.0rc0](https://github.com/fschuch/xcompact3d_toolbox/releases/tag/v1.2.0rc0) - 2024-03-21<!-- markdown-link-check-disable-line -->
 
 ### Added
 
 - Added [loguru](https://loguru.readthedocs.io/en/stable/) to enhance logging in the project
 - Added support for Python 3.10, 3.11, and 3.12
 - Configured [sonarcloud](https://sonarcloud.io/project/overview?id=fschuch_xcompact3d_toolbox) to power code quality analysis and coverage tracking on the project
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/requirements.txt` & `xcompact3d_toolbox-1.2.0rc1/docs/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by hatch-pip-compile with Python 3.12
+# This file is autogenerated by hatch-pip-compile with Python 3.10
 #
 # - docutils
 # - ipykernel
 # - jupyter-book
 # - nbsphinx
 # - pooch
 # - sphinx-autobuild
@@ -25,40 +25,44 @@
 # - datashader>=0.13
 # - holoviews>=1.14
 # - hvplot>=0.7
 # - matplotlib>=3.2
 # - panel>=0.12
 #
 
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
     # via pydata-sphinx-theme
 alabaster==0.7.16
     # via sphinx
+anyio==4.3.0
+    # via
+    #   starlette
+    #   watchfiles
 appnope==0.1.4
     # via ipykernel
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
     # via
     #   jsonschema
     #   jupyter-cache
     #   referencing
-babel==2.14.0
+babel==2.15.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via
     #   nbconvert
     #   panel
-bokeh==3.3.4
+bokeh==3.4.1
     # via
     #   hatch.envs.docs
     #   dask
     #   hvplot
     #   panel
 certifi==2024.2.2
     # via
@@ -71,208 +75,218 @@
 click==8.1.7
     # via
     #   dask
     #   distributed
     #   jupyter-book
     #   jupyter-cache
     #   sphinx-external-toc
+    #   uvicorn
 cloudpickle==3.0.0
     # via
     #   dask
     #   distributed
 colorama==0.4.6
     # via sphinx-autobuild
 colorcet==3.1.0
     # via
     #   datashader
     #   holoviews
     #   hvplot
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via
     #   bokeh
     #   matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.2.1
+dask==2024.5.1
     # via
     #   hatch.envs.docs
+    #   dask-expr
     #   datashader
     #   distributed
-datashader==0.16.0
+dask-expr==1.1.1
+    # via dask
+datashader==0.16.1
     # via hatch.envs.docs
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-distributed==2024.2.1
+distributed==2024.5.1
     # via dask
 docutils==0.20.1
     # via
     #   hatch.envs.docs
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-rtd-theme
     #   sphinx-togglebutton
     #   sphinxcontrib-bibtex
+exceptiongroup==1.2.1
+    # via
+    #   anyio
+    #   ipython
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-fonttools==4.50.0
+fonttools==4.52.1
     # via matplotlib
-fsspec==2024.3.1
+fsspec==2024.5.0
     # via dask
+h11==0.14.0
+    # via uvicorn
 holoviews==1.18.3
     # via
     #   hatch.envs.docs
     #   hvplot
-hvplot==0.9.2
+hvplot==0.10.0
     # via hatch.envs.docs
-idna==3.6
-    # via requests
+idna==3.7
+    # via
+    #   anyio
+    #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==7.0.1
+importlib-metadata==7.1.0
     # via
     #   dask
     #   jupyter-cache
     #   myst-nb
-ipykernel==6.29.3
+ipykernel==6.29.4
     # via
     #   hatch.envs.docs
     #   myst-nb
-ipython==8.22.1
+ipython==8.24.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via hatch.envs.docs
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   bokeh
     #   dask
     #   distributed
     #   jupyter-book
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via
     #   jupyter-book
     #   nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-book==1.0.0
     # via hatch.envs.docs
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.2
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyterlab-pygments==0.3.0
     # via nbconvert
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 kiwisolver==1.4.5
     # via matplotlib
-latexcodec==2.0.1
+latexcodec==3.0.0
     # via pybtex
 linkify-it-py==2.0.3
     # via
     #   jupyter-book
     #   panel
-livereload==2.6.3
-    # via sphinx-autobuild
 llvmlite==0.42.0
     # via numba
 locket==1.0.0
     # via
     #   distributed
     #   partd
 loguru==0.7.2
     # via hatch.envs.docs
 lz4==4.3.3
     # via dask
-markdown==3.5.2
+markdown==3.6
     # via panel
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
     #   panel
 markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.8.3
+matplotlib==3.9.0
     # via hatch.envs.docs
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
     # via
     #   myst-parser
     #   panel
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
 msgpack==1.0.8
     # via distributed
 multipledispatch==1.0.0
     # via datashader
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via jupyter-book
 myst-parser==2.0.0
     # via
     #   jupyter-book
     #   myst-nb
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   nbconvert
-nbconvert==7.16.1
+nbconvert==7.16.4
     # via nbsphinx
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   myst-nb
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.3
+nbsphinx==0.9.4
     # via hatch.envs.docs
 nest-asyncio==1.6.0
     # via ipykernel
 netcdf4==1.6.5
     # via hatch.envs.docs
-numba==0.59.0
+numba==0.59.1
     # via
     #   hatch.envs.docs
     #   datashader
 numpy==1.26.4
     # via
     #   hatch.envs.docs
     #   bokeh
@@ -288,66 +302,67 @@
     #   numpy-stl
     #   pandas
     #   pyarrow
     #   scipy
     #   xarray
 numpy-stl==3.1.1
     # via hatch.envs.docs
-packaging==23.2
+packaging==24.0
     # via
     #   bokeh
     #   dask
     #   distributed
     #   holoviews
     #   hvplot
     #   ipykernel
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-jupyterbook-latex
     #   xarray
-pandas==2.2.1
+pandas==2.2.2
     # via
     #   hatch.envs.docs
     #   bokeh
     #   dask
+    #   dask-expr
     #   datashader
     #   holoviews
     #   hvplot
     #   panel
     #   xarray
 pandocfilters==1.5.1
     # via nbconvert
-panel==1.3.8
+panel==1.4.3
     # via
     #   hatch.envs.docs
     #   holoviews
     #   hvplot
-param==2.0.2
+param==2.1.0
     # via
     #   datashader
     #   holoviews
     #   hvplot
     #   panel
     #   pyct
     #   pyviz-comms
-parso==0.8.3
+parso==0.8.4
     # via jedi
-partd==1.4.1
+partd==1.4.2
     # via dask
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   bokeh
     #   datashader
     #   matplotlib
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via
     #   jupyter-core
     #   pooch
 pooch==1.8.1
     # via hatch.envs.docs
 prompt-toolkit==3.0.43
     # via ipython
@@ -355,98 +370,100 @@
     # via
     #   distributed
     #   ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.2
-    # via dask
+pyarrow==16.1.0
+    # via
+    #   dask
+    #   dask-expr
 pyarrow-hotfix==0.6
     # via dask
 pybtex==0.24.0
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.3
     # via sphinxcontrib-bibtex
 pyct==0.5.0
     # via datashader
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   accessible-pygments
     #   ipython
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
 pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.9.0
+python-dateutil==2.9.0.post0
     # via
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-utils==3.8.2
     # via numpy-stl
 pytz==2024.1
     # via pandas
-pyviz-comms==3.0.1
+pyviz-comms==3.0.2
     # via
     #   holoviews
     #   panel
 pyyaml==6.0.1
     # via
     #   bokeh
     #   dask
     #   distributed
     #   jupyter-book
     #   jupyter-cache
     #   myst-nb
     #   myst-parser
     #   pybtex
     #   sphinx-external-toc
-pyzmq==25.1.2
+pyzmq==26.0.3
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.33.0
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   datashader
     #   panel
     #   pooch
     #   sphinx
-rpds-py==0.18.0
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-scipy==1.12.0
+scipy==1.13.1
     # via
     #   hatch.envs.docs
     #   datashader
 six==1.16.0
     # via
     #   asttokens
     #   bleach
-    #   latexcodec
-    #   livereload
     #   pybtex
     #   python-dateutil
+sniffio==1.3.1
+    # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via distributed
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   hatch.envs.docs
     #   jupyter-book
     #   myst-nb
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
@@ -459,23 +476,23 @@
     #   sphinx-jupyterbook-latex
     #   sphinx-multitoc-numbering
     #   sphinx-rtd-theme
     #   sphinx-thebe
     #   sphinx-togglebutton
     #   sphinxcontrib-bibtex
     #   sphinxcontrib-jquery
-sphinx-autobuild==2024.2.4
+sphinx-autobuild==2024.4.16
     # via hatch.envs.docs
 sphinx-book-theme==1.1.2
     # via jupyter-book
 sphinx-comments==0.0.3
     # via jupyter-book
 sphinx-copybutton==0.5.2
     # via jupyter-book
-sphinx-design==0.5.0
+sphinx-design==0.6.0
     # via jupyter-book
 sphinx-external-toc==1.0.1
     # via jupyter-book
 sphinx-jupyterbook-latex==1.0.0
     # via jupyter-book
 sphinx-multitoc-numbering==0.1.3
     # via jupyter-book
@@ -497,88 +514,100 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.30
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
+starlette==0.37.2
+    # via sphinx-autobuild
 tabulate==0.9.0
     # via jupyter-cache
 tblib==3.0.0
     # via distributed
-tinycss2==1.2.1
+tinycss2==1.3.0
     # via nbconvert
+tomli==2.0.1
+    # via sphinx
 toolz==0.12.1
     # via
     #   dask
     #   datashader
     #   distributed
     #   partd
 tornado==6.4
     # via
     #   bokeh
     #   distributed
     #   ipykernel
     #   jupyter-client
-    #   livereload
-tqdm==4.66.2
+tqdm==4.66.4
     # via
     #   hatch.envs.docs
     #   panel
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   hatch.envs.docs
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
-typing-extensions==4.10.0
+typing-extensions==4.12.0
     # via
+    #   anyio
+    #   ipython
     #   myst-nb
     #   panel
     #   pydata-sphinx-theme
     #   python-utils
     #   sqlalchemy
+    #   uvicorn
 tzdata==2024.1
     # via pandas
 uc-micro-py==1.0.3
     # via linkify-it-py
 urllib3==2.2.1
     # via
     #   distributed
     #   requests
+uvicorn==0.29.0
+    # via sphinx-autobuild
+watchfiles==0.21.0
+    # via sphinx-autobuild
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-wheel==0.42.0
+websockets==12.0
+    # via sphinx-autobuild
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
-xarray==2024.2.0
+xarray==2024.5.0
     # via
     #   hatch.envs.docs
     #   datashader
-xyzservices==2023.10.1
+xyzservices==2024.4.0
     # via
     #   bokeh
     #   panel
 zict==3.0.0
     # via distributed
-zipp==3.17.0
+zipp==3.18.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Axisymmetric_flow.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Axisymmetric_flow.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(2, 'For more information about them, checkout the [API "*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters).')], "*

 * *            "delete: [2]}}, 9: {'source': ['Everything needed is in one Dataset (see [API "*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):']}}"}*

```diff
@@ -54,15 +54,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "* Xcompact3d's parameters\n",
                 "\n",
-                "For more information about them, checkout the [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
+                "For more information about them, checkout the [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -110,15 +110,15 @@
                 "## Setup"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one Dataset (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
+                "Everything needed is in one Dataset (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Axisymmetric_flow.jpg` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Axisymmetric_flow.jpg`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Cylinder.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Cylinder.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988194444444445%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(2, 'For more information about them, checkout the [API "*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters).')], "*

 * *            "delete: [2]}}, 10: {'source': ['Everything needed is in one dictionary of Arrays (see "*

 * *            '[API '*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):']}, "*

 * *            "24: {'source': {ins […]*

```diff
@@ -57,15 +57,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "* Xcompact3d's parameters\n",
                 "\n",
-                "For more information about them, checkout the [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
+                "For more information about them, checkout the [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -120,15 +120,15 @@
                 "### Geometry"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one dictionary of Arrays (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):"
+                "Everything needed is in one dictionary of Arrays (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -252,15 +252,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "It was just to show the capabilities of `xcompact3d_toolbox.sandbox`, you can use it to build many different geometries and arrange them in many ways. However, keep in mind the aspects of numerical stability of our Navier-Stokes solver, **it is up to the user to find the right set of numerical and physical parameters**.\n",
                 "\n",
-                "For a complete description about the available geometries see [Api reference](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.sandbox.Geometry). Notice that you combine them for the creation of unique geometries, or even create your own routines for your own objects.\n",
+                "For a complete description about the available geometries see [Api reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.Geometry). Notice that you combine them for the creation of unique geometries, or even create your own routines for your own objects.\n",
                 "\n",
                 "So, let's start over with a simpler geometry:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -304,15 +304,15 @@
                 "### Boundary Condition"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one Dataset (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
+                "Everything needed is in one Dataset (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Heat-exchanger.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Heat-exchanger.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998937074829932%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(2, 'For more information about them, checkout the [API "*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters).')], "*

 * *            "delete: [2]}}, 10: {'source': ['Everything needed is in one dictionary of Arrays (see "*

 * *            '[API '*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):']}, "*

 * *            "19: {'source': ['Ev […]*

```diff
@@ -53,15 +53,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "* Xcompact3d's parameters\n",
                 "\n",
-                "For more information about them, checkout the [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
+                "For more information about them, checkout the [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -135,15 +135,15 @@
                 "### Geometry"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one dictionary of Arrays (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):"
+                "Everything needed is in one dictionary of Arrays (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -219,15 +219,15 @@
                 "### Boundary Condition"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one Dataset (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
+                "Everything needed is in one Dataset (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Heat-exchanger.jpg` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Heat-exchanger.jpg`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Square.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Square.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988677536231884%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(2, 'For more information about them, checkout the [API "*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters).')], "*

 * *            "delete: [2]}}, 11: {'source': ['Everything needed is in one dictionary of Arrays (see "*

 * *            '[API '*

 * *            "reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):']}, "*

 * *            "21: {'source': ['Ev […]*

```diff
@@ -65,15 +65,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "* Xcompact3d's parameters\n",
                 "\n",
-                "For more information about them, checkout the [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
+                "For more information about them, checkout the [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -145,15 +145,15 @@
                 "### Geometry"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one dictionary of Arrays (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):"
+                "Everything needed is in one dictionary of Arrays (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_epsi)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -243,15 +243,15 @@
                 "### Boundary Condition"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Everything needed is in one Dataset (see [API reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
+                "Everything needed is in one Dataset (see [API reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.sandbox.init_dataset)):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/examples/Square.svg` & `xcompact3d_toolbox-1.2.0rc1/docs/examples/Square.svg`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/tutorial/computing_and_plotting.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/tutorial/computing_and_plotting.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992223011363637%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(7, 'Additionally, xcompact3d-toolbox includes extra "*

 * *            'functionalities for '*

 * *            '[DataArray](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray) '*

 * *            'and '*

 * *            "[Dataset](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataset).\\n')], "*

 * *            'delete: [7]}}, 8: {\'source\': ["Notice there is an entire [tutorial dedicated to the '*

 * *         […]*

```diff
@@ -45,15 +45,15 @@
                 "## Why xarray?\n",
                 "\n",
                 "The data structures are provided by [xarray](http://docs.xarray.dev/en/stable/index.html), that introduces labels in the form of dimensions, coordinates and attributes on top of raw NumPy-like arrays, which allows for a more intuitive, more concise, and less error-prone developer experience.\n",
                 "It integrates tightly with [dask](https://dask.org/) for parallel computing.\n",
                 "\n",
                 "The goal here is to speed up the development of customized post-processing applications with the concise interface provided by [xarray](http://docs.xarray.dev/en/stable/index.html). Ultimately, we can compute solutions with fewer lines of code and better readability, so we expend less time testing and debugging and more time exploring our datasets and getting insights.\n",
                 "\n",
-                "Additionally, xcompact3d-toolbox includes extra functionalities for [DataArray](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray) and [Dataset](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.array.X3dDataset).\n",
+                "Additionally, xcompact3d-toolbox includes extra functionalities for [DataArray](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray) and [Dataset](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataset).\n",
                 "\n",
                 "Before going forward, please, take a look at [Overview: Why xarray?](http://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html) and [Quick overview](http://docs.xarray.dev/en/stable/getting-started-guide/quick-overview.html) to understand the motivation to use [xarray](http://docs.xarray.dev/en/stable/index.html)'s data structures instead of just numpy-like arrays."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5",
@@ -82,15 +82,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8",
             "metadata": {},
             "source": [
-                "Notice there is an entire [tutorial dedicated to the parameters file](https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/parameters.html). Now, let's take a look at the dataset:"
+                "Notice there is an entire [tutorial dedicated to the parameters file](https://docs.fschuch.com/xcompact3d_toolbox/tutorial/parameters.html). Now, let's take a look at the dataset:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9",
             "metadata": {},
@@ -389,15 +389,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "38",
             "metadata": {},
             "source": [
-                "We can use [xarray.DataArray.differentiate](http://docs.xarray.dev/en/stable/generated/xarray.DataArray.differentiate.html) just out of the box with its second order accurate central differences. However, we can use the 4th order accurate centered scheme available at [X3dDataArray.first_derivative](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.first_derivative)."
+                "We can use [xarray.DataArray.differentiate](http://docs.xarray.dev/en/stable/generated/xarray.DataArray.differentiate.html) just out of the box with its second order accurate central differences. However, we can use the 4th order accurate centered scheme available at [X3dDataArray.first_derivative](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.first_derivative)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "39",
             "metadata": {},
             "source": [
@@ -442,16 +442,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "44",
             "metadata": {},
             "source": [
-                "We can use [X3dDataArray.pencil_decomp](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.pencil_decomp) to coarse the velocity array to a dask array, ready for parallel computing (see [Using Dask with xarray](http://docs.xarray.dev/en/stable/user-guide/dask.html#using-dask-with-xarray)).\n",
-                "Notice that [X3dDataArray.pencil_decomp](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.pencil_decomp) applies `chunk=-1` for all coordinates listed in `args`, which means no decomposition, and `'auto'` to the others, delagating to dask the job of finding the optimal distribition.\n",
+                "We can use [X3dDataArray.pencil_decomp](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.pencil_decomp) to coarse the velocity array to a dask array, ready for parallel computing (see [Using Dask with xarray](http://docs.xarray.dev/en/stable/user-guide/dask.html#using-dask-with-xarray)).\n",
+                "Notice that [X3dDataArray.pencil_decomp](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.pencil_decomp) applies `chunk=-1` for all coordinates listed in `args`, which means no decomposition, and `'auto'` to the others, delagating to dask the job of finding the optimal distribition.\n",
                 "One important point here is that dask considers the dataset in this example so small that the overhead for parallel computing is not worth it. As a result, it returns with just one chunk:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "45",
@@ -463,15 +463,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "46",
             "metadata": {},
             "source": [
-                "Parallel computing is presented in this tutorial anyway, because [X3dDataArray.pencil_decomp](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.pencil_decomp) returns the arrays with several chunks for datasets in real scale. Each of these chunks will be computed in parallel in multi-core systems."
+                "Parallel computing is presented in this tutorial anyway, because [X3dDataArray.pencil_decomp](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.array.X3dDataArray.pencil_decomp) returns the arrays with several chunks for datasets in real scale. Each of these chunks will be computed in parallel in multi-core systems."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "47",
             "metadata": {},
             "source": [
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/tutorial/io.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/tutorial/io.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997915524488303%*

 * *Differences: {"'cells'": '{61: {\'source\': ["In the last example we computed the vorticity but did nothing '*

 * *            "with it. This time, let's write it to the disc using "*

 * *            '[write](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.io.Dataset.write):"]}, '*

 * *            '76: {\'source\': {insert: [(14, \'    "url": '*

 * *            '"https://docs.fschuch.com/xcompact3d_toolbox/tutorial/io.html",\\n\')], delete: '*

 * *            '[14]}}, 77: {\'source\': {insert: [(14, \'    "url": ' […]*

```diff
@@ -641,15 +641,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "61",
             "metadata": {},
             "source": [
-                "In the last example we computed the vorticity but did nothing with it. This time, let's write it to the disc using [write](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.io.Dataset.write):"
+                "In the last example we computed the vorticity but did nothing with it. This time, let's write it to the disc using [write](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.io.Dataset.write):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "62",
             "metadata": {},
@@ -809,15 +809,15 @@
                 "snapshot.uy.attrs = {\"name\": \"y\", \"long_name\": \"Vertical velocity\", \"units\": \"-\"}\n",
                 "snapshot.pp.attrs = {\"name\": \"p\", \"long_name\": \"Pressure\", \"units\": \"-\"}\n",
                 "snapshot.w3.attrs = {\"name\": \"w3\", \"long_name\": \"Vorticity\", \"units\": \"-\"}\n",
                 "\n",
                 "# Setting attributes for the dataset\n",
                 "snapshot.attrs = {\n",
                 "    \"title\": \"An example from the tutorials\",\n",
-                "    \"url\": \"https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/io.html\",\n",
+                "    \"url\": \"https://docs.fschuch.com/xcompact3d_toolbox/tutorial/io.html\",\n",
                 "    \"authors\": \"List of names\",\n",
                 "    \"doi\": \"maybe a fancy doi from zenodo\",\n",
                 "}"
             ]
         },
         {
             "cell_type": "code",
@@ -836,15 +836,15 @@
                 "snapshot.uy.attrs = {\"name\": \"y\", \"long_name\": \"Vertical velocity\", \"units\": \"-\"}\n",
                 "snapshot.pp.attrs = {\"name\": \"p\", \"long_name\": \"Pressure\", \"units\": \"-\"}\n",
                 "snapshot.w3.attrs = {\"name\": \"w3\", \"long_name\": \"Vorticity\", \"units\": \"-\"}\n",
                 "\n",
                 "# Setting attributes for the dataset\n",
                 "snapshot.attrs = {\n",
                 "    \"title\": \"An example from the tutorials\",\n",
-                "    \"url\": \"https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/io.html\",\n",
+                "    \"url\": \"https://docs.fschuch.com/xcompact3d_toolbox/tutorial/io.html\",\n",
                 "    \"authors\": \"List of names\",\n",
                 "    \"doi\": \"maybe a fancy doi from zenodo\",\n",
                 "}"
             ]
         },
         {
             "cell_type": "code",
@@ -863,15 +863,15 @@
                 "snapshot.uy.attrs = {\"name\": \"y\", \"long_name\": \"Vertical velocity\", \"units\": \"-\"}\n",
                 "snapshot.pp.attrs = {\"name\": \"p\", \"long_name\": \"Pressure\", \"units\": \"-\"}\n",
                 "snapshot.w3.attrs = {\"name\": \"w3\", \"long_name\": \"Vorticity\", \"units\": \"-\"}\n",
                 "\n",
                 "# Setting attributes for the dataset\n",
                 "snapshot.attrs = {\n",
                 "    \"title\": \"An example from the tutorials\",\n",
-                "    \"url\": \"https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/io.html\",\n",
+                "    \"url\": \"https://docs.fschuch.com/xcompact3d_toolbox/tutorial/io.html\",\n",
                 "    \"authors\": \"List of names\",\n",
                 "    \"doi\": \"maybe a fancy doi from zenodo\",\n",
                 "}"
             ]
         },
         {
             "cell_type": "code",
@@ -890,15 +890,15 @@
                 "snapshot.uy.attrs = {\"name\": \"y\", \"long_name\": \"Vertical velocity\", \"units\": \"-\"}\n",
                 "snapshot.pp.attrs = {\"name\": \"p\", \"long_name\": \"Pressure\", \"units\": \"-\"}\n",
                 "snapshot.w3.attrs = {\"name\": \"w3\", \"long_name\": \"Vorticity\", \"units\": \"-\"}\n",
                 "\n",
                 "# Setting attributes for the dataset\n",
                 "snapshot.attrs = {\n",
                 "    \"title\": \"An example from the tutorials\",\n",
-                "    \"url\": \"https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/io.html\",\n",
+                "    \"url\": \"https://docs.fschuch.com/xcompact3d_toolbox/tutorial/io.html\",\n",
                 "    \"authors\": \"List of names\",\n",
                 "    \"doi\": \"maybe a fancy doi from zenodo\",\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/docs/tutorial/parameters.ipynb` & `xcompact3d_toolbox-1.2.0rc1/docs/tutorial/parameters.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999488936988937%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'The computational and physical parameters are handled "*

 * *            'by '*

 * *            '[xcompact3d_toolbox.Parameters](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters). '*

 * *            'It is built on top of '*

 * *            '[Traitlets](https://traitlets.readthedocs.io/en/stable/index.html), which aims to '*

 * *            'make the parameters compatible with what XCompact3d expects, and also brings some '*

 * *            "a […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Parameters\n",
                 "\n",
-                "The computational and physical parameters are handled by [xcompact3d_toolbox.Parameters](https://xcompact3d-toolbox.readthedocs.io/en/stable/Docstrings.html#xcompact3d_toolbox.parameters.Parameters). It is built on top of [Traitlets](https://traitlets.readthedocs.io/en/stable/index.html), which aims to make the parameters compatible with what XCompact3d expects, and also brings some advantages:\n",
+                "The computational and physical parameters are handled by [xcompact3d_toolbox.Parameters](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html#xcompact3d_toolbox.parameters.Parameters). It is built on top of [Traitlets](https://traitlets.readthedocs.io/en/stable/index.html), which aims to make the parameters compatible with what XCompact3d expects, and also brings some advantages:\n",
                 "\n",
                 "* Attributes are type-checked;\n",
                 "* Default values, restrictions and connections between related parameters are applied when necessary;\n",
                 "* 'On change' callbacks for validation and observation;\n",
                 "* Two-way linking with [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/)."
             ]
         },
@@ -64,15 +64,15 @@
                 "prm = x3d.Parameters()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You can access a list with all the available variables at the [Api reference](https://xcompact3d-toolbox.readthedocs.io/en/latest/Docstrings.html)."
+                "You can access a list with all the available variables at the [Api reference](https://docs.fschuch.com/xcompact3d_toolbox/Docstrings.html)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's see how it looks like:"
@@ -255,16 +255,16 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "More details about I/O and array manipulations with [xarray](http://docs.xarray.dev/en/stable/index.html) are available at:\n",
                 "\n",
-                "* [Reading and writing files](https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/io.html);\n",
-                "* [Computing and Plotting](https://xcompact3d-toolbox.readthedocs.io/en/stable/tutorial/computing_and_plotting.html)."
+                "* [Reading and writing files](https://docs.fschuch.com/xcompact3d_toolbox/tutorial/io.html);\n",
+                "* [Computing and Plotting](https://docs.fschuch.com/xcompact3d_toolbox/tutorial/computing_and_plotting.html)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Traitlets\n",
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/integration/test_genepsi.py` & `xcompact3d_toolbox-1.2.0rc1/tests/integration/test_genepsi.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/integration/test_stretched_derivatives.py` & `xcompact3d_toolbox-1.2.0rc1/tests/integration/test_stretched_derivatives.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/integration/data/input.i3d` & `xcompact3d_toolbox-1.2.0rc1/tests/integration/data/input.i3d`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/xixf.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/xixf.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/yiyf.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/yiyf.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/integration/data/geometry/zizf.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/integration/data/geometry/zizf.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/test_array.py` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/test_array.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/test_derivatives.py` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/test_io.py` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/test_io.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/test_mesh.py` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/test_mesh.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/test_parameters.py` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/test_parameters.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/test_sandbox.py` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/snapshots_istret_0.xdmf` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/snapshots_istret_0.xdmf`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/snapshots_istret_1.xdmf` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/snapshots_istret_1.xdmf`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_1_0.75_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_1_0.75_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_1_1_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_1_1_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_1_4_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_1_4_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_2_0.75_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_2_0.75_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_2_1_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_2_1_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_2_4_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_2_4_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_3_0.75_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_3_0.75_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_3_1_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_3_1_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/tests/unit/data/yp/yp_3_4_.dat` & `xcompact3d_toolbox-1.2.0rc1/tests/unit/data/yp/yp_3_4_.dat`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/array.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/array.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/derive.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/derive.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/genepsi.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/genepsi.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/gui.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/gui.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/io.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/io.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/mesh.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/mesh.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/param.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/param.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/parameters.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/parameters.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/sandbox.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/xcompact3d_toolbox/tutorial.py` & `xcompact3d_toolbox-1.2.0rc1/xcompact3d_toolbox/tutorial.py`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/.gitignore` & `xcompact3d_toolbox-1.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/LICENSE` & `xcompact3d_toolbox-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `xcompact3d_toolbox-1.2.0rc0/README.md` & `xcompact3d_toolbox-1.2.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Xcompact3d Toolbox
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | QA      | [![CI](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/ci.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/fschuch/xcompact3d_toolbox/main.svg)](https://results.pre-commit.ci/latest/github/fschuch/xcompact3d_toolbox/main)[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fschuch_xcompact3d_toolbox&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fschuch_xcompact3d_toolbox)[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fschuch_xcompact3d_toolbox&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fschuch_xcompact3d_toolbox)        |
-| Docs    | [![Docs](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/docs.yaml)[![Documentation Status](https://readthedocs.org/projects/xcompact3d_toolbox/badge/?version=latest)](https://xcompact3d-toolbox.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| Docs    | [![Docs](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/docs.yaml/badge.svg?branch=main)](https://docs.fschuch.com/xcompact3d_toolbox)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/xcompact3d-toolbox.svg?logo=pypi&label=PyPI)](https://pypi.org/project/xcompact3d-toolbox/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcompact3d-toolbox.svg?logo=python&label=Python)](https://pypi.org/project/xcompact3d-toolbox/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
 | Meta    | [![Wizard Template](https://img.shields.io/badge/Wizard-Template-%23447CAA)](https://github.com/fschuch/wizard-template) [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![PyPI - License](https://img.shields.io/pypi/l/xcompact3d-toolbox?color=blue)](https://github.com/fschuch/xcompact3d_toolbox/blob/master/LICENSE) [![EffVer Versioning](https://img.shields.io/badge/version_scheme-EffVer-0097a7)](https://jacobtomlinson.dev/effver) |
 
 It is a Python package designed to handle the pre and postprocessing of
 the high-order Navier-Stokes solver [XCompact3d](https://github.com/xcompact3d/Incompact3d). It aims to help users and
 code developers to build case-specific solutions with a set of tools and
 automated processes.
@@ -15,22 +15,22 @@
 The physical and computational parameters are built on top of [traitlets](https://traitlets.readthedocs.io/en/stable/index.html),
 a framework that lets Python classes have attributes with type checking, dynamically calculated default values, and ‘on change’ callbacks.
 In addition to [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/) for an user friendly interface.
 
 Data structure is provided by [xarray](https://docs.xarray.dev/en/stable) (see [Why xarray?](https://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html)), that introduces labels in the form of dimensions, coordinates and attributes on top of raw [NumPy](https://numpy.org/)-like arrays, which allows for a more intuitive, more concise, and less error-prone developer experience. It integrates tightly with [dask](https://dask.org/) for parallel computing and [hvplot](https://hvplot.holoviz.org/user_guide/Gridded_Data.html) for interactive data visualization.
 
 Finally, Xcompact3d-toolbox is fully integrated with the new *Sandbox Flow Configuration*.
-The idea is to easily provide everything that XCompact3d needs from a [Jupyter Notebook](https://jupyter.org/), like initial conditions, solid geometry, boundary conditions, and the parameters ([see examples](https://xcompact3d-toolbox.readthedocs.io/en/latest/tutorial.html#sandbox-examples)).
+The idea is to easily provide everything that XCompact3d needs from a [Jupyter Notebook](https://jupyter.org/), like initial conditions, solid geometry, boundary conditions, and the parameters.
 It makes life easier for beginners, that can run any new flow configuration without worrying about Fortran and [2decomp](http://www.2decomp.org/).
 For developers, it works as a rapid prototyping tool, to test concepts and then compare results to validate any future Fortran implementation.
 
 ## Useful links
 
-- [Documentation](https://xcompact3d-toolbox.readthedocs.io/);
-- [Changelog](https://github.com/fschuch/xcompact3d_toolbox/blob/master/docs/news.md);
+- [Documentation](https://docs.fschuch.com/xcompact3d_toolbox/);
+- [Changelog](https://docs.fschuch.com/xcompact3d_toolbox/news.html);
 - [Suggestions for new features and bug report](https://github.com/fschuch/xcompact3d_toolbox/issues);
 - [See what is coming next (Project page)](https://github.com/fschuch/xcompact3d_toolbox/projects/1);
 - [Xcompact3d's repository](https://github.com/xcompact3d/Incompact3d).
 
 ## Installation
 
 It is possible to install using pip:
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/hatch.toml` & `xcompact3d_toolbox-1.2.0rc1/hatch.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 [version]
 path = "xcompact3d_toolbox/_version.py"
 pattern = '__version__ = "(?P<version>[^"]+)"'
 
 [envs.default]
 description = "Base development environment"
+installer = "uv"
 dependencies = [
     "coverage[toml]",
     "hypothesis>=4.53",
     "pre-commit",
     "pytest-cov",
     "pytest",
 ]
@@ -18,15 +19,15 @@
 [envs.default.scripts]
 pre-commit-install = "pre-commit install {args}"
 pre-commit-uninstall = "pre-commit uninstall {args}"
 check = "pre-commit run {args} --all-files"
 type = "check mypy {args}"
 lint = "check ruff {args}"
 format = "check ruff-format {args}"
-test = "pytest --cov --cov-report=term {args}"
+test = "pytest --cov --cov-report=term --cov=xcompact3d_toolbox --cov=tests {args}"
 test-no-cov = "test --no-cov {args}"
 qa = ["check", "test", "echo '✅ QA passed'"]
 
 [envs.test]
 description = "Extended test environment"
 extra-dependencies = ["pytest-randomly", "pytest-rerunfailures", "pytest-xdist"]
 
@@ -35,16 +36,16 @@
 
 [[envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [envs.docs]
 description = "Documentation environment"
 features = ["visu"]
+template = "docs"
 install = true
-detached = false
 dependencies = [
     "docutils",
     "ipykernel",
     "jupyter-book",
     "nbsphinx",
     "pooch",
     "sphinx-autobuild",
@@ -57,21 +58,19 @@
 [envs.docs.scripts]
 config = "jupyter-book config sphinx docs {args}"
 build = ["config", "jupyter-book build docs --path-output build {args}"]
 serve = ["config", "sphinx-autobuild docs build/_build/html --ignore='**/data/*' --open-browser {args}"]
 
 [envs.changelog]
 description = "Changelog handler"
+template = "changelog"
+install = true
 dependencies = ["towncrier"]
 
 [envs.changelog.scripts]
 build = "towncrier build {args}"
 draft = "build --draft {args}"
 create = "towncrier create {args}"
 check = "towncrier check {args}"
 
 [envs.hatch-static-analysis]
 config-path = "ruff_defaults.toml"
-
-[dirs.env]
-virtual = ".venv"
-pip-compile = ".venv"
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/pyproject.toml` & `xcompact3d_toolbox-1.2.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     "datashader>=0.13",
     "hvplot>=0.7",
     "panel>=0.12",
     "holoviews>=1.14",
 ]
 
 [project.urls]
-Changelog = "https://github.com/fschuch/xcompact3d_toolbox/blob/main/docs/news.md"
-Documentation = "https://xcompact3d-toolbox.readthedocs.io/"
+Changelog = "https://docs.fschuch.com/xcompact3d_toolbox/news.html"
+Documentation = "https://docs.fschuch.com/xcompact3d_toolbox"
 Issues = "https://github.com/fschuch/xcompact3d_toolbox/issues"
 Repository = "https://github.com/fschuch/xcompact3d_toolbox"
 
 [tool.pytest.ini_options]
 minversion = "8.0"
 # addopts = [
 #     "--doctest-modules",
@@ -57,15 +57,15 @@
 #     "--doctest-report=ndiff",
 # ]
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 source = ["xcompact3d_toolbox", "tests"]
-omit = ["xcompact3d_toolbox/_version.py"]
+omit = ["xcompact3d_toolbox/_version.py", "**/__init__.py"]
 
 [tool.coverage.report]
 show_missing = true
 precision = 2
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:", "def __repr__"]
 
 [tool.ruff]
```

### Comparing `xcompact3d_toolbox-1.2.0rc0/PKG-INFO` & `xcompact3d_toolbox-1.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: xcompact3d_toolbox
-Version: 1.2.0rc0
+Version: 1.2.0rc1
 Summary: A set of tools for pre and postprocessing prepared for the high-order Navier-Stokes solver XCompact3d
-Project-URL: Changelog, https://github.com/fschuch/xcompact3d_toolbox/blob/main/docs/news.md
-Project-URL: Documentation, https://xcompact3d-toolbox.readthedocs.io/
+Project-URL: Changelog, https://docs.fschuch.com/xcompact3d_toolbox/news.html
+Project-URL: Documentation, https://docs.fschuch.com/xcompact3d_toolbox
 Project-URL: Issues, https://github.com/fschuch/xcompact3d_toolbox/issues
 Project-URL: Repository, https://github.com/fschuch/xcompact3d_toolbox
 Author-email: "Felipe N. Schuch" <me@fschuch.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -41,15 +41,15 @@
 Description-Content-Type: text/markdown
 
 # Xcompact3d Toolbox
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | QA      | [![CI](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/ci.yaml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/fschuch/xcompact3d_toolbox/main.svg)](https://results.pre-commit.ci/latest/github/fschuch/xcompact3d_toolbox/main)[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fschuch_xcompact3d_toolbox&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fschuch_xcompact3d_toolbox)[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fschuch_xcompact3d_toolbox&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fschuch_xcompact3d_toolbox)        |
-| Docs    | [![Docs](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/docs.yaml)[![Documentation Status](https://readthedocs.org/projects/xcompact3d_toolbox/badge/?version=latest)](https://xcompact3d-toolbox.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| Docs    | [![Docs](https://github.com/fschuch/xcompact3d_toolbox/actions/workflows/docs.yaml/badge.svg?branch=main)](https://docs.fschuch.com/xcompact3d_toolbox)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/xcompact3d-toolbox.svg?logo=pypi&label=PyPI)](https://pypi.org/project/xcompact3d-toolbox/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcompact3d-toolbox.svg?logo=python&label=Python)](https://pypi.org/project/xcompact3d-toolbox/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
 | Meta    | [![Wizard Template](https://img.shields.io/badge/Wizard-Template-%23447CAA)](https://github.com/fschuch/wizard-template) [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![PyPI - License](https://img.shields.io/pypi/l/xcompact3d-toolbox?color=blue)](https://github.com/fschuch/xcompact3d_toolbox/blob/master/LICENSE) [![EffVer Versioning](https://img.shields.io/badge/version_scheme-EffVer-0097a7)](https://jacobtomlinson.dev/effver) |
 
 It is a Python package designed to handle the pre and postprocessing of
 the high-order Navier-Stokes solver [XCompact3d](https://github.com/xcompact3d/Incompact3d). It aims to help users and
 code developers to build case-specific solutions with a set of tools and
 automated processes.
@@ -57,22 +57,22 @@
 The physical and computational parameters are built on top of [traitlets](https://traitlets.readthedocs.io/en/stable/index.html),
 a framework that lets Python classes have attributes with type checking, dynamically calculated default values, and ‘on change’ callbacks.
 In addition to [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/) for an user friendly interface.
 
 Data structure is provided by [xarray](https://docs.xarray.dev/en/stable) (see [Why xarray?](https://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html)), that introduces labels in the form of dimensions, coordinates and attributes on top of raw [NumPy](https://numpy.org/)-like arrays, which allows for a more intuitive, more concise, and less error-prone developer experience. It integrates tightly with [dask](https://dask.org/) for parallel computing and [hvplot](https://hvplot.holoviz.org/user_guide/Gridded_Data.html) for interactive data visualization.
 
 Finally, Xcompact3d-toolbox is fully integrated with the new *Sandbox Flow Configuration*.
-The idea is to easily provide everything that XCompact3d needs from a [Jupyter Notebook](https://jupyter.org/), like initial conditions, solid geometry, boundary conditions, and the parameters ([see examples](https://xcompact3d-toolbox.readthedocs.io/en/latest/tutorial.html#sandbox-examples)).
+The idea is to easily provide everything that XCompact3d needs from a [Jupyter Notebook](https://jupyter.org/), like initial conditions, solid geometry, boundary conditions, and the parameters.
 It makes life easier for beginners, that can run any new flow configuration without worrying about Fortran and [2decomp](http://www.2decomp.org/).
 For developers, it works as a rapid prototyping tool, to test concepts and then compare results to validate any future Fortran implementation.
 
 ## Useful links
 
-- [Documentation](https://xcompact3d-toolbox.readthedocs.io/);
-- [Changelog](https://github.com/fschuch/xcompact3d_toolbox/blob/master/docs/news.md);
+- [Documentation](https://docs.fschuch.com/xcompact3d_toolbox/);
+- [Changelog](https://docs.fschuch.com/xcompact3d_toolbox/news.html);
 - [Suggestions for new features and bug report](https://github.com/fschuch/xcompact3d_toolbox/issues);
 - [See what is coming next (Project page)](https://github.com/fschuch/xcompact3d_toolbox/projects/1);
 - [Xcompact3d's repository](https://github.com/xcompact3d/Incompact3d).
 
 ## Installation
 
 It is possible to install using pip:
```

