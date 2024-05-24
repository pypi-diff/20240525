# Comparing `tmp/matrix42sdk-3.0.2.tar.gz` & `tmp/matrix42sdk-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix42sdk-3.0.2.tar", max compression
+gzip compressed data, was "matrix42sdk-3.0.3.tar", max compression
```

## Comparing `matrix42sdk-3.0.2.tar` & `matrix42sdk-3.0.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1061 2021-06-26 12:33:45.914123 matrix42sdk-3.0.2/LICENSE
--rw-r--r--   0        0        0     6452 2021-07-03 17:49:55.807624 matrix42sdk-3.0.2/README.md
--rw-r--r--   0        0        0     3362 2021-07-03 17:47:10.878682 matrix42sdk-3.0.2/matrix42sdk/AuthNClient.py
--rw-r--r--   0        0        0      162 2021-06-26 13:56:43.212587 matrix42sdk-3.0.2/matrix42sdk/Exceptions.py
--rw-r--r--   0        0        0        0 2021-06-26 12:17:06.409400 matrix42sdk-3.0.2/matrix42sdk/__init__.py
--rw-r--r--   0        0        0      694 2021-06-26 13:47:53.680732 matrix42sdk-3.0.2/matrix42sdk/api_endpoints/__init__.py
--rw-r--r--   0        0        0    18334 2021-07-03 17:47:10.970682 matrix42sdk-3.0.2/matrix42sdk/api_endpoints/fragments.py
--rw-r--r--   0        0        0     7906 2021-07-03 17:46:34.830476 matrix42sdk-3.0.2/matrix42sdk/api_endpoints/objects.py
--rw-r--r--   0        0        0     1571 2021-07-03 17:46:55.334593 matrix42sdk-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     7374 2021-07-03 17:51:25.115736 matrix42sdk-3.0.2/setup.py
--rw-r--r--   0        0        0     7320 2021-07-03 17:51:25.117339 matrix42sdk-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2021-06-26 12:33:44.000000 matrix42sdk-3.0.3/LICENSE
+-rw-r--r--   0        0        0     5792 2024-05-24 21:55:20.261269 matrix42sdk-3.0.3/README.md
+-rw-r--r--   0        0        0     3362 2021-07-03 17:47:10.000000 matrix42sdk-3.0.3/matrix42sdk/AuthNClient.py
+-rw-r--r--   0        0        0      162 2021-06-26 13:56:42.000000 matrix42sdk-3.0.3/matrix42sdk/Exceptions.py
+-rw-r--r--   0        0        0        0 2021-06-26 12:17:06.000000 matrix42sdk-3.0.3/matrix42sdk/__init__.py
+-rw-r--r--   0        0        0      694 2021-06-26 13:47:52.000000 matrix42sdk-3.0.3/matrix42sdk/api_endpoints/__init__.py
+-rw-r--r--   0        0        0    18334 2021-07-03 17:47:10.000000 matrix42sdk-3.0.3/matrix42sdk/api_endpoints/fragments.py
+-rw-r--r--   0        0        0     7906 2021-07-03 17:46:34.000000 matrix42sdk-3.0.3/matrix42sdk/api_endpoints/objects.py
+-rw-r--r--   0        0        0     1601 2024-05-24 22:07:33.131682 matrix42sdk-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6820 1970-01-01 00:00:00.000000 matrix42sdk-3.0.3/PKG-INFO
```

### Comparing `matrix42sdk-3.0.2/LICENSE` & `matrix42sdk-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix42sdk-3.0.2/README.md` & `matrix42sdk-3.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # Python 3 Matrix42 SDK for Enterprise Service Management (ESM) tool
 
-[![Quality gate](https://sonarcloud.io/api/project_badges/quality_gate?project=dmpe_matrix42sdk)](https://sonarcloud.io/dashboard?id=dmpe_matrix42sdk)
-
 "ERP for Software Asset Management"
 
 [![matrix42sdk package in my-feed feed in Azure Artifacts](https://feeds.dev.azure.com/johnmalc/2efa647f-e5a5-4720-835d-4fc45fde9432/_apis/public/Packaging/Feeds/0c65acb4-f8ae-4df6-9f17-9db0f7687350/Packages/313927f6-82a5-4f2b-9bb0-9b90bcf3cec2/Badge)](https://dev.azure.com/johnmalc/Matrix42SDK/_packaging?_a=package&feed=0c65acb4-f8ae-4df6-9f17-9db0f7687350&package=313927f6-82a5-4f2b-9bb0-9b90bcf3cec2&preferRelease=true)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=dmpe_matrix42sdk&metric=alert_status)](https://sonarcloud.io/dashboard?id=dmpe_matrix42sdk)
 [![Build Status](https://dev.azure.com/johnmalc/Matrix42SDK/_apis/build/status/dmpe.matrix42sdk?branchName=master)](https://dev.azure.com/johnmalc/Matrix42SDK/_build/latest?definitionId=10&branchName=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![GitHub](https://img.shields.io/github/license/dmpe/matrix42sdk)
 ![Pull Requests](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)
-![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/dmpe/matrix42sdk)
-![Requires.io](https://img.shields.io/requires/github/dmpe/matrix42sdk)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/dmpe/matrix42sdk.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/dmpe/matrix42sdk/alerts/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/dmpe/matrix42sdk)
 
 ## The background story
 
-As of July 2020, Matrix42 AG, a German company is offering a [Configuration Management Database (CMBD)](https://www.matrix42.com/en/digital-workspace-management/enterprise-service-management) - basically a competing product to ServiceNOW and many others like Microsoft Intune.
+As of July 2020, Matrix42 AG, a German company is offering a [Configuration Management Database (CMBD)](https://www.matrix42.com/en/enterprise-service-management) - basically a competing product to ServiceNOW and many others like Microsoft Intune.
 
 Their Angular based product can be installed on-prem and used as ITIL supporting tool for the company.
 
 It provides a REST API which this Python3+ SDK tries to cover.
 Unfortunately, Swagger support is currently not available which has led me to write this client package myself - becoming my first python3 client SDK.
 
 It shows - also due to learning Python OOP principles.
```

### Comparing `matrix42sdk-3.0.2/matrix42sdk/AuthNClient.py` & `matrix42sdk-3.0.3/matrix42sdk/AuthNClient.py`

 * *Files identical despite different names*

### Comparing `matrix42sdk-3.0.2/matrix42sdk/api_endpoints/__init__.py` & `matrix42sdk-3.0.3/matrix42sdk/api_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix42sdk-3.0.2/matrix42sdk/api_endpoints/fragments.py` & `matrix42sdk-3.0.3/matrix42sdk/api_endpoints/fragments.py`

 * *Files identical despite different names*

### Comparing `matrix42sdk-3.0.2/matrix42sdk/api_endpoints/objects.py` & `matrix42sdk-3.0.3/matrix42sdk/api_endpoints/objects.py`

 * *Files identical despite different names*

### Comparing `matrix42sdk-3.0.2/pyproject.toml` & `matrix42sdk-3.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "matrix42sdk"
-version = "3.0.2"
+version = "3.0.3"
 description = "Python SDK for Matrix42 Enterprise Service Management CMBD"
 authors = ["John Malc <cincenko@outlook.com>"]
 homepage = "https://github.com/dmpe/matrix42sdk"
-documentation = ""
+documentation = "https://github.com/dmpe/matrix42sdk"
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Internet :: WWW/HTTP",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8" #minimal
-requests = "^2"
-mypy = "0.*"
-pytest = "6.*"
+requests = "*"
+mypy = "*"
 
 [tool.poetry.dev-dependencies]
+pytest = "*"
 mock = "*"
 isort = {extras = ["pyproject"], version = "*"}
 black = {version = "*", allow-prereleases = true }
 pytest-cov = "*"
 pylint = "*"
 keyring = "*"
 artifacts-keyring = "*"
```

### Comparing `matrix42sdk-3.0.2/setup.py` & `matrix42sdk-3.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,186 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: matrix42sdk
+Version: 3.0.3
+Summary: Python SDK for Matrix42 Enterprise Service Management CMBD
+Home-page: https://github.com/dmpe/matrix42sdk
+License: MIT
+Author: John Malc
+Author-email: cincenko@outlook.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: mypy
+Requires-Dist: requests
+Project-URL: Documentation, https://github.com/dmpe/matrix42sdk
+Description-Content-Type: text/markdown
 
-packages = \
-['matrix42sdk', 'matrix42sdk.api_endpoints']
+# Python 3 Matrix42 SDK for Enterprise Service Management (ESM) tool
 
-package_data = \
-{'': ['*']}
+"ERP for Software Asset Management"
 
-install_requires = \
-['mypy<1.0.0', 'pytest>=6.0.0,<7.0.0', 'requests>=2,<3']
-
-setup_kwargs = {
-    'name': 'matrix42sdk',
-    'version': '3.0.2',
-    'description': 'Python SDK for Matrix42 Enterprise Service Management CMBD',
-    'long_description': '# Python 3 Matrix42 SDK for Enterprise Service Management (ESM) tool\n\n[![Quality gate](https://sonarcloud.io/api/project_badges/quality_gate?project=dmpe_matrix42sdk)](https://sonarcloud.io/dashboard?id=dmpe_matrix42sdk)\n\n"ERP for Software Asset Management"\n\n[![matrix42sdk package in my-feed feed in Azure Artifacts](https://feeds.dev.azure.com/johnmalc/2efa647f-e5a5-4720-835d-4fc45fde9432/_apis/public/Packaging/Feeds/0c65acb4-f8ae-4df6-9f17-9db0f7687350/Packages/313927f6-82a5-4f2b-9bb0-9b90bcf3cec2/Badge)](https://dev.azure.com/johnmalc/Matrix42SDK/_packaging?_a=package&feed=0c65acb4-f8ae-4df6-9f17-9db0f7687350&package=313927f6-82a5-4f2b-9bb0-9b90bcf3cec2&preferRelease=true)\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=dmpe_matrix42sdk&metric=alert_status)](https://sonarcloud.io/dashboard?id=dmpe_matrix42sdk)\n[![Build Status](https://dev.azure.com/johnmalc/Matrix42SDK/_apis/build/status/dmpe.matrix42sdk?branchName=master)](https://dev.azure.com/johnmalc/Matrix42SDK/_build/latest?definitionId=10&branchName=master)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![GitHub](https://img.shields.io/github/license/dmpe/matrix42sdk)\n![Pull Requests](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)\n![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/dmpe/matrix42sdk)\n![Requires.io](https://img.shields.io/requires/github/dmpe/matrix42sdk)\n[![Total alerts](https://img.shields.io/lgtm/alerts/g/dmpe/matrix42sdk.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/dmpe/matrix42sdk/alerts/)\n![GitHub repo size](https://img.shields.io/github/repo-size/dmpe/matrix42sdk)\n\n## The background story\n\nAs of July 2020, Matrix42 AG, a German company is offering a [Configuration Management Database (CMBD)](https://www.matrix42.com/en/digital-workspace-management/enterprise-service-management) - basically a competing product to ServiceNOW and many others like Microsoft Intune.\n\nTheir Angular based product can be installed on-prem and used as ITIL supporting tool for the company.\n\nIt provides a REST API which this Python3+ SDK tries to cover.\nUnfortunately, Swagger support is currently not available which has led me to write this client package myself - becoming my first python3 client SDK.\n\nIt shows - also due to learning Python OOP principles.\n\n### Documentation of Rest API\n\n- <https://help.matrix42.com/030_DWP/030_INT> Intro\n- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations> How to use the API\n- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Matrix42_Web_Services_API> Matrix42 Approach to the API\n- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Web_Services%3A_Authentication_types> Example of AuthN\n- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Web_Services_tokens%3A_Generate_API_Token> Generate API Token\n\nSetting up the Sphinx auto-generate documentation:\n\n- <https://samnicholls.net/2016/06/15/how-to-sphinx-readthedocs/>\n\n# What works and what does not?\n\nWorks:\n\n- get and put (i.e. update) fragment\n\nUse Cases:\n\n- updating CI version numbers\n\nSemi/or not working:\n\n- creating fragment was not tested, but is implemented as a Rest API call\n- get and put object -> here not tested extensively and one must expect bugs\n\n# Testing\n\nWithout having a Matrix42 ESM portal which allows API access and is publicly available for unlimited use,\nthe only option how to test this library is to use **your** own ESM portal installation (be it in public cloud or on prem).\nHence the need to use your own API keys, etc.\n\nFrom this follows that this library cannot - as of now - include more python tests, at least not publicly available.\nIt is my recommendation to write your `own, private tests` and report issues here.\n\nSorry for inconvenience!\n\n# Usage\n\n## Python 3 - Simple Testing\n\nUsing `requests` you can call\n\n```\nimport requests\n\nurl = "https://xxxx/m42Services/api/ApiToken/GenerateAccessTokenFromApiToken/"\n\npayload = {}\nheaders = {\n  \'Content-Type\': \'application/json\',\n  \'Authorization\': \'Bearer the \'short\' version of bearer token generated from Administration Panel in the GUI\'\n}\n\nresponse = requests.request("POST", url, headers=headers, data = payload, verify = False)\n\nprint(response.text.encode(\'utf8\'))\n\n# only then start using proper API requests\nimport requests\n\nurl = "https://xxxx/m42Services/api/data/fragments/Ud_SoftwareproduktVersionClassBase/775c82cf-d243-4bfb-a1b2-f3edad93c826"\n\npayload = {}\nheaders = {\n  \'Authorization\': \'Bearer "output of the previous requests "RawToken" \'\n}\n\nresponse = requests.request("GET", url, headers=headers, data = payload)\n\nprint(response.text.encode(\'utf8\'))\n```\n## Matrix42 SDK for Python\n\nTo use Matrix42 SDK, first decide which authN approach you are going to use.\n\nFor a **basic**, create a `Matrix42RestClient` object by using your (or any other matrix42 CMBD) account:\n\n```{python}\nimport matrix42sdk\nfrom matrix42sdk import Matrix42RestClient\nfrom matrix42sdk.api_endpoints import *\n```\n\nFor using `Access/API Tokens`, you can set your `MATRIX42SDK_API_TOKEN` via a shell (**higher priority**):\n\n```{shell}\nexport MATRIX42_URL="xxx"\nexport MATRIX42SDK_API_TOKEN="xxx"\n```\n\nand then:\n\n```{python3}\nmat = api_endpoints.fragments.FragmentsDataService()\n```\n\nThen to [get a fragment for a specific CI](https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Public_API_reference_documentation/Fragments_Data_Service%3A_Get_Fragment_data), insert correct parameters according to the documentation:\n\n```\nJUPYTERLAB_ID_FRAG = "8c51cfff-bf16-452e-8d2c-527cc25518c3"\nSYS_ENTITY = "SPSSoftwareType"\nfull_ci_frg = mat.get_fragement(SYS_FRAGEMENT, JUPYTERLAB_ID_FRAG)\n```\n\n## Documentation\n\nWe use <https://sphinx-rtd-theme.readthedocs.io/> and <https://www.sphinx-doc.org/en/master/>\n\n```\ncd docs\nsphinx-apidoc -o source ../matrix42sdk\nmake html\n```\n\n# Building this package yourself\n\nThis package is being build on Azure DevOps services:\n\n<https://dev.azure.com/johnmalc/Matrix42SDK/_build>\n\nand further uses SonarCloud:\n\n<https://sonarcloud.io/dashboard?id=dmpe_matrix42sdk>\n\nUse to install package from non-PyPI feed (the azure one):\n\n```\npip3 install --index https://pkgs.dev.azure.com/johnmalc/Matrix42SDK/_packaging/my-feed/pypi/simple/ matrix42sdk\n```\n\n## PyPI\n\n```\npoetry build\n```\n',
-    'author': 'John Malc',
-    'author_email': 'cincenko@outlook.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/dmpe/matrix42sdk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+[![matrix42sdk package in my-feed feed in Azure Artifacts](https://feeds.dev.azure.com/johnmalc/2efa647f-e5a5-4720-835d-4fc45fde9432/_apis/public/Packaging/Feeds/0c65acb4-f8ae-4df6-9f17-9db0f7687350/Packages/313927f6-82a5-4f2b-9bb0-9b90bcf3cec2/Badge)](https://dev.azure.com/johnmalc/Matrix42SDK/_packaging?_a=package&feed=0c65acb4-f8ae-4df6-9f17-9db0f7687350&package=313927f6-82a5-4f2b-9bb0-9b90bcf3cec2&preferRelease=true)
+[![Build Status](https://dev.azure.com/johnmalc/Matrix42SDK/_apis/build/status/dmpe.matrix42sdk?branchName=master)](https://dev.azure.com/johnmalc/Matrix42SDK/_build/latest?definitionId=10&branchName=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![GitHub](https://img.shields.io/github/license/dmpe/matrix42sdk)
+![Pull Requests](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)
+![GitHub repo size](https://img.shields.io/github/repo-size/dmpe/matrix42sdk)
+
+## The background story
+
+As of July 2020, Matrix42 AG, a German company is offering a [Configuration Management Database (CMBD)](https://www.matrix42.com/en/enterprise-service-management) - basically a competing product to ServiceNOW and many others like Microsoft Intune.
+
+Their Angular based product can be installed on-prem and used as ITIL supporting tool for the company.
+
+It provides a REST API which this Python3+ SDK tries to cover.
+Unfortunately, Swagger support is currently not available which has led me to write this client package myself - becoming my first python3 client SDK.
+
+It shows - also due to learning Python OOP principles.
+
+### Documentation of Rest API
+
+- <https://help.matrix42.com/030_DWP/030_INT> Intro
+- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations> How to use the API
+- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Matrix42_Web_Services_API> Matrix42 Approach to the API
+- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Web_Services%3A_Authentication_types> Example of AuthN
+- <https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Web_Services_tokens%3A_Generate_API_Token> Generate API Token
+
+Setting up the Sphinx auto-generate documentation:
+
+- <https://samnicholls.net/2016/06/15/how-to-sphinx-readthedocs/>
+
+# What works and what does not?
+
+Works:
+
+- get and put (i.e. update) fragment
+
+Use Cases:
+
+- updating CI version numbers
+
+Semi/or not working:
+
+- creating fragment was not tested, but is implemented as a Rest API call
+- get and put object -> here not tested extensively and one must expect bugs
+
+# Testing
+
+Without having a Matrix42 ESM portal which allows API access and is publicly available for unlimited use,
+the only option how to test this library is to use **your** own ESM portal installation (be it in public cloud or on prem).
+Hence the need to use your own API keys, etc.
+
+From this follows that this library cannot - as of now - include more python tests, at least not publicly available.
+It is my recommendation to write your `own, private tests` and report issues here.
+
+Sorry for inconvenience!
+
+# Usage
+
+## Python 3 - Simple Testing
+
+Using `requests` you can call
+
+```
+import requests
+
+url = "https://xxxx/m42Services/api/ApiToken/GenerateAccessTokenFromApiToken/"
+
+payload = {}
+headers = {
+  'Content-Type': 'application/json',
+  'Authorization': 'Bearer the 'short' version of bearer token generated from Administration Panel in the GUI'
+}
+
+response = requests.request("POST", url, headers=headers, data = payload, verify = False)
+
+print(response.text.encode('utf8'))
+
+# only then start using proper API requests
+import requests
+
+url = "https://xxxx/m42Services/api/data/fragments/Ud_SoftwareproduktVersionClassBase/775c82cf-d243-4bfb-a1b2-f3edad93c826"
+
+payload = {}
+headers = {
+  'Authorization': 'Bearer "output of the previous requests "RawToken" '
 }
 
+response = requests.request("GET", url, headers=headers, data = payload)
+
+print(response.text.encode('utf8'))
+```
+## Matrix42 SDK for Python
+
+To use Matrix42 SDK, first decide which authN approach you are going to use.
+
+For a **basic**, create a `Matrix42RestClient` object by using your (or any other matrix42 CMBD) account:
+
+```{python}
+import matrix42sdk
+from matrix42sdk import Matrix42RestClient
+from matrix42sdk.api_endpoints import *
+```
+
+For using `Access/API Tokens`, you can set your `MATRIX42SDK_API_TOKEN` via a shell (**higher priority**):
+
+```{shell}
+export MATRIX42_URL="xxx"
+export MATRIX42SDK_API_TOKEN="xxx"
+```
+
+and then:
+
+```{python3}
+mat = api_endpoints.fragments.FragmentsDataService()
+```
+
+Then to [get a fragment for a specific CI](https://help.matrix42.com/030_DWP/030_INT/Business_Processes_and_API_Integrations/Public_API_reference_documentation/Fragments_Data_Service%3A_Get_Fragment_data), insert correct parameters according to the documentation:
+
+```
+JUPYTERLAB_ID_FRAG = "8c51cfff-bf16-452e-8d2c-527cc25518c3"
+SYS_ENTITY = "SPSSoftwareType"
+full_ci_frg = mat.get_fragement(SYS_FRAGEMENT, JUPYTERLAB_ID_FRAG)
+```
+
+## Documentation
+
+We use <https://sphinx-rtd-theme.readthedocs.io/> and <https://www.sphinx-doc.org/en/master/>
+
+```
+cd docs
+sphinx-apidoc -o source ../matrix42sdk
+make html
+```
+
+# Building this package yourself
+
+This package is being build on Azure DevOps services:
+
+<https://dev.azure.com/johnmalc/Matrix42SDK/_build>
+
+and further uses SonarCloud:
+
+<https://sonarcloud.io/dashboard?id=dmpe_matrix42sdk>
+
+Use to install package from non-PyPI feed (the azure one):
+
+```
+pip3 install --index https://pkgs.dev.azure.com/johnmalc/Matrix42SDK/_packaging/my-feed/pypi/simple/ matrix42sdk
+```
+
+## PyPI
+
+```
+poetry build
+```
 
-setup(**setup_kwargs)
```

