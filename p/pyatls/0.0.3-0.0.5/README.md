# Comparing `tmp/pyatls-0.0.3.tar.gz` & `tmp/pyatls-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatls-0.0.3.tar", last modified: Fri Sep  1 17:35:39 2023, max compression
+gzip compressed data, was "pyatls-0.0.5.tar", last modified: Fri May 24 18:27:30 2024, max compression
```

## Comparing `pyatls-0.0.3.tar` & `pyatls-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    10995 2023-08-21 20:19:12.000000 pyatls-0.0.3/LICENSE
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    18299 2023-09-01 17:35:39.783471 pyatls-0.0.3/PKG-INFO
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     5192 2023-09-01 17:33:28.000000 pyatls-0.0.3/README.md
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      781 2023-09-01 17:33:28.000000 pyatls-0.0.3/pyproject.toml
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2023-09-01 17:35:39.783471 pyatls-0.0.3/setup.cfg
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2023-08-21 20:19:12.000000 pyatls-0.0.3/setup.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      149 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/__init__.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     3780 2023-09-01 17:33:28.000000 pyatls-0.0.3/src/atls/atls_context.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     2078 2023-09-01 17:33:28.000000 pyatls-0.0.3/src/atls/httpa_connection.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/utils/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        0 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/utils/__init__.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1121 2023-09-01 17:33:28.000000 pyatls-0.0.3/src/atls/utils/_httpa_connection_shim.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/utils/requests/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       81 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/utils/requests/__init__.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     2335 2023-09-01 17:33:28.000000 pyatls-0.0.3/src/atls/utils/requests/adapter.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/utils/urllib3/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      138 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/utils/urllib3/__init__.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1416 2023-09-01 17:33:28.000000 pyatls-0.0.3/src/atls/utils/urllib3/patch.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/validators/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       73 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/validators/__init__.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/validators/azure/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        0 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/validators/azure/__init__.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/atls/validators/azure/aas/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      261 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/validators/azure/aas/__init__.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     7670 2023-08-31 19:22:01.000000 pyatls-0.0.3/src/atls/validators/azure/aas/aci_validator.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      639 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/validators/azure/aas/cvm_validator.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      264 2023-08-29 23:44:56.000000 pyatls-0.0.3/src/atls/validators/azure/aas/shared.py
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1843 2023-08-21 20:19:12.000000 pyatls-0.0.3/src/atls/validators/validator.py
-drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2023-09-01 17:35:39.783471 pyatls-0.0.3/src/pyatls.egg-info/
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    18299 2023-09-01 17:35:39.000000 pyatls-0.0.3/src/pyatls.egg-info/PKG-INFO
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      770 2023-09-01 17:35:39.000000 pyatls-0.0.3/src/pyatls.egg-info/SOURCES.txt
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        1 2023-09-01 17:35:39.000000 pyatls-0.0.3/src/pyatls.egg-info/dependency_links.txt
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       51 2023-09-01 17:35:39.000000 pyatls-0.0.3/src/pyatls.egg-info/requires.txt
--rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        5 2023-09-01 17:35:39.000000 pyatls-0.0.3/src/pyatls.egg-info/top_level.txt
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.906526 pyatls-0.0.5/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)    10995 2024-05-24 17:57:56.000000 pyatls-0.0.5/LICENSE
+-rw-r--r--   0 hegatta   (1000) hegatta   (1000)    18484 2024-05-24 18:27:30.906526 pyatls-0.0.5/PKG-INFO
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     5196 2024-05-24 17:57:56.000000 pyatls-0.0.5/README.md
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      838 2024-05-24 18:17:25.000000 pyatls-0.0.5/pyproject.toml
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2024-05-24 18:27:30.906526 pyatls-0.0.5/setup.cfg
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       38 2024-05-24 17:57:56.000000 pyatls-0.0.5/setup.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      149 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     4852 2024-05-24 18:17:25.000000 pyatls-0.0.5/src/atls/atls_context.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     2078 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/httpa_connection.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/utils/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/utils/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1121 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/utils/_httpa_connection_shim.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/utils/requests/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       81 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/utils/requests/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     2335 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/utils/requests/adapter.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/utils/urllib3/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      138 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/utils/urllib3/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1416 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/utils/urllib3/patch.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/validators/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       73 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/validators/__init__.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/validators/azure/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/validators/azure/__init__.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.902526 pyatls-0.0.5/src/atls/validators/azure/aas/
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      261 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/validators/azure/aas/__init__.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     8836 2024-05-24 18:17:25.000000 pyatls-0.0.5/src/atls/validators/azure/aas/aci_validator.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      639 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/validators/azure/aas/cvm_validator.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      264 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/validators/azure/aas/shared.py
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)     1843 2024-05-24 17:57:56.000000 pyatls-0.0.5/src/atls/validators/validator.py
+drwxrwxr-x   0 hegatta   (1000) hegatta   (1000)        0 2024-05-24 18:27:30.906526 pyatls-0.0.5/src/pyatls.egg-info/
+-rw-r--r--   0 hegatta   (1000) hegatta   (1000)    18484 2024-05-24 18:27:30.000000 pyatls-0.0.5/src/pyatls.egg-info/PKG-INFO
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)      770 2024-05-24 18:27:30.000000 pyatls-0.0.5/src/pyatls.egg-info/SOURCES.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        1 2024-05-24 18:27:30.000000 pyatls-0.0.5/src/pyatls.egg-info/dependency_links.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)       72 2024-05-24 18:27:30.000000 pyatls-0.0.5/src/pyatls.egg-info/requires.txt
+-rw-rw-r--   0 hegatta   (1000) hegatta   (1000)        5 2024-05-24 18:27:30.000000 pyatls-0.0.5/src/pyatls.egg-info/top_level.txt
```

### Comparing `pyatls-0.0.3/LICENSE` & `pyatls-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/PKG-INFO` & `pyatls-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatls
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Python package that implements Attested TLS (aTLS).
 Author-email: Opaque Systems <pypi@opaque.co>
 License:                                 Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,31 +202,37 @@
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
 Project-URL: Homepage, https://github.com/opaque-systems/atls-python
-Keywords: confidential,llm,tls,ssl,atls,attestation,security,privacy
+Keywords: atls,attestation,confidential,llm,privacy,security,ssl,tls
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
+Requires-Dist: PyJWT
+Requires-Dist: pyOpenSSL
+Requires-Dist: urllib3<2.1.0,>=2.0.0
+Provides-Extra: requests
+Requires-Dist: requests; extra == "requests"
 
 # Python aTLS Package
 
 An implementation of Attested TLS (aTLS) for Python.
 
 Supports the client-side handshake against a custom attester that issues JWT
 tokens via the Azure Attestation Service (AAS) running on Azure Container
 Instance (ACI) instances.
 
 For the moment, this package exists to support
-[`promptguard`](https://pypi.org/project/promptguard/), a confidential
+[`OpaquePrompts`](https://pypi.org/project/opaqueprompts/), a confidential
 information redaction service that runs in a Trusted Execution Environment
 (TEE).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
 
 **Note:** The server-side counterpart to this package is not yet public. If you
```

### Comparing `pyatls-0.0.3/README.md` & `pyatls-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 An implementation of Attested TLS (aTLS) for Python.
 
 Supports the client-side handshake against a custom attester that issues JWT
 tokens via the Azure Attestation Service (AAS) running on Azure Container
 Instance (ACI) instances.
 
 For the moment, this package exists to support
-[`promptguard`](https://pypi.org/project/promptguard/), a confidential
+[`OpaquePrompts`](https://pypi.org/project/opaqueprompts/), a confidential
 information redaction service that runs in a Trusted Execution Environment
 (TEE).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
 
 **Note:** The server-side counterpart to this package is not yet public. If you
```

### Comparing `pyatls-0.0.3/pyproject.toml` & `pyatls-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [project]
 name = "pyatls"
-version = "0.0.3"
+version = "0.0.5"
 description = "A Python package that implements Attested TLS (aTLS)."
 readme = "README.md"
 authors = [{ name = "Opaque Systems", email = "pypi@opaque.co" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 keywords = [
-    "confidential",
-    "llm",
-    "tls",
-    "ssl",
     "atls",
     "attestation",
-    "security",
+    "confidential",
+    "llm",
     "privacy",
+    "security",
+    "ssl",
+    "tls",
 ]
 dependencies = [
     "cryptography",
     "PyJWT",
     "pyOpenSSL",
     "urllib3 >= 2.0.0, < 2.1.0",
 ]
 
+[project.optional-dependencies]
+requests = ["requests"]
+
 [project.urls]
 Homepage = "https://github.com/opaque-systems/atls-python"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pyatls-0.0.3/src/atls/atls_context.py` & `pyatls-0.0.5/src/atls/atls_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import logging
 import secrets
 import socket
 import ssl
 import warnings
 from typing import List, Optional
 
 import OpenSSL.crypto
@@ -15,14 +16,16 @@
 # support custom certificate validation or switching to mbedTLS (and
 # contributing support for custom certificate validation there).
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 from atls.validators import Validator  # noqa: E402
 from urllib3.contrib.pyopenssl import PyOpenSSLContext  # noqa: E402
 from urllib3.contrib.pyopenssl import WrappedSocket  # noqa: E402
 
+logger = logging.getLogger(__name__)
+
 
 class ATLSContext(PyOpenSSLContext):
     """
     An SSL context that supports validation of aTLS certificates.
 
     Attention: Because this class manages the aTLS handshake's nonce, you must
     use different instances for different connections.
@@ -64,32 +67,59 @@
         x509: OpenSSL.crypto.X509,
         _err_no: int,
         _err_depth: int,
         _return_code: int,
     ) -> bool:
         """OpenSSL certificate validation callback"""
 
+        logger.info("Validating certificate...")
+
         peer_cert = x509.to_cryptography()
 
+        logger.info("Looking for a suitable validator...")
         for validator in self._validators:
             extension: Extension[ExtensionType]
             for extension in peer_cert.extensions:
                 if validator.accepts(extension.oid):
                     if not hasattr(extension.value, "value"):
                         continue
 
+                    logger.debug("Fetching certificate extension value...")
                     document = extension.value.value
+
+                    logger.debug("Fetching certificate public key...")
                     pub = peer_cert.public_key()
+
+                    logger.debug(
+                        "Fetching certificate SubjectPublicKeyInfo..."
+                    )
                     spki = pub.public_bytes(
                         Encoding.DER, PublicFormat.SubjectPublicKeyInfo
                     )
 
-                    if validator.validate(document, spki, self._nonce):
+                    logger.debug(
+                        "Calling into validator (validator: %s)...",
+                        validator.__class__,
+                    )
+
+                    result = validator.validate(document, spki, self._nonce)
+
+                    if result:
+                        logger.info(
+                            "Certificate validation succeeded (validator: %s)",
+                            validator.__class__,
+                        )
                         return True
 
+                    logger.error(
+                        "Certificate validation failed (validator: %s)",
+                        validator.__class__,
+                    )
+
+        logger.error("No validator found for certiticate")
         return False
 
     def wrap_socket(self, sock: socket.socket) -> WrappedSocket:
         # To perform aTLS over regular TLS, we use the Server Name Indication
         # extension to carry the nonce.
         sni = base64.encodebytes(self._nonce)
```

### Comparing `pyatls-0.0.3/src/atls/httpa_connection.py` & `pyatls-0.0.5/src/atls/httpa_connection.py`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/src/atls/utils/_httpa_connection_shim.py` & `pyatls-0.0.5/src/atls/utils/_httpa_connection_shim.py`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/src/atls/utils/requests/adapter.py` & `pyatls-0.0.5/src/atls/utils/requests/adapter.py`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/src/atls/utils/urllib3/patch.py` & `pyatls-0.0.5/src/atls/utils/urllib3/patch.py`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/src/atls/validators/azure/aas/aci_validator.py` & `pyatls-0.0.5/src/atls/validators/azure/aas/aci_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import base64
 import hashlib
 import json
+import logging
+from datetime import timedelta
 from typing import Any, Dict, List, Optional
 
 import jwt
 from atls.validators import Validator
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric.types import (
     CertificatePublicKeyTypes,
 )
 from cryptography.x509.oid import ObjectIdentifier
 
+logger = logging.getLogger(__name__)
+
 
 class AciValidator(Validator):
     """
     Validates an attestation document issued for a confidential Azure ACI
     container running on AMD SEV-SNP using the Azure Attestation Service (AAS).
 
     Parameters
@@ -46,21 +50,24 @@
         # 1.3.9999.2.1.2 = iso.identified-organization.reserved.azure.aas.aci
         return oid == ObjectIdentifier("1.3.9999.2.1.2")
 
     def validate(
         self, document: bytes, public_key: bytes, nonce: bytes
     ) -> bool:
         # This verifies the signature of the JWT, too.
+        logger.info("Verifying and decoding JWT token...")
         try:
             token = _verify_and_decode_token(document.decode(), self._jkus)
-        except jwt.PyJWTError:
+        except jwt.PyJWTError as ex:
+            logger.error("Failed to verify and decode JWT token:\n%s", ex)
             return False
 
         # The runtime data structure must match exactly the structure generated
         # by the Go ACI attestation issuer.
+        logger.info("Parsing runtime data...")
         runtime_data = {
             "publicKey": base64.b64encode(public_key).decode(),
             "nonce": base64.b64encode(nonce).decode(),
         }
 
         # The JSON representation of the runtime data structure must match
         # exactly that generated by the Go ACI attestation issuer. In this
@@ -81,55 +88,63 @@
 
         # TODO/HEGATTA: The AAS SEV-SNP attestation endpoint expects the
         # runtime data hash to be SHA256 while SEV-SNP hardware itself expects
         # a 512-byte block. As such, the last 64 hex bytes in AAS' claim is
         # just zeroes. Ideally, AAS should accept a SHA512 hash of the runtime
         # data.
         if "x-ms-sevsnpvm-reportdata" not in token:
+            logger.error("x-ms-sevsnpvm-reportdata is missing")
             return False
 
         aas_runtime_data_hash: str = token["x-ms-sevsnpvm-reportdata"]
         aas_runtime_data_hash = aas_runtime_data_hash[:64]
 
         if runtime_data_json_hash_hex != aas_runtime_data_hash:
+            logger.error("Runtime data in JWT is not as expected")
             return False
 
         if (
             "x-ms-attestation-type" not in token
             or token["x-ms-attestation-type"] != "sevsnpvm"
         ):
+            logger.error("x-ms-attestation-type is missing or incorrect")
             return False
 
         if (
             "x-ms-compliance-status" not in token
             or token["x-ms-compliance-status"] != "azure-compliant-uvm"
         ):
+            logger.error("x-ms-compliance-status is missing or incorrect")
             return False
 
         if (
             "x-ms-sevsnpvm-is-debuggable" not in token
             or token["x-ms-sevsnpvm-is-debuggable"]
         ):
+            logger.error("x-ms-sevsnpvm-is-debuggable is missing or incorrect")
             return False
 
         if "x-ms-runtime" not in token:
+            logger.error("x-ms-runtime is missing")
             return False
 
         token_runtime: Dict[str, Any] = token["x-ms-runtime"]
 
         if (
             "nonce" not in token_runtime
             or base64.b64decode(token_runtime["nonce"]) != nonce
         ):
+            logger.error("nonce is incorrect")
             return False
 
         if (
             "publicKey" not in token_runtime
             or base64.b64decode(token_runtime["publicKey"]) != public_key
         ):
+            logger.error("public key in runtime data is incorrect")
             return False
 
         if self._policies is not None:
             if "x-ms-sevsnpvm-hostdata" not in token:
                 return False
 
             token_host_data = token["x-ms-sevsnpvm-hostdata"]
@@ -137,14 +152,15 @@
                 policy_hash_hex = hashlib.sha256(policy.encode()).hexdigest()
 
                 if token_host_data == policy_hash_hex:
                     return True
 
             return False
 
+        logger.info("JWT validation succeeded")
         return True
 
     @property
     def jkus(self) -> Optional[List[str]]:
         """List of allowed JKU claim values."""
         return self._jkus
 
@@ -190,20 +206,28 @@
         header was passed to this function.
     """
     jku: str = header["jku"]
 
     if jkus is not None and jku not in jkus:
         raise ValueError("Untrusted JKU found in token")
 
+    logger.info("Fetching KID...")
     kid: str = header["kid"]
 
     jwks_client = jwt.PyJWKClient(jku)
-    for key in jwks_client.fetch_data().get("keys", []):
+
+    logger.info("Fetching JWKS data...")
+    jwks_data = jwks_client.fetch_data()
+
+    for key in jwks_data.get("keys", []):
         if key["kid"] == kid:
+            logger.info("Decoding x5c value...")
             cert_der = jwt.utils.base64url_decode(key["x5c"][0])
+
+            logger.info("Loading certificate and public key...")
             return x509.load_der_x509_certificate(cert_der).public_key()
 
     raise LookupError("No matching key was found in JWKS")
 
 
 def _verify_and_decode_token(
     token: str, jkus: Optional[List[str]]
@@ -223,8 +247,14 @@
     Returns
     -------
     claims : dict of str to any
         A dictionary containing the decoded claims from the provided JWT token.
     """
     hdr = jwt.get_unverified_header(token)
 
-    return jwt.decode(token, _get_key_by_header(hdr, jkus), [hdr["alg"]])
+    return jwt.decode(
+        token,
+        _get_key_by_header(hdr, jkus),
+        [hdr["alg"]],
+        # Account for clock skew
+        leeway=timedelta(seconds=5),
+    )
```

### Comparing `pyatls-0.0.3/src/atls/validators/azure/aas/cvm_validator.py` & `pyatls-0.0.5/src/atls/validators/azure/aas/cvm_validator.py`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/src/atls/validators/validator.py` & `pyatls-0.0.5/src/atls/validators/validator.py`

 * *Files identical despite different names*

### Comparing `pyatls-0.0.3/src/pyatls.egg-info/PKG-INFO` & `pyatls-0.0.5/src/pyatls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatls
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Python package that implements Attested TLS (aTLS).
 Author-email: Opaque Systems <pypi@opaque.co>
 License:                                 Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,31 +202,37 @@
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
 Project-URL: Homepage, https://github.com/opaque-systems/atls-python
-Keywords: confidential,llm,tls,ssl,atls,attestation,security,privacy
+Keywords: atls,attestation,confidential,llm,privacy,security,ssl,tls
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
+Requires-Dist: PyJWT
+Requires-Dist: pyOpenSSL
+Requires-Dist: urllib3<2.1.0,>=2.0.0
+Provides-Extra: requests
+Requires-Dist: requests; extra == "requests"
 
 # Python aTLS Package
 
 An implementation of Attested TLS (aTLS) for Python.
 
 Supports the client-side handshake against a custom attester that issues JWT
 tokens via the Azure Attestation Service (AAS) running on Azure Container
 Instance (ACI) instances.
 
 For the moment, this package exists to support
-[`promptguard`](https://pypi.org/project/promptguard/), a confidential
+[`OpaquePrompts`](https://pypi.org/project/opaqueprompts/), a confidential
 information redaction service that runs in a Trusted Execution Environment
 (TEE).
 
 **API Stability:** This package is still in development. As such, its API may
 change until it is sufficiently mature.
 
 **Note:** The server-side counterpart to this package is not yet public. If you
```

### Comparing `pyatls-0.0.3/src/pyatls.egg-info/SOURCES.txt` & `pyatls-0.0.5/src/pyatls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

