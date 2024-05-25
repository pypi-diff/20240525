# Comparing `tmp/pymoxel-0.1.1.tar.gz` & `tmp/pymoxel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoxel-0.1.1.tar", last modified: Tue May  7 11:14:41 2024, max compression
+gzip compressed data, was "pymoxel-0.1.2.tar", last modified: Sat May 25 16:09:35 2024, max compression
```

## Comparing `pymoxel-0.1.1.tar` & `pymoxel-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.766997 pymoxel-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.750997 pymoxel-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-07 11:14:37.000000 pymoxel-0.1.1/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 11:14:37.000000 pymoxel-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-07 11:14:37.000000 pymoxel-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 11:14:37.000000 pymoxel-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 11:14:41.766997 pymoxel-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-07 11:14:37.000000 pymoxel-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.754997 pymoxel-0.1.1/docs/source/down/
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/down/CIFs.zip
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/down/IRMOF-1.cif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.758997 pymoxel-0.1.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)   101913 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/moxel_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  1955651 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/moxel_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   423802 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/plot_voxels.png
--rw-r--r--   0 runner    (1001) docker     (127)   347027 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/images/voxels.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/moxel.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-07 11:14:37.000000 pymoxel-0.1.1/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-07 11:14:37.000000 pymoxel-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:14:41.766997 pymoxel-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.750997 pymoxel-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.762997 pymoxel-0.1.1/src/moxel/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-07 11:14:37.000000 pymoxel-0.1.1/src/moxel/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.766997 pymoxel-0.1.1/src/pymoxel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 11:14:41.000000 pymoxel-0.1.1/src/pymoxel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.762997 pymoxel-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:41.766997 pymoxel-0.1.1/tests/CIFs/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/COF-5.cif
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/IRMOF-1.cif
--rw-r--r--   0 runner    (1001) docker     (127)   113146 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/MnH28C26(N2Cl)2.json
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/ZIF-69.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/ZnHBDC.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/ZnMOF-74.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_1.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_2.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_3.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/CIFs/corrupted_4.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 11:14:37.000000 pymoxel-0.1.1/tests/test_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.618469 pymoxel-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.606469 pymoxel-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.606469 pymoxel-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-25 16:09:31.000000 pymoxel-0.1.2/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-25 16:09:31.000000 pymoxel-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-25 16:09:31.000000 pymoxel-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 16:09:31.000000 pymoxel-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-25 16:09:35.618469 pymoxel-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-25 16:09:31.000000 pymoxel-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.606469 pymoxel-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.610468 pymoxel-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.610468 pymoxel-0.1.2/docs/source/down/
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/down/CIFs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/down/IRMOF-1.cif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.614468 pymoxel-0.1.2/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   101913 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/images/moxel_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1955651 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/images/moxel_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   423802 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/images/plot_voxels.png
+-rw-r--r--   0 runner    (1001) docker     (127)   347027 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/images/voxels.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/moxel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-25 16:09:31.000000 pymoxel-0.1.2/docs/source/visualize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-25 16:09:31.000000 pymoxel-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:09:35.618469 pymoxel-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.606469 pymoxel-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.614468 pymoxel-0.1.2/src/moxel/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-25 16:09:31.000000 pymoxel-0.1.2/src/moxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-25 16:09:31.000000 pymoxel-0.1.2/src/moxel/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-25 16:09:31.000000 pymoxel-0.1.2/src/moxel/_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-25 16:09:31.000000 pymoxel-0.1.2/src/moxel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-25 16:09:31.000000 pymoxel-0.1.2/src/moxel/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.618469 pymoxel-0.1.2/src/pymoxel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-25 16:09:35.000000 pymoxel-0.1.2/src/pymoxel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-25 16:09:35.000000 pymoxel-0.1.2/src/pymoxel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:09:35.000000 pymoxel-0.1.2/src/pymoxel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 16:09:35.000000 pymoxel-0.1.2/src/pymoxel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 16:09:35.000000 pymoxel-0.1.2/src/pymoxel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 16:09:35.000000 pymoxel-0.1.2/src/pymoxel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.614468 pymoxel-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:35.618469 pymoxel-0.1.2/tests/CIFs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/COF-5.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/IRMOF-1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   113146 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/MnH28C26(N2Cl)2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/ZIF-69.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/ZnHBDC.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/ZnMOF-74.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/corrupted_1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/corrupted_2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/corrupted_3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/CIFs/corrupted_4.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-25 16:09:31.000000 pymoxel-0.1.2/tests/test_visualize.py
```

### Comparing `pymoxel-0.1.1/.github/workflows/python-publish.yaml` & `pymoxel-0.1.2/.github/workflows/python-publish.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `pymoxel-0.1.1/.readthedocs.yaml` & `pymoxel-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/LICENSE` & `pymoxel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/PKG-INFO` & `pymoxel-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pymoxel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for parallel calculation of energy voxels.
 Author-email: "Antonios P. Sarikas" <antonios.sarikas@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/adosar/moxel
 Project-URL: Documentation, https://moxel.readthedocs.io
-Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changes.html
+Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changelog.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `pymoxel-0.1.1/README.md` & `pymoxel-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/Makefile` & `pymoxel-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/make.bat` & `pymoxel-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/conf.py` & `pymoxel-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/down/CIFs.zip` & `pymoxel-0.1.2/docs/source/down/CIFs.zip`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/down/IRMOF-1.cif` & `pymoxel-0.1.2/docs/source/down/IRMOF-1.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/images/moxel_logo.png` & `pymoxel-0.1.2/docs/source/images/moxel_logo.png`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/images/moxel_logo.svg` & `pymoxel-0.1.2/docs/source/images/moxel_logo.svg`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/images/plot_voxels.png` & `pymoxel-0.1.2/docs/source/images/plot_voxels.png`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/images/voxels.gif` & `pymoxel-0.1.2/docs/source/images/voxels.gif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/index.rst` & `pymoxel-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/docs/source/tutorial.rst` & `pymoxel-0.1.2/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/pyproject.toml` & `pymoxel-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -35,11 +35,11 @@
 	"matplotlib",
 	"pyvista",
 ]
 
 [project.urls]
 Homepage = "https://github.com/adosar/moxel"
 Documentation = "https://moxel.readthedocs.io"
-Changelog = "https://moxel.readthedocs.io/en/stable/changes.html"
+Changelog = "https://moxel.readthedocs.io/en/stable/changelog.html"
 
 [project.scripts]
-moxel = "moxel.cli:moxel_fire"
+moxel = "moxel._cli:moxel_fire"
```

### Comparing `pymoxel-0.1.1/src/moxel/__init__.py` & `pymoxel-0.1.2/src/moxel/__init__.py`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/src/moxel/_params.py` & `pymoxel-0.1.2/src/moxel/_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+r"""
+This module provides the Lennard-Jones parameters from UFF.
+"""
+
 lj_params = {
     "H": [
         22.11417,
         2.571134
     ],
     "B": [
         90.5798,
```

### Comparing `pymoxel-0.1.1/src/moxel/cli.py` & `pymoxel-0.1.2/src/moxel/_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+r"""
+This module provides helper functions for the CLI.
+"""
+
 import fire
 from . utils import voxels_from_dir, batch_clean
 
 
 def moxel_fire():
-  fire.Fire({
-      'clean': batch_clean,
-      'create': voxels_from_dir,
-  })
+    r"""
+    Run the CLI.
+    """
+    fire.Fire({
+        'clean': batch_clean,
+        'create': voxels_from_dir,
+    })
```

### Comparing `pymoxel-0.1.1/src/moxel/utils.py` & `pymoxel-0.1.2/src/moxel/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,31 +45,31 @@
 import numpy as np
 from tqdm import tqdm
 from pymatgen.core import Structure
 from . _params import lj_params
 warnings.filterwarnings('ignore')
 
 
-def get_names(fname):
+def load_json(fname):
     r"""
-    Load a list of material names saved in ``.json`` format.
+    Load a ``.json`` file.
 
     Parameters
     ----------
     fname : str
         Pathname to the ``.json`` file.
 
     Returns
     -------
     names : list
     """
     with open(fname, 'r') as fhand:
-        names = json.load(fhand)
+        data = json.load(fhand)
 
-    return names
+    return data
 
 
 def mic_scale_factors(r, lattice_vectors):
     r"""
     Return scale factors to satisfy minimum image convention [MIC]_.
 
     Parameters
@@ -164,16 +164,16 @@
             LJ potential is supported.
         cubic_box : bool, default=False
             If ``True``, the simulation box is cubic.
         length : float, default=30
             The size of the cubic box in Å. Takes effect only
             if ``cubic_box == True``.
         n_jobs : int, optional
-            Number of jobs to run in parallel. If ``None``, all processors are
-            used.
+            Number of jobs to run in parallel. If ``None``, then the number returned
+            by ``os.cpu_count()`` is used.
 
         Returns
         -------
         voxels : array of shape (grid_size,)*3
             The energy voxels as :math:`e^{-\beta \mathcal{V}}`, to ensure
             numerical stability.
         Notes
@@ -274,15 +274,16 @@
     sigma : float, default=25
         Sigma value (σ/Å) of the probe atom.
     cubic_box : bool, default=False
         If ``True``, the simulation box is cubic.
     length : float, default=30
         The size of the cubic box in Å. Takes effect only if ``cubic_box == True``.
     n_jobs : int, optional
-        Number of jobs to run in parallel. If ``None``, all processors are used.
+        Number of jobs to run in parallel. If ``None``, then the number returned
+        by ``os.cpu_count()`` is used.
     only_voxels : bool, default=True
         Determines ``out`` type.
         
     Returns
     -------
     out : ``array`` or :class:`Grid`
         If ``only_voxels == True``, array of shape ``(grid_size,)*3``.
@@ -297,16 +298,16 @@
         grid.load_structure(cif_pathname)
         grid.calculate(cubic_box=cubic_box, length=length, n_jobs=n_jobs)
     except:
         grid.voxels = np.full(shape=(grid_size,)*3, fill_value=0, dtype=np.float32)
 
     if only_voxels:
         return grid.voxels
-    else:
-        return grid
+
+    return grid
 
 
 def voxels_from_files(
         cif_pathnames, out_pathname, grid_size=25, cutoff=10,
         epsilon=50, sigma=2.5, cubic_box=False, length=30,
         n_jobs=None,
         ):
@@ -463,15 +464,15 @@
 
     Returns
     -------
     exit_status : int
         If no voxels are missing ``0`` else ``1``.
     """
     # Case 1: no missing voxels.
-    names = get_names(f'{batch_dirname}/names.json')
+    names = load_json(f'{batch_dirname}/names.json')
     voxels = np.load(f'{batch_dirname}/voxels.npy', mmap_mode='r')
 
     missing_idx = [i for i, x in enumerate(voxels) if np.all(x == 0)]
 
     if len(missing_idx) == 0:
         print('No missing voxels found!')
         return 0
```

### Comparing `pymoxel-0.1.1/src/moxel/visualize.py` & `pymoxel-0.1.2/src/moxel/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     Examples
     --------
     >>> voxels = np.random.randn(5, 5, 5)
     >>> fig = plot_voxels_mpl(voxels, cmap='coolwarm')
     >>> plt.show()  # Not needed for Jupyter.
     """
 
-    if np.all(fill_pattern) == None:
+    if np.all(fill_pattern) is None:
         fill_pattern = np.full(voxels.shape, True)
 
     cmap = plt.get_cmap(cmap)
     norm = mpl.colors.Normalize()
     colors = cmap((voxels - voxels.min()) / (voxels.max() - voxels.min()))
 
     fig, ax = plt.subplots(subplot_kw={'projection': '3d'})
```

### Comparing `pymoxel-0.1.1/src/pymoxel.egg-info/PKG-INFO` & `pymoxel-0.1.2/src/pymoxel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pymoxel
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for parallel calculation of energy voxels.
 Author-email: "Antonios P. Sarikas" <antonios.sarikas@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/adosar/moxel
 Project-URL: Documentation, https://moxel.readthedocs.io
-Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changes.html
+Project-URL: Changelog, https://moxel.readthedocs.io/en/stable/changelog.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `pymoxel-0.1.1/src/pymoxel.egg-info/SOURCES.txt` & `pymoxel-0.1.2/src/pymoxel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 docs/source/cli.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/modules.rst
 docs/source/moxel.rst
 docs/source/tutorial.rst
+docs/source/utils.rst
+docs/source/visualize.rst
 docs/source/down/CIFs.zip
 docs/source/down/IRMOF-1.cif
 docs/source/images/moxel_logo.png
 docs/source/images/moxel_logo.svg
 docs/source/images/plot_voxels.png
 docs/source/images/voxels.gif
 src/moxel/__init__.py
+src/moxel/_cli.py
 src/moxel/_params.py
-src/moxel/cli.py
 src/moxel/utils.py
 src/moxel/visualize.py
 src/pymoxel.egg-info/PKG-INFO
 src/pymoxel.egg-info/SOURCES.txt
 src/pymoxel.egg-info/dependency_links.txt
 src/pymoxel.egg-info/entry_points.txt
 src/pymoxel.egg-info/requires.txt
```

### Comparing `pymoxel-0.1.1/tests/CIFs/COF-5.cif` & `pymoxel-0.1.2/tests/CIFs/COF-5.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/tests/CIFs/IRMOF-1.cif` & `pymoxel-0.1.2/tests/CIFs/IRMOF-1.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/tests/CIFs/MnH28C26(N2Cl)2.json` & `pymoxel-0.1.2/tests/CIFs/MnH28C26(N2Cl)2.json`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/tests/CIFs/ZIF-69.cif` & `pymoxel-0.1.2/tests/CIFs/ZIF-69.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/tests/CIFs/ZnHBDC.cif` & `pymoxel-0.1.2/tests/CIFs/ZnHBDC.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/tests/CIFs/ZnMOF-74.cif` & `pymoxel-0.1.2/tests/CIFs/ZnMOF-74.cif`

 * *Files identical despite different names*

### Comparing `pymoxel-0.1.1/tests/test_utils.py` & `pymoxel-0.1.2/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         names = [Path(i).stem for i in cif_files]
 
         # Check that output files are properly stored.
         with tempfile.TemporaryDirectory() as dir_path:
             voxels_from_files(cif_files, out_pathname=dir_path, grid_size=grid_size)
 
             voxels = np.load(f'{dir_path}/voxels.npy', mmap_mode='r')
-            stored_names = get_names(f'{dir_path}/names.json')
+            stored_names = load_json(f'{dir_path}/names.json')
 
             self.assertEqual(voxels.shape, (n_files, grid_size, grid_size, grid_size))
             self.assertEqual(names, stored_names)
 
     def test_voxels_from_dir(self):
         # The cif_dir contains 2 corrupted .cif files.
         cif_dir = 'tests/CIFs'
@@ -122,15 +122,15 @@
 
         names = [Path(i).stem for i in cif_names]
 
         with tempfile.TemporaryDirectory() as dir_path:
             voxels_from_dir(cif_dir, dir_path, grid_size=grid_size)
 
             voxels = np.load(f'{dir_path}/voxels.npy', mmap_mode='r')
-            stored_names = get_names(f'{dir_path}/names.json')
+            stored_names = load_json(f'{dir_path}/names.json')
 
             self.assertEqual(voxels.shape, (n_files, grid_size, grid_size, grid_size))
             self.assertEqual(names, stored_names)
 
             # Check that corrupted .cif files aren't processed.
             n_bad_voxels = sum([np.all(x == 0) for x in voxels])
             self.assertEqual(n_bad_files, n_bad_voxels)
@@ -141,18 +141,18 @@
 
         with tempfile.TemporaryDirectory() as dir_path:
             voxels_from_dir(cif_dir, dir_path, grid_size=grid_size)
             
             batch_clean(dir_path)
 
             voxels = np.load(f'{dir_path}/voxels.npy', mmap_mode='r')
-            names = get_names(f'{dir_path}/names.json')
+            names = load_json(f'{dir_path}/names.json')
 
             clean_voxels = np.load(f'{dir_path}/clean_voxels.npy', mmap_mode='r')
-            clean_names = get_names(f'{dir_path}/clean_names.json')
+            clean_names = load_json(f'{dir_path}/clean_names.json')
 
             # Get the indices of filled voxels.
             filled_idx = [i for i, x in enumerate(voxels) if not np.all(x == 0)]
 
             # Check that the voxels have been cleaned.
             self.assertTrue(np.all(voxels[filled_idx] == clean_voxels))
```

