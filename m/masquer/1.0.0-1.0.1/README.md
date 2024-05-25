# Comparing `tmp/masquer-1.0.0.tar.gz` & `tmp/masquer-1.0.1.tar.gz`

## Comparing `masquer-1.0.0.tar` & `masquer-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/__about__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/__init__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/utils/__init__.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/utils/assets.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/utils/response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/utils/select.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 masquer-1.0.0/src/masquerade/utils/validate.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 masquer-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 masquer-1.0.0/LICENSE
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 masquer-1.0.0/README.md
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 masquer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 masquer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/__about__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/utils/__init__.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/utils/assets.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/utils/response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/utils/select.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 masquer-1.0.1/src/masquer/utils/validate.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 masquer-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 masquer-1.0.1/LICENSE
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 masquer-1.0.1/README.md
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 masquer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 masquer-1.0.1/PKG-INFO
```

### Comparing `masquer-1.0.0/src/masquerade/app.py` & `masquer-1.0.1/src/masquer/app.py`

 * *Files identical despite different names*

### Comparing `masquer-1.0.0/src/masquerade/utils/assets.py` & `masquer-1.0.1/src/masquer/utils/assets.py`

 * *Files identical despite different names*

### Comparing `masquer-1.0.0/src/masquerade/utils/response.py` & `masquer-1.0.1/src/masquer/utils/response.py`

 * *Files identical despite different names*

### Comparing `masquer-1.0.0/.gitignore` & `masquer-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `masquer-1.0.0/LICENSE` & `masquer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `masquer-1.0.0/README.md` & `masquer-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Masquerade
+# Masquer
 
-[![GitHub Actions Workflow Status](https://github.com/essteer/masquerade/actions/workflows/test.yaml/badge.svg)](https://github.com/essteer/masquerade/actions/workflows/test.yaml)
-![](https://img.shields.io/badge/Python-3.9_|_3.10_|_3.11_|_3.12-3776AB.svg?style=flat&logo=Python&logoColor=white)
+[![GitHub Actions Workflow Status](https://github.com/essteer/masquer/actions/workflows/test.yaml/badge.svg)](https://github.com/essteer/masquer/actions/workflows/test.yaml)
+[![PyPI - Version](https://img.shields.io/badge/PyPI-v1.0.1-3775A9.svg?style=flat&logo=PyPI&logoColor=white)](https://pypi.org/project/masquer/)
+[![Python - Version](https://img.shields.io/badge/Python-3.9_|_3.10_|_3.11_|_3.12-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://pypi.org/project/masquer/)
 
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 A tool to generate random user-agent and referer data for GET requests.
 
 ## Overview
 
-Use `masquerade` to obtain any combination of a random user-agent, referer or header data template, then use this with a library like [`requests`](https://github.com/psf/requests) to control the session data you send to other services.
+Use `masquer` to obtain any combination of a random user-agent, referer or header data template, then use this with a library like [`requests`](https://github.com/psf/requests) to control the session data you send to other services.
 
 The user-agent data is drawn from [this list](https://www.useragents.me/) of the most common desktop user-agents, and referer data is taken from [this list](https://gs.statcounter.com/search-engine-market-share/desktop/worldwide) of search engines with the largest global market share.
 
 Weighted random selections are made from those lists to approximate authentic header data patterns.
 
 A basic header template with common attributes — including the recommended [`"Upgrade-Insecure-Requests": "1"`](https://stackoverflow.com/questions/31950470/what-is-the-upgrade-insecure-requests-http-header/32003517#32003517) — is also provided and defaults to the most common referer and user-agent data from the above lists.
 
@@ -24,34 +25,36 @@
 
 Controlling header data in this way can help to preserve privacy and hinder third-party tracking behaviour, by blending part of your web profile with the most common configurations. 
 
 It does not provide anonymity — that is a much more complex topic, and the open-source [Privacy Guides](https://www.privacyguides.org/en/) are a good place to start.
 
 ## Installation
 
-To get hold of `masquerade` either install the package from PyPI into your project's virtual environment, or clone the GitHub repo for the full code base.
+To get hold of `masquer` either install the package from PyPI into your project's virtual environment, or clone the GitHub repo for the full code base.
 
 ### PyPI package
 
-Install the `masquerade` package from PyPI to retrieve just the tool with no extras.
+[![](https://img.shields.io/badge/PyPI-masquer-3775A9.svg?style=flat&logo=PyPI&logoColor=white)](https://pypi.org/project/masquer/)
 
-Activate your existing project's virtual environment, then download `masquerade` using a package manager. The below example uses [Astral's](https://astral.sh/blog/uv) `uv`; substitute `pip` by dropping "`uv`" or use another package manager as needed: 
+Install the `masquer` package from PyPI to retrieve just the tool with no extras.
+
+Activate your existing project's virtual environment, then download `masquer` using a package manager. The below example uses [Astral's](https://astral.sh/blog/uv) `uv`; substitute `pip` by dropping "`uv`" or use another package manager as needed: 
 
 ```console
 $ uv pip install masquer
 ```
 
 ### GitHub repo
 
-[![](https://img.shields.io/badge/GitHub-masquerade-181717.svg?flat&logo=GitHub&logoColor=white)](https://github.com/essteer/masquerade)
+[![](https://img.shields.io/badge/GitHub-masquer-181717.svg?flat&logo=GitHub&logoColor=white)](https://github.com/essteer/masquer)
 
-Clone the `masquerade` repo from GitHub for the full source code. The repo includes the JSON source files used to generate the header data, a script to sync the programme if updates are made to the JSON files, and a test suite.
+Clone the `masquer` repo from GitHub for the full source code. The repo includes the JSON source files used to generate the header data, a script to sync the programme if updates are made to the JSON files, and a test suite.
 
 ```console
-$ git clone git@github.com:essteer/masquerade
+$ git clone git@github.com:essteer/masquer
 ```
 
 The functional code within the package `src` directory has no dependencies beyond Python built-in modules. If you intend to make changes to your cloned version of the repo, you may optionally install the `project.optional-dependencies` declared in the `pyproject.toml` file.
 
 First create and activate a virtual environment — the below example uses [Astral's](https://astral.sh/blog/uv) `uv`; substitute `pip` or use another package manager as needed — then install the `dev` dependencies:
 
 ![](https://img.shields.io/badge/Linux-FCC624.svg?style=flat&logo=Linux&logoColor=black)
@@ -69,18 +72,18 @@
 $ uv venv
 $ .venv\Scripts\activate
 $ uv pip install hatchling==1.24.2 pre-commit==3.7.1 ruff==0.4.4
 ```
 
 ## Operation
 
-Interact with `masquerade` via the `masq` method:
+Interact with `masquer` via the `masq` method:
 
 ```python
-from masquerade import masq
+from masquer import masq
 ```
 
 The `masq` function accepts up to three boolean parameters:
 
 ```python
 useragent = masq(
   ua = True,  # user-agent, defaults to True
@@ -158,15 +161,15 @@
 
 ## Local development
 
 The following details will assist with making and testing changes to a cloned version of the repository.
 
 ### Updates
 
-The root directory includes `update.py`: if you make changes to the JSON assets stored in the `assets` directory, sync those changes with the `assets.py` file inside the `masquerade` package by running `update.py` from the terminal:
+The root directory includes `update.py`: if you make changes to the JSON assets stored in the `assets` directory, sync those changes with the `assets.py` file inside the `masquer` package by running `update.py` from the terminal:
 
 ![](https://img.shields.io/badge/Linux-FCC624.svg?style=flat&logo=Linux&logoColor=black)
 ![](https://img.shields.io/badge/macOS-000000.svg?style=flat&logo=Apple&logoColor=white)
 
 ```console
 $ python3 update.py
 Asset update successful
@@ -177,15 +180,15 @@
 ```console
 $ python update.py
 Asset update successful
 ```
 
 ### Tests
 
-`masquerade` uses Python's in-built `unittest` module. 
+`masquer` uses Python's in-built `unittest` module. 
 
 To run the entire test suite using `discover`, or specify an individual test file from the `tests` directory — for example `test_assets.py` — run one of the following shell commands from the project `root` directory:
 
 ![](https://img.shields.io/badge/Linux-FCC624.svg?style=flat&logo=Linux&logoColor=black)
 ![](https://img.shields.io/badge/macOS-000000.svg?style=flat&logo=Apple&logoColor=white)
 
 ```console
```

### Comparing `masquer-1.0.0/pyproject.toml` & `masquer-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 dynamic = ["version"]
 description = "Weighted-random user-agent and referer data for GET requests"
 authors = [{ name = "Elliott Steer", email = "essteer@pm.me" }]
 dependencies = []
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 readme = "README.md"
-keywords = ["get", "header data", "requests", "user-agents"]
+keywords = ["requests", "header data", "user-agents"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -25,28 +25,28 @@
     "Programming Language :: Python :: 3.12",
 ]
 
 [project.optional-dependencies]
 dev = ["hatch==1.11.1", "hatchling==1.24.2", "pre-commit==3.7.1", "ruff==0.4.4"]
 
 [project.urls]
-documentation = "https://github.com/essteer/masquerade/blob/main/README.md"
-repository = "https://github.com/essteer/masquerade"
-issues = "https://github.com/essteer/masquerade/issues"
+documentation = "https://github.com/essteer/masquer/blob/main/README.md"
+repository = "https://github.com/essteer/masquer"
+issues = "https://github.com/essteer/masquer/issues"
 
 [tool.hatch.version]
-path = "src/masquerade/__about__.py"
+path = "src/masquer/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "src/masquerade/**/*.py"
+    "src/masquer/**/*.py"
 ]
 exclude = [
     "/.github",
     "*.json",
     "/tests",
     ".pre-commit-config.yaml",
     "update.py"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/masquerade"]
+packages = ["src/masquer"]
```

### Comparing `masquer-1.0.0/PKG-INFO` & `masquer-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: masquer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Weighted-random user-agent and referer data for GET requests
-Project-URL: documentation, https://github.com/essteer/masquerade/blob/main/README.md
-Project-URL: repository, https://github.com/essteer/masquerade
-Project-URL: issues, https://github.com/essteer/masquerade/issues
+Project-URL: documentation, https://github.com/essteer/masquer/blob/main/README.md
+Project-URL: repository, https://github.com/essteer/masquer
+Project-URL: issues, https://github.com/essteer/masquer/issues
 Author-email: Elliott Steer <essteer@pm.me>
 License: MIT License
         
         Copyright (c) 2024 Elliott Steer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,16 +24,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Keywords: get,header data,requests,user-agents
-Classifier: Development Status :: 4 - Beta
+Keywords: header data,requests,user-agents
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -43,29 +43,30 @@
 Provides-Extra: dev
 Requires-Dist: hatch==1.11.1; extra == 'dev'
 Requires-Dist: hatchling==1.24.2; extra == 'dev'
 Requires-Dist: pre-commit==3.7.1; extra == 'dev'
 Requires-Dist: ruff==0.4.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# Masquerade
+# Masquer
 
-[![GitHub Actions Workflow Status](https://github.com/essteer/masquerade/actions/workflows/test.yaml/badge.svg)](https://github.com/essteer/masquerade/actions/workflows/test.yaml)
-![](https://img.shields.io/badge/Python-3.9_|_3.10_|_3.11_|_3.12-3776AB.svg?style=flat&logo=Python&logoColor=white)
+[![GitHub Actions Workflow Status](https://github.com/essteer/masquer/actions/workflows/test.yaml/badge.svg)](https://github.com/essteer/masquer/actions/workflows/test.yaml)
+[![PyPI - Version](https://img.shields.io/badge/PyPI-v1.0.1-3775A9.svg?style=flat&logo=PyPI&logoColor=white)](https://pypi.org/project/masquer/)
+[![Python - Version](https://img.shields.io/badge/Python-3.9_|_3.10_|_3.11_|_3.12-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://pypi.org/project/masquer/)
 
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 A tool to generate random user-agent and referer data for GET requests.
 
 ## Overview
 
-Use `masquerade` to obtain any combination of a random user-agent, referer or header data template, then use this with a library like [`requests`](https://github.com/psf/requests) to control the session data you send to other services.
+Use `masquer` to obtain any combination of a random user-agent, referer or header data template, then use this with a library like [`requests`](https://github.com/psf/requests) to control the session data you send to other services.
 
 The user-agent data is drawn from [this list](https://www.useragents.me/) of the most common desktop user-agents, and referer data is taken from [this list](https://gs.statcounter.com/search-engine-market-share/desktop/worldwide) of search engines with the largest global market share.
 
 Weighted random selections are made from those lists to approximate authentic header data patterns.
 
 A basic header template with common attributes — including the recommended [`"Upgrade-Insecure-Requests": "1"`](https://stackoverflow.com/questions/31950470/what-is-the-upgrade-insecure-requests-http-header/32003517#32003517) — is also provided and defaults to the most common referer and user-agent data from the above lists.
 
@@ -73,34 +74,36 @@
 
 Controlling header data in this way can help to preserve privacy and hinder third-party tracking behaviour, by blending part of your web profile with the most common configurations. 
 
 It does not provide anonymity — that is a much more complex topic, and the open-source [Privacy Guides](https://www.privacyguides.org/en/) are a good place to start.
 
 ## Installation
 
-To get hold of `masquerade` either install the package from PyPI into your project's virtual environment, or clone the GitHub repo for the full code base.
+To get hold of `masquer` either install the package from PyPI into your project's virtual environment, or clone the GitHub repo for the full code base.
 
 ### PyPI package
 
-Install the `masquerade` package from PyPI to retrieve just the tool with no extras.
+[![](https://img.shields.io/badge/PyPI-masquer-3775A9.svg?style=flat&logo=PyPI&logoColor=white)](https://pypi.org/project/masquer/)
 
-Activate your existing project's virtual environment, then download `masquerade` using a package manager. The below example uses [Astral's](https://astral.sh/blog/uv) `uv`; substitute `pip` by dropping "`uv`" or use another package manager as needed: 
+Install the `masquer` package from PyPI to retrieve just the tool with no extras.
+
+Activate your existing project's virtual environment, then download `masquer` using a package manager. The below example uses [Astral's](https://astral.sh/blog/uv) `uv`; substitute `pip` by dropping "`uv`" or use another package manager as needed: 
 
 ```console
 $ uv pip install masquer
 ```
 
 ### GitHub repo
 
-[![](https://img.shields.io/badge/GitHub-masquerade-181717.svg?flat&logo=GitHub&logoColor=white)](https://github.com/essteer/masquerade)
+[![](https://img.shields.io/badge/GitHub-masquer-181717.svg?flat&logo=GitHub&logoColor=white)](https://github.com/essteer/masquer)
 
-Clone the `masquerade` repo from GitHub for the full source code. The repo includes the JSON source files used to generate the header data, a script to sync the programme if updates are made to the JSON files, and a test suite.
+Clone the `masquer` repo from GitHub for the full source code. The repo includes the JSON source files used to generate the header data, a script to sync the programme if updates are made to the JSON files, and a test suite.
 
 ```console
-$ git clone git@github.com:essteer/masquerade
+$ git clone git@github.com:essteer/masquer
 ```
 
 The functional code within the package `src` directory has no dependencies beyond Python built-in modules. If you intend to make changes to your cloned version of the repo, you may optionally install the `project.optional-dependencies` declared in the `pyproject.toml` file.
 
 First create and activate a virtual environment — the below example uses [Astral's](https://astral.sh/blog/uv) `uv`; substitute `pip` or use another package manager as needed — then install the `dev` dependencies:
 
 ![](https://img.shields.io/badge/Linux-FCC624.svg?style=flat&logo=Linux&logoColor=black)
@@ -118,18 +121,18 @@
 $ uv venv
 $ .venv\Scripts\activate
 $ uv pip install hatchling==1.24.2 pre-commit==3.7.1 ruff==0.4.4
 ```
 
 ## Operation
 
-Interact with `masquerade` via the `masq` method:
+Interact with `masquer` via the `masq` method:
 
 ```python
-from masquerade import masq
+from masquer import masq
 ```
 
 The `masq` function accepts up to three boolean parameters:
 
 ```python
 useragent = masq(
   ua = True,  # user-agent, defaults to True
@@ -207,15 +210,15 @@
 
 ## Local development
 
 The following details will assist with making and testing changes to a cloned version of the repository.
 
 ### Updates
 
-The root directory includes `update.py`: if you make changes to the JSON assets stored in the `assets` directory, sync those changes with the `assets.py` file inside the `masquerade` package by running `update.py` from the terminal:
+The root directory includes `update.py`: if you make changes to the JSON assets stored in the `assets` directory, sync those changes with the `assets.py` file inside the `masquer` package by running `update.py` from the terminal:
 
 ![](https://img.shields.io/badge/Linux-FCC624.svg?style=flat&logo=Linux&logoColor=black)
 ![](https://img.shields.io/badge/macOS-000000.svg?style=flat&logo=Apple&logoColor=white)
 
 ```console
 $ python3 update.py
 Asset update successful
@@ -226,15 +229,15 @@
 ```console
 $ python update.py
 Asset update successful
 ```
 
 ### Tests
 
-`masquerade` uses Python's in-built `unittest` module. 
+`masquer` uses Python's in-built `unittest` module. 
 
 To run the entire test suite using `discover`, or specify an individual test file from the `tests` directory — for example `test_assets.py` — run one of the following shell commands from the project `root` directory:
 
 ![](https://img.shields.io/badge/Linux-FCC624.svg?style=flat&logo=Linux&logoColor=black)
 ![](https://img.shields.io/badge/macOS-000000.svg?style=flat&logo=Apple&logoColor=white)
 
 ```console
```

