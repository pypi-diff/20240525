# Comparing `tmp/opaqueprompts-0.1.0.tar.gz` & `tmp/opaqueprompts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opaqueprompts-0.1.0.tar", last modified: Wed Sep 20 23:19:47 2023, max compression
+gzip compressed data, was "opaqueprompts-0.1.1.tar", last modified: Fri May 24 18:34:06 2024, max compression
```

## Comparing `opaqueprompts-0.1.0.tar` & `opaqueprompts-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ggroode   (1000) ggroode   (1000)        0 2023-09-20 23:19:47.119861 opaqueprompts-0.1.0/
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)    10995 2023-08-21 23:05:40.000000 opaqueprompts-0.1.0/LICENSE
--rw-r--r--   0 ggroode   (1000) ggroode   (1000)    14140 2023-09-20 23:19:47.119861 opaqueprompts-0.1.0/PKG-INFO
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)      759 2023-08-31 00:48:04.000000 opaqueprompts-0.1.0/README.md
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)      913 2023-09-20 23:19:05.000000 opaqueprompts-0.1.0/pyproject.toml
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)       38 2023-09-20 23:19:47.119861 opaqueprompts-0.1.0/setup.cfg
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)      447 2023-08-31 00:48:04.000000 opaqueprompts-0.1.0/setup.py
-drwxrwxr-x   0 ggroode   (1000) ggroode   (1000)        0 2023-09-20 23:19:47.115861 opaqueprompts-0.1.0/src/
-drwxrwxr-x   0 ggroode   (1000) ggroode   (1000)        0 2023-09-20 23:19:47.119861 opaqueprompts-0.1.0/src/opaqueprompts/
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)      208 2023-08-31 00:48:04.000000 opaqueprompts-0.1.0/src/opaqueprompts/__init__.py
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)      586 2023-08-31 00:48:04.000000 opaqueprompts-0.1.0/src/opaqueprompts/authentication.py
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)     1279 2023-09-07 18:37:10.000000 opaqueprompts-0.1.0/src/opaqueprompts/configuration.py
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)     7033 2023-09-20 23:19:05.000000 opaqueprompts-0.1.0/src/opaqueprompts/opaqueprompts_service.py
-drwxrwxr-x   0 ggroode   (1000) ggroode   (1000)        0 2023-09-20 23:19:47.119861 opaqueprompts-0.1.0/src/opaqueprompts.egg-info/
--rw-r--r--   0 ggroode   (1000) ggroode   (1000)    14140 2023-09-20 23:19:47.000000 opaqueprompts-0.1.0/src/opaqueprompts.egg-info/PKG-INFO
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)      389 2023-09-20 23:19:47.000000 opaqueprompts-0.1.0/src/opaqueprompts.egg-info/SOURCES.txt
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)        1 2023-09-20 23:19:47.000000 opaqueprompts-0.1.0/src/opaqueprompts.egg-info/dependency_links.txt
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)       28 2023-09-20 23:19:47.000000 opaqueprompts-0.1.0/src/opaqueprompts.egg-info/requires.txt
--rw-rw-r--   0 ggroode   (1000) ggroode   (1000)       14 2023-09-20 23:19:47.000000 opaqueprompts-0.1.0/src/opaqueprompts.egg-info/top_level.txt
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    10995 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/LICENSE
+-rw-r--r--   0 hegatta   (1000) hegatta   (1000)    14140 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/PKG-INFO
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      759 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/README.md
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      913 2024-05-24 18:33:15.000000 opaqueprompts-0.1.1/pyproject.toml
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/setup.cfg
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      447 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/setup.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.867674 opaqueprompts-0.1.1/src/
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.867674 opaqueprompts-0.1.1/src/opaqueprompts/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      208 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      587 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/authentication.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1280 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/configuration.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     7350 2024-05-24 18:13:37.000000 opaqueprompts-0.1.1/src/opaqueprompts/opaqueprompts_service.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:34:06.871674 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/
+-rw-r--r--   0 hegatta   (1000) hegatta   (1000)    14140 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/PKG-INFO
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      389 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/SOURCES.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        1 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/dependency_links.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       28 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/requires.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       14 2024-05-24 18:34:06.000000 opaqueprompts-0.1.1/src/opaqueprompts.egg-info/top_level.txt
```

### Comparing `opaqueprompts-0.1.0/LICENSE` & `opaqueprompts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.0/PKG-INFO` & `opaqueprompts-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opaqueprompts
-Version: 0.1.0
+Version: 0.1.1
 Summary: The client-side SDK for OpaquePrompts, a privacy layer that enables applications to wrap external provider calls with a sanitization mechanism that hides sensitive inputs via an attested trusted execution environment.
 Author-email: Opaque Systems <pypi@opaque.co>
 License:                                 Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Keywords: confidential,llm,ai,generative,security,privacy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyatls>=0.0.3
+Requires-Dist: pyatls>=0.0.5
 Requires-Dist: requests>=2.0
 
 # OpaquePrompts
 OpaquePrompts enables applications to leverage the power of language models while preserving user privacy. This repo contains the OpaquePrompts Python library, which provides a simple interface for interacting with the OpaquePrompts Service. More information about OpaquePrompts can be found in the [documentation](https://opaqueprompts.readthedocs.io/).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
```

### Comparing `opaqueprompts-0.1.0/README.md` & `opaqueprompts-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opaqueprompts-0.1.0/pyproject.toml` & `opaqueprompts-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "opaqueprompts"
-version = "0.1.0"
+version = "0.1.1"
 description = "The client-side SDK for OpaquePrompts, a privacy layer that enables applications to wrap external provider calls with a sanitization mechanism that hides sensitive inputs via an attested trusted execution environment."
 readme = "README.md"
 authors= [{ name = "Opaque Systems", email = "pypi@opaque.co" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 keywords = ["confidential", "llm", "ai", "generative", "security", "privacy"]
 dependencies = [
-    "pyatls >= 0.0.3",
+    "pyatls >= 0.0.5",
     "requests >= 2.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/opaque-systems/opaqueprompts-python"
 
 [build-system]
```

### Comparing `opaqueprompts-0.1.0/src/opaqueprompts/authentication.py` & `opaqueprompts-0.1.1/src/opaqueprompts/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module handles authentication logic for the opaqueprompts package.
 """
+
 import os
 
 API_KEY_ENV_VAR = "OPAQUEPROMPTS_API_KEY"
 
 
 def get_api_key() -> str:
     """
```

### Comparing `opaqueprompts-0.1.0/src/opaqueprompts/configuration.py` & `opaqueprompts-0.1.1/src/opaqueprompts/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module handles configuration logic for the opaqueprompts package.
 """
+
 import os
 from typing import Tuple
 
 # TODO: Once we have deployed the OpaquePrompts Service this should be
 # hardcoded to use that domain, as end users shouldn't need to configure
 # the domain name manually.
 SERVER_HOSTNAME_ENV_VAR = "OPAQUEPROMPTS_SERVER_HOSTNAME"
```

### Comparing `opaqueprompts-0.1.0/src/opaqueprompts/opaqueprompts_service.py` & `opaqueprompts-0.1.1/src/opaqueprompts/opaqueprompts_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
-This module exposes wrappers around API calls to the OpaquePrompts service.
+This module exposes wrappers around API calls to the Opaque Gateway service.
 """
+
 import json
 import os
 import threading
 from dataclasses import dataclass
 from http import HTTPStatus
 from http.client import HTTPException
 from importlib import metadata
@@ -20,14 +21,16 @@
 # Global requests session to leverage connection pooling to in turn avoid
 # establishing a new connection for each request to the service.
 _session: Optional[requests.Session] = None
 
 # Protects the global requests session when creating it for the first time.
 _session_lock: threading.Lock = threading.Lock()
 
+SERVER_ATLS_ENV_VAR = "OPAQUEPROMPTS_CLIENT_ATLS_ENABLED"
+
 
 @dataclass
 class SanitizeResponse:
     """
     Class representing the return value of the sanitize method
 
     Attributes
@@ -63,16 +66,16 @@
         up when errors occur.
     timeout : int, optional
         The number of seconds to wait until a request to the service times out.
 
     Returns
     -------
     SanitizeResponse
-        The anonymized version of input_texts without PII and a secret entropy
-        value.
+        The anonymized version of `input_texts` without PII, and a secret
+        entropy value.
     """
     response = _send_request_to_opaqueprompts_service(
         endpoint="sanitize",
         payload={"input_texts": input_texts},
         retries=retries,
         timeout=timeout,
     )
@@ -115,15 +118,15 @@
         up when errors occur.
     timeout : int, optional
         The number of seconds to wait until a request to the service times out.
 
     Returns
     -------
     DesanitizeResponse
-        The deanonymzied version of sanitized_text with PII added back in.
+        The de-anonymized version of `sanitized_text` with PII added back in.
     """
     response = _send_request_to_opaqueprompts_service(
         endpoint="desanitize",
         payload={
             "sanitized_text": sanitized_text,
             "secure_context": secure_context,
         },
@@ -166,42 +169,49 @@
         The response body returned by the request, only returned if the request
         was successful.
     """
 
     global _session
     global _session_lock
 
-    # This flag is used to disable aTLS for testing purposes.
-    # INTERNAL USE ONLY.
-    # It breaks the communication with the aTLS enabled server.
-    _client_atls_enabled = bool(
-        os.environ.get("OPAQUEPROMPTS_CLIENT_ATLS_ENABLED", True)
-    )
-    http_protocol = "httpa" if _client_atls_enabled else "http"
+    # TESTING USE ONLY!!!
+    # This environment variable is used to disable aTLS for testing purposes.
+    # If aTLS is disabled, this package will not be able to communicate with an
+    # aTLS-enabled endpoint.
+    atls_enabled_str: Union[None, str]
+    atls_enabled_str = os.environ.get(SERVER_ATLS_ENV_VAR)
+
+    if atls_enabled_str is None or atls_enabled_str.lower() == "true":
+        atls_enabled = True
+    elif atls_enabled_str.lower() == "false":
+        atls_enabled = False
+    else:
+        raise Exception(
+            f"Invalid value for {SERVER_ATLS_ENV_VAR}: {atls_enabled_str}"
+        )
+
+    scheme = "httpa" if atls_enabled else "http"
 
     with _session_lock:
         if _session is None:
             _session = requests.Session()
-            if _client_atls_enabled:
-                _session.mount(
-                    "httpa://", HTTPAAdapter(_get_default_validators())
-                )
+            _session.mount("httpa://", HTTPAAdapter(_get_default_validators()))
 
     api_key = get_api_key()
     hostname, port = get_server_config()
 
     if retries is None:
         retries = 3
 
     conn_except: ConnectionError
     while retries > 0:
         try:
             response = _session.request(
                 "POST",
-                f"{http_protocol}://{hostname}:{port}/{endpoint}",
+                f"{scheme}://{hostname}:{port}/{endpoint}",
                 headers={
                     "Authorization": f"Bearer {api_key}",
                     "Client-Version": metadata.version("opaqueprompts"),
                 },
                 data=json.dumps(payload),
                 timeout=timeout,
             )
```

### Comparing `opaqueprompts-0.1.0/src/opaqueprompts.egg-info/PKG-INFO` & `opaqueprompts-0.1.1/src/opaqueprompts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opaqueprompts
-Version: 0.1.0
+Version: 0.1.1
 Summary: The client-side SDK for OpaquePrompts, a privacy layer that enables applications to wrap external provider calls with a sanitization mechanism that hides sensitive inputs via an attested trusted execution environment.
 Author-email: Opaque Systems <pypi@opaque.co>
 License:                                 Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Keywords: confidential,llm,ai,generative,security,privacy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyatls>=0.0.3
+Requires-Dist: pyatls>=0.0.5
 Requires-Dist: requests>=2.0
 
 # OpaquePrompts
 OpaquePrompts enables applications to leverage the power of language models while preserving user privacy. This repo contains the OpaquePrompts Python library, which provides a simple interface for interacting with the OpaquePrompts Service. More information about OpaquePrompts can be found in the [documentation](https://opaqueprompts.readthedocs.io/).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
```

