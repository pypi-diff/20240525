# Comparing `tmp/opvious-0.9.5.tar.gz` & `tmp/opvious-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opvious-0.9.5.tar", max compression
+gzip compressed data, was "opvious-0.9.6.tar", max compression
```

## Comparing `opvious-0.9.5.tar` & `opvious-0.9.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    10756 2023-04-07 19:54:09.822804 opvious-0.9.5/LICENSE
--rw-r--r--   0        0        0     3181 2023-04-07 19:54:09.822804 opvious-0.9.5/README.md
--rw-r--r--   0        0        0     2177 2023-04-07 19:54:09.822804 opvious-0.9.5/opvious/__init__.py
--rw-r--r--   0        0        0    23786 2023-04-07 19:54:09.822804 opvious-0.9.5/opvious/client.py
--rw-r--r--   0        0        0     1062 2023-04-07 19:54:09.822804 opvious-0.9.5/opvious/common.py
--rw-r--r--   0        0        0    15835 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/data.py
--rw-r--r--   0        0        0     2354 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/executors/__init__.py
--rw-r--r--   0        0        0     2348 2023-04-07 19:55:15.655073 opvious-0.9.5/opvious/executors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3521 2023-04-07 19:55:15.667073 opvious-0.9.5/opvious/executors/__pycache__/aiohttp.cpython-310.pyc
--rw-r--r--   0        0        0     9683 2023-04-07 19:55:15.655073 opvious-0.9.5/opvious/executors/__pycache__/common.cpython-310.pyc
--rw-r--r--   0        0        0     2762 2023-04-07 19:55:15.807073 opvious-0.9.5/opvious/executors/__pycache__/urllib.cpython-310.pyc
--rw-r--r--   0        0        0     4068 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/executors/aiohttp.py
--rw-r--r--   0        0        0     8942 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/executors/common.py
--rw-r--r--   0        0        0     2412 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/executors/pyodide.py
--rw-r--r--   0        0        0     2685 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/executors/urllib.py
--rw-r--r--   0        0        0        0 2023-04-07 19:54:09.826804 opvious-0.9.5/opvious/py.typed
--rw-r--r--   0        0        0      788 2023-04-07 19:54:09.826804 opvious-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 opvious-0.9.5/setup.py
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 opvious-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    10756 2023-04-07 21:32:16.543161 opvious-0.9.6/LICENSE
+-rw-r--r--   0        0        0     3181 2023-04-07 21:32:16.543161 opvious-0.9.6/README.md
+-rw-r--r--   0        0        0     2203 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/__init__.py
+-rw-r--r--   0        0        0    23969 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/client.py
+-rw-r--r--   0        0        0     1062 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/common.py
+-rw-r--r--   0        0        0    15835 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/data.py
+-rw-r--r--   0        0        0     2354 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/executors/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-07 21:33:17.499926 opvious-0.9.6/opvious/executors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3521 2023-04-07 21:33:17.507926 opvious-0.9.6/opvious/executors/__pycache__/aiohttp.cpython-310.pyc
+-rw-r--r--   0        0        0     9683 2023-04-07 21:33:17.503926 opvious-0.9.6/opvious/executors/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0        0        0     2762 2023-04-07 21:33:17.627927 opvious-0.9.6/opvious/executors/__pycache__/urllib.cpython-310.pyc
+-rw-r--r--   0        0        0     4068 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/executors/aiohttp.py
+-rw-r--r--   0        0        0     8942 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/executors/common.py
+-rw-r--r--   0        0        0     2412 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/executors/pyodide.py
+-rw-r--r--   0        0        0     2685 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/executors/urllib.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:32:16.543161 opvious-0.9.6/opvious/py.typed
+-rw-r--r--   0        0        0      788 2023-04-07 21:32:16.543161 opvious-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 opvious-0.9.6/setup.py
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 opvious-0.9.6/PKG-INFO
```

### Comparing `opvious-0.9.5/LICENSE` & `opvious-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/README.md` & `opvious-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/__init__.py` & `opvious-0.9.6/opvious/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.
 """
 
 import logging
 
-from .client import Client
+from .client import Client, Settings
 from .common import __version__
 from .executors import (
     ApiError,
     Executor,
     aiohttp_executor,
     default_executor,
     pyodide_executor,
@@ -73,14 +73,15 @@
     "Key",
     "KeyItem",
     "Label",
     "Notification",
     "Outcome",
     "Penalty",
     "Relaxation",
+    "Settings",
     "SolveInputs",
     "SolveOptions",
     "SolveOutputs",
     "SolveResponse",
     "SparseTensorArgument",
     "Summary",
     "Tensor",
```

### Comparing `opvious-0.9.5/opvious/client.py` & `opvious-0.9.6/opvious/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.
 """
 
 import backoff
 from datetime import datetime, timezone
+import enum
 import json
 import humanize
 import logging
 import os
 from typing import (
     Any,
     cast,
@@ -68,18 +69,19 @@
 
 _logger = logging.getLogger(__name__)
 
 
 _DEFAULT_DOMAIN = "beta.opvious.io"
 
 
-_TOKEN_EVAR = "OPVIOUS_TOKEN"
+class Settings(enum.Enum):
+    """Environment variable names"""
 
-
-_DOMAIN_EVAR = "OPVIOUS_DOMAIN"
+    TOKEN = "OPVIOUS_TOKEN"
+    DOMAIN = "OPVIOUS_DOMAIN"
 
 
 class Client:
     """Opvious API client"""
 
     def __init__(self, executor: Executor, api_url: str, hub_url: str):
         self._executor = executor
@@ -96,39 +98,44 @@
     @classmethod
     def from_token(cls, token: str, domain: Optional[str] = None) -> "Client":
         """
         Creates a client from an API token. You can use an empty token to
         create an unauthenticated client with limited functionality.
         """
         token = token.strip()
+        authorization = None
+        if token:
+            authorization = token if " " in token else f"Bearer {token}"
         api_url = f"https://api.{domain or _DEFAULT_DOMAIN}"
         return Client(
             executor=default_executor(
                 api_url=api_url,
-                authorization=token if " " in token else f"Bearer {token}",
+                authorization=authorization,
             ),
             api_url=api_url,
             hub_url=f"https://hub.{domain}",
         )
 
     @classmethod
     def from_environment(
         cls, env=os.environ, require_authenticated=False
     ) -> "Client":
         """
-        Creates a client from environment variables. If present, OPVIOUS_TOKEN
-        should contain a valid API token. OPVIOUS_DOMAIN can optionally be set
-        to use a custom domain.
+        Creates a client from environment variables. If present, the token
+        should contain a valid API token. A custom domain can optionally be
+        set.
         """
-        token = env.get(_TOKEN_EVAR, "")
+        token = env.get(Settings.TOKEN.value, "")
         if not token and require_authenticated:
             raise Exception(
-                f"Missing or empty {_TOKEN_EVAR} environment variable"
+                f"Missing or empty {Settings.TOKEN.value} environment variable"
             )
-        return Client.from_token(token=token, domain=env.get(_DOMAIN_EVAR))
+        return Client.from_token(
+            token=token, domain=env.get(Settings.DOMAIN.value)
+        )
 
     @property
     def authenticated(self):
         """
         Returns true if the client was created with a non-empty API token.
         """
         return self._executor.authenticated
```

### Comparing `opvious-0.9.5/opvious/common.py` & `opvious-0.9.6/opvious/common.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/data.py` & `opvious-0.9.6/opvious/data.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/executors/__init__.py` & `opvious-0.9.6/opvious/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/executors/__pycache__/__init__.cpython-310.pyc` & `opvious-0.9.6/opvious/executors/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 19:54:09 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e174 3064 3209 0000  o........t0d2...
+00000000: 6f0d 0d0a 0000 0000 e08b 3064 3209 0000  o.........0d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6700 6406 a201 5a0b 0902  m.Z...g.d...Z...
 00000070: 6414 6407 650c 6408 6503 650c 1900 6409  d.d.e.d.e.e...d.
```

### Comparing `opvious-0.9.5/opvious/executors/__pycache__/aiohttp.cpython-310.pyc` & `opvious-0.9.6/opvious/executors/__pycache__/aiohttp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 19:54:09 2023 UTC, .py size: 4068 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e174 3064 e40f 0000  o........t0d....
+00000000: 6f0d 0d0a 0000 0000 e08b 3064 e40f 0000  o.........0d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `opvious-0.9.5/opvious/executors/__pycache__/common.cpython-310.pyc` & `opvious-0.9.6/opvious/executors/__pycache__/common.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 19:54:09 2023 UTC, .py size: 8942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e174 3064 ee22 0000  o........t0d."..
+00000000: 6f0d 0d0a 0000 0000 e08b 3064 ee22 0000  o.........0d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6401 6402 6c0d 5a0e 6404  m.Z...d.d.l.Z.d.
```

### Comparing `opvious-0.9.5/opvious/executors/__pycache__/urllib.cpython-310.pyc` & `opvious-0.9.6/opvious/executors/__pycache__/urllib.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 19:54:09 2023 UTC, .py size: 2685 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e174 3064 7d0a 0000  o........t0d}...
+00000000: 6f0d 0d0a 0000 0000 e08b 3064 7d0a 0000  o.........0d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c06 6d07 5a07 6d08 5a08  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `opvious-0.9.5/opvious/executors/aiohttp.py` & `opvious-0.9.6/opvious/executors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/executors/common.py` & `opvious-0.9.6/opvious/executors/common.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/executors/pyodide.py` & `opvious-0.9.6/opvious/executors/pyodide.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/opvious/executors/urllib.py` & `opvious-0.9.6/opvious/executors/urllib.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.5/pyproject.toml` & `opvious-0.9.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opvious"
-version = "0.9.5"
+version = "0.9.6"
 description = "Opvious Python SDK"
 authors = ["Opvious Engineering <oss@opvious.io>"]
 readme = "README.md"
 repository = "https://github.com/opvious/sdk.py"
 packages = [{include = "opvious"}]
 
 [tool.poetry.dependencies]
```

### Comparing `opvious-0.9.5/setup.py` & `opvious-0.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['backoff>=2.2,<3.0', 'humanize>=4.4.0,<5.0.0', 'pandas>=1.4,<2.0']
 
 extras_require = \
 {'aio': ['aiohttp>=3.8,<4.0', 'Brotli>=1.0.9,<2.0.0']}
 
 setup_kwargs = {
     'name': 'opvious',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'Opvious Python SDK',
     'long_description': '# Opvious Python SDK  [![CI](https://github.com/opvious/sdk.py/actions/workflows/ci.yml/badge.svg)](https://github.com/opvious/sdk.py/actions/workflows/ci.yml) [![Pypi badge](https://badge.fury.io/py/opvious.svg)](https://pypi.python.org/pypi/opvious/)\n\nThis package provides a lightweight SDK for solving optimization models with the\n[Opvious API][api]. Its main features are:\n\n+ Seamless data import/export via native support for [`pandas`][pandas]\n+ Powerful built-in debugging capabilities: automatic infeasibility relaxation,\n  variable pinning, and more\n+ Non-blocking APIs for performant parallel calls\n\n\n## Quickstart\n\nFirst, install this package and have an API access token handy (these can be\ngenerated [here][token]).\n\n```sh\npip install opvious[aio] # aio is recommended for improved performance\n```\n\nWith these steps out of the way, you are ready to optimize!\n\n```python\nimport opvious\n\n# Instantiate an API client from an API token\nclient = opvious.Client.from_token(TOKEN)\n\n# Solve a simple portfolio selection optimization model\nresponse = await client.solve(\n    sources=[\n      r"""\n          We find an allocation of assets which minimizes risk while satisfying\n          a minimum expected return:\n\n          + A collection of assets: $\\S^d_{asset}: A$\n          + Covariances: $\\S^p_{covariance}: c \\in \\mathbb{R}^{A \\times A}$\n          + Expected return: $\\S^p_{expectedReturn}: m \\in \\mathbb{R}^A$\n          + Minimum desired return: $\\S^p_{desiredReturn}: r \\in \\mathbb{R}$\n\n          The only output is the allocation per asset\n          $\\S^v_{allocation}: \\alpha \\in [0,1]^A$ chosen to minimize risk:\n          $\\S^o_{risk}: \\min \\sum_{a, b \\in A} c_{a,b} \\alpha_a \\alpha_b$.\n\n          Subject to the following constraints:\n\n          + $\\S^c_{atLeastMinimumReturn}: \\sum_{a \\in A} m_a \\alpha_a \\geq r$\n          + $\\S^c_{totalAllocation}: \\sum_{a \\in A} \\alpha_a = 1$\n      """\n    ],\n    parameters={\n        "covariance": {\n            ("AAPL", "AAPL"): 0.08,\n            # ...\n        },\n        "expectedReturn": {\n            "AAPL": 0.07,\n            # ..\n        },\n        "desiredReturn": 0.05,\n    },\n)\n\n# Print the optimal allocation, if any\nif isinstance(response.outcome, opvious.FeasibleOutcome):\n  print(response.outputs.variable("allocation"))\nelse:\n  print(f"Problem was {response.status}.") # INFEASIBLE, UNBOUNDED\n```\n\n\n## Environments\n\nClients are compatible with Pyodide environments, for example [JupyterLite][]\nkernels. Simply install the package as usual in a notebook, omitting the `aio`\noptional dependencies:\n\n```python\nimport piplite\nawait piplite.install(\'opvious\')\n```\n\nIn other environments, prefer using the `aiohttp`-powered clients as they are\nmore performant (this is the default if the `aio` dependencies were specified).\n\n\n## Next steps\n\nThis SDK is focused on solving optimization models. For convenient access to the\nrest of Opvious API\'s functionality, consider using the [TypeScript SDK and\nCLI][cli].\n\n\n[api]: https://www.opvious.io\n[cli]: https://www.opvious.io/sdk.ts\n[JupyterLite]: https://jupyterlite.readthedocs.io/\n[token]: https://hub.beta.opvious.io/authorizations\n[pandas]: https://pandas.pydata.org\n',
     'author': 'Opvious Engineering',
     'author_email': 'oss@opvious.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/opvious/sdk.py',
```

### Comparing `opvious-0.9.5/PKG-INFO` & `opvious-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opvious
-Version: 0.9.5
+Version: 0.9.6
 Summary: Opvious Python SDK
 Home-page: https://github.com/opvious/sdk.py
 Author: Opvious Engineering
 Author-email: oss@opvious.io
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

