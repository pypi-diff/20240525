# Comparing `tmp/biobricks-0.3.6.tar.gz` & `tmp/biobricks-0.3.7.tar.gz`

## Comparing `biobricks-0.3.6.tar` & `biobricks-0.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 biobricks-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks.svg
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 biobricks-0.3.6/changelog.md
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 biobricks-0.3.6/requirements.txt
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 biobricks-0.3.6/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 biobricks-0.3.6/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 biobricks-0.3.6/.vscode/tasks.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/api.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/brick.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/checks.py
--rwxr-xr-x   0        0        0     5446 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/cli.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/config.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/downloader.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/dvc_fetcher.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/local_bb.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 biobricks-0.3.6/biobricks/logger.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 biobricks-0.3.6/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.3.6/docker/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 biobricks-0.3.6/tests/test_bricks.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 biobricks-0.3.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.3.6/LICENSE
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 biobricks-0.3.6/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 biobricks-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 biobricks-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 biobricks-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks.svg
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 biobricks-0.3.7/changelog.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 biobricks-0.3.7/requirements.txt
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 biobricks-0.3.7/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 biobricks-0.3.7/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 biobricks-0.3.7/.vscode/tasks.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/api.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/brick.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/checks.py
+-rwxr-xr-x   0        0        0     5446 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/cli.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/config.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/downloader.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/dvc_fetcher.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/local_bb.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 biobricks-0.3.7/biobricks/logger.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 biobricks-0.3.7/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.3.7/docker/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 biobricks-0.3.7/tests/test_bricks.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 biobricks-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.3.7/LICENSE
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 biobricks-0.3.7/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 biobricks-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 biobricks-0.3.7/PKG-INFO
```

### Comparing `biobricks-0.3.6/biobricks.svg` & `biobricks-0.3.7/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/.github/workflows/biobricks.yml` & `biobricks-0.3.7/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/.github/workflows/pypi_publish.yml` & `biobricks-0.3.7/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/.vscode/tasks.json` & `biobricks-0.3.7/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/api.py` & `biobricks-0.3.7/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/brick.py` & `biobricks-0.3.7/biobricks/brick.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/checks.py` & `biobricks-0.3.7/biobricks/checks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/cli.py` & `biobricks-0.3.7/biobricks/cli.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/config.py` & `biobricks-0.3.7/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/downloader.py` & `biobricks-0.3.7/biobricks/downloader.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/dvc_fetcher.py` & `biobricks-0.3.7/biobricks/dvc_fetcher.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/biobricks/local_bb.py` & `biobricks-0.3.7/biobricks/local_bb.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/docker/Dockerfile` & `biobricks-0.3.7/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/tests/test_bricks.py` & `biobricks-0.3.7/tests/test_bricks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/LICENSE` & `biobricks-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/README.md` & `biobricks-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `biobricks-0.3.6/pyproject.toml` & `biobricks-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="Thomas Luechtefeld", email="tom@insilica.co" },
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'click>=8.1.3',
```

### Comparing `biobricks-0.3.6/PKG-INFO` & `biobricks-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: biobricks
-Version: 0.3.6
+Version: 0.3.7
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Documentation, https://docs.biobricks.ai
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: Thomas Luechtefeld <tom@insilica.co>, "Jose A. Jaramillo" <jjv@utp.edu.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: click>=8.1.3
 Requires-Dist: cloup>=3.0.0
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: requests>=2.0.0
 Requires-Dist: tqdm>=4.0.0
 Description-Content-Type: text/markdown
```

