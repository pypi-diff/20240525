# Comparing `tmp/infisical_python-2.1.9.tar.gz` & `tmp/infisical_python-2.2.0.tar.gz`

## Comparing `infisical_python-2.1.9.tar` & `infisical_python-2.2.0.tar`

### file list

```diff
@@ -1,52 +1,59 @@
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 infisical_python-2.1.9/local_dependencies/infisical-json/Cargo.toml
--rw-r--r--   0     1001      127     2314 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/client.rs
--rw-r--r--   0     1001      127     1122 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/command.rs
--rw-r--r--   0     1001      127       51 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/lib.rs
--rw-r--r--   0     1001      127     1788 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical-json/src/response.rs
--rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 infisical_python-2.1.9/local_dependencies/infisical/Cargo.toml
--rw-r--r--   0     1001      127     1625 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/access_token.rs
--rw-r--r--   0     1001      127     1951 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/mod.rs
--rw-r--r--   0     1001      127     2311 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/create_secret.rs
--rw-r--r--   0     1001      127     1907 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/delete_secret.rs
--rw-r--r--   0     1001      127     2590 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/get_secret.rs
--rw-r--r--   0     1001      127     2904 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/list_secrets.rs
--rw-r--r--   0     1001      127      111 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/mod.rs
--rw-r--r--   0     1001      127     1733 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/update_secret.rs
--rw-r--r--   0     1001      127      806 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/auth/authenticate.rs
--rw-r--r--   0     1001      127      133 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/auth/mod.rs
--rw-r--r--   0     1001      127     4966 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/cache.rs
--rw-r--r--   0     1001      127     1658 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/client/client.rs
--rw-r--r--   0     1001      127     1032 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/client/client_settings.rs
--rw-r--r--   0     1001      127       61 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/client/mod.rs
--rw-r--r--   0     1001      127     4621 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/error.rs
--rw-r--r--   0     1001      127     2935 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/helper.rs
--rw-r--r--   0     1001      127      167 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/lib.rs
--rw-r--r--   0     1001      127     1144 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_cryptography.rs
--rw-r--r--   0     1001      127     1894 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_secrets.rs
--rw-r--r--   0     1001      127      708 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs
--rw-r--r--   0     1001      127     2519 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs
--rw-r--r--   0     1001      127     2405 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs
--rw-r--r--   0     1001      127      335 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/mod.rs
--rw-r--r--   0     1001      127       93 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/mod.rs
--rw-r--r--   0     1001      127     1365 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/create.rs
--rw-r--r--   0     1001      127     1092 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/delete.rs
--rw-r--r--   0     1001      127      985 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/get.rs
--rw-r--r--   0     1001      127      990 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/list.rs
--rw-r--r--   0     1001      127      979 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/mod.rs
--rw-r--r--   0     1001      127     1201 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/update.rs
--rw-r--r--   0     1001      127     3791 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/tests/cryptography.rs
--rw-r--r--   0     1001      127    10538 2024-04-15 11:50:35.000000 infisical_python-2.1.9/local_dependencies/infisical/tests/secrets.rs
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 infisical_python-2.1.9/Cargo.toml
--rw-r--r--   0     1001      127     1053 2024-04-15 11:50:35.000000 infisical_python-2.1.9/LICENSE
--rw-r--r--   0     1001      127       43 2024-04-15 11:50:35.000000 infisical_python-2.1.9/MANIFEST.in
--rw-r--r--   0     1001      127      502 2024-04-15 11:50:35.000000 infisical_python-2.1.9/README.md
--rw-r--r--   0     1001      127      894 2024-04-15 11:50:35.000000 infisical_python-2.1.9/example.py
--rw-r--r--   0     1001      127      866 2024-04-15 11:50:44.000000 infisical_python-2.1.9/infisical_client/__init__.py
--rw-r--r--   0     1001      127     3643 2024-04-15 11:50:35.000000 infisical_python-2.1.9/infisical_client/infisical_client.py
--rw-r--r--   0     1001      127     2123 2024-04-15 11:50:44.000000 infisical_python-2.1.9/pyproject.toml
--rw-r--r--   0     1001      127      938 2024-04-15 11:50:35.000000 infisical_python-2.1.9/src/client.rs
--rw-r--r--   0     1001      127      104 2024-04-15 11:50:35.000000 infisical_python-2.1.9/src/lib.rs
--rw-r--r--   0     1001      127      189 2024-04-15 11:50:35.000000 infisical_python-2.1.9/src/python_module.rs
--rw-r--r--   0        0        0    62705 2024-04-15 11:51:30.000000 infisical_python-2.1.9/Cargo.lock
--rw-r--r--   0     1001      127    40201 2024-04-15 11:50:45.000000 infisical_python-2.1.9/infisical_client/schemas.py
--rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 infisical_python-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 infisical_python-2.2.0/local_dependencies/infisical/Cargo.toml
+-rw-r--r--   0     1001      127     3901 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/aws_iam_login.rs
+-rw-r--r--   0     1001      127     3895 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/gcp_iam_login.rs
+-rw-r--r--   0     1001      127     1814 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/gcp_id_token_login.rs
+-rw-r--r--   0     1001      127     1826 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/kubernetes_login.rs
+-rw-r--r--   0     1001      127     3734 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/mod.rs
+-rw-r--r--   0     1001      127     1807 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/universal_auth_login.rs
+-rw-r--r--   0     1001      127     1943 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/mod.rs
+-rw-r--r--   0     1001      127     2311 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/create_secret.rs
+-rw-r--r--   0     1001      127     1907 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/delete_secret.rs
+-rw-r--r--   0     1001      127     2590 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/get_secret.rs
+-rw-r--r--   0     1001      127     3754 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/list_secrets.rs
+-rw-r--r--   0     1001      127      111 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/mod.rs
+-rw-r--r--   0     1001      127     1733 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/update_secret.rs
+-rw-r--r--   0     1001      127      830 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/auth/authenticate.rs
+-rw-r--r--   0     1001      127      125 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/auth/mod.rs
+-rw-r--r--   0     1001      127     4966 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/cache.rs
+-rw-r--r--   0     1001      127     8184 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/auth_method_settings.rs
+-rw-r--r--   0     1001      127     1977 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/client.rs
+-rw-r--r--   0     1001      127     2006 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/client_settings.rs
+-rw-r--r--   0     1001      127       91 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/mod.rs
+-rw-r--r--   0     1001      127     1135 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/constants.rs
+-rw-r--r--   0     1001      127     5797 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/error.rs
+-rw-r--r--   0     1001      127     8314 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/helper.rs
+-rw-r--r--   0     1001      127      159 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/lib.rs
+-rw-r--r--   0     1001      127     1144 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_cryptography.rs
+-rw-r--r--   0     1001      127     1894 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_secrets.rs
+-rw-r--r--   0     1001      127      708 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs
+-rw-r--r--   0     1001      127     2519 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs
+-rw-r--r--   0     1001      127     2405 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs
+-rw-r--r--   0     1001      127      335 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/mod.rs
+-rw-r--r--   0     1001      127       93 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/mod.rs
+-rw-r--r--   0     1001      127     1365 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/create.rs
+-rw-r--r--   0     1001      127     1092 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/delete.rs
+-rw-r--r--   0     1001      127      985 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/get.rs
+-rw-r--r--   0     1001      127     1071 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/list.rs
+-rw-r--r--   0     1001      127      979 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/mod.rs
+-rw-r--r--   0     1001      127     1201 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/update.rs
+-rw-r--r--   0     1001      127     4361 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/tests/cryptography.rs
+-rw-r--r--   0     1001      127    11199 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/tests/secrets.rs
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 infisical_python-2.2.0/local_dependencies/infisical-json/Cargo.toml
+-rw-r--r--   0     1001      127     2314 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/client.rs
+-rw-r--r--   0     1001      127     1122 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/command.rs
+-rw-r--r--   0     1001      127       51 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/lib.rs
+-rw-r--r--   0     1001      127     1788 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/response.rs
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 infisical_python-2.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     1053 2024-05-25 17:01:55.000000 infisical_python-2.2.0/LICENSE
+-rw-r--r--   0     1001      127       43 2024-05-25 17:01:55.000000 infisical_python-2.2.0/MANIFEST.in
+-rw-r--r--   0     1001      127      502 2024-05-25 17:01:55.000000 infisical_python-2.2.0/README.md
+-rw-r--r--   0     1001      127      894 2024-05-25 17:01:55.000000 infisical_python-2.2.0/example.py
+-rw-r--r--   0     1001      127     1198 2024-05-25 17:02:00.000000 infisical_python-2.2.0/infisical_client/__init__.py
+-rw-r--r--   0     1001      127     3814 2024-05-25 17:01:55.000000 infisical_python-2.2.0/infisical_client/infisical_client.py
+-rw-r--r--   0     1001      127     2123 2024-05-25 17:01:59.000000 infisical_python-2.2.0/pyproject.toml
+-rw-r--r--   0     1001      127      938 2024-05-25 17:01:55.000000 infisical_python-2.2.0/src/client.rs
+-rw-r--r--   0     1001      127      104 2024-05-25 17:01:55.000000 infisical_python-2.2.0/src/lib.rs
+-rw-r--r--   0     1001      127      189 2024-05-25 17:01:55.000000 infisical_python-2.2.0/src/python_module.rs
+-rw-r--r--   0        0        0    80967 2024-05-25 17:02:48.000000 infisical_python-2.2.0/Cargo.lock
+-rw-r--r--   0     1001      127    47505 2024-05-25 17:02:01.000000 infisical_python-2.2.0/infisical_client/schemas.py
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 infisical_python-2.2.0/PKG-INFO
```

### Comparing `infisical_python-2.1.9/local_dependencies/infisical-json/src/client.rs` & `infisical_python-2.2.0/local_dependencies/infisical-json/src/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical-json/src/command.rs` & `infisical_python-2.2.0/local_dependencies/infisical-json/src/command.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical-json/src/response.rs` & `infisical_python-2.2.0/local_dependencies/infisical-json/src/response.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/Cargo.toml` & `infisical_python-2.2.0/local_dependencies/infisical/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 [package]
 name = "infisical"
 version = "0.1.0"
 edition = "2021"
 rust-version = "1.57"
 
 [dependencies]
+aws-config = "1.0.1"
+aws-credential-types = "1.0.1"
+aws-sigv4 = "1.2.1"
+http = "1.0.0"
+google-iamcredentials1 = "5.0.4"
 schemars = { version = ">=0.8, <0.9", features = ["uuid1", "chrono"] }
 aes = ">=0.8.2, <0.9"
 argon2 = { version = ">=0.5.0, <0.6", features = [
     "alloc",
 ], default-features = false }
 assert_matches = ">=1.5.0, <2.0"
 base64 = ">=0.21.2, <0.22"
```

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/api/mod.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/api/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pub mod access_token;
+pub mod auth;
 pub mod secrets;
 
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 use std::error;
 use std::fmt;
```

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/create_secret.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/create_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/delete_secret.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/delete_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/get_secret.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/get_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/api/secrets/update_secret.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/update_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/cache.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/cache.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/error.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/error.rs`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,50 @@
     "Failed workspace authorization due to blind indices not being enabled";
 
 #[derive(Debug, Error)]
 pub enum Error {
     #[error("Something unexpected went wrong.")]
     UnknownError,
 
+    #[error("Something went wrong: {}", .message)]
+    UnknownErrorWithMessage { message: String },
+
+    #[error("Failed to get AWS credentials: {}", .message)]
+    AwsCredentialsError { message: String },
+
+    #[error("Failed to build AWS request signer: {}", .message)]
+    AwsBuildRequestSignerError { message: String },
+
+    #[error("Failed to sign AWS request: {}", .message)]
+    AwsSignRequestError { message: String },
+
+    #[error("Failed to get AWS region: {}", .message)]
+    AwsGetRegionError { message: String },
+
     #[error("Failed to create symmetric key: {}", .message)]
     CreateSymmetricKeyError { message: String },
 
+    #[error("Failed to authenticate due to missing parameters: {}", .message)]
+    MissingParametersAuthError { message: String },
+
+    #[error("Failed to obtain metadata from Google Cloud")]
+    GoogleMetadataError,
+
+    #[error("Failed to sign JWT from Google Cloud: {}", .message)]
+    GoogleJwtError { message: String },
+
+    #[error("Failed to get token from Google Cloud Platform: {}", .message)]
+    GoogleTokenError { message: String },
+
+    #[error("Authentication parsing failed: {}", .message)]
+    AuthSanitizationError { message: String },
+
+    #[error("No access token was obtained after authentication.")]
+    NoAccessTokenObtained,
+
     #[error("Failed to encrypt symmetric key: {}", .message)]
     EncryptSymmetricKeyError { message: String },
 
     #[error("Failed to decrypt symmetric key: {}", .message)]
     DecryptSymmetricKeyError { message: String },
 
     #[error("Missing access token.")]
```

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_cryptography.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_cryptography.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/client_secrets.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/create.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/create.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/delete.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/delete.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/get.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/get.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/list.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/list.rs`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #[derive(Serialize, Deserialize, Debug, JsonSchema)]
 #[serde(rename_all = "camelCase")]
 pub struct ListSecretsOptions {
     pub environment: String,
     pub project_id: String,
     pub path: Option<String>,
 
+    pub expand_secret_references: Option<bool>,
+    pub recursive: Option<bool>,
     pub attach_to_process_env: Option<bool>,
     pub include_imports: Option<bool>,
 }
 
 #[derive(Serialize, Deserialize, Debug, JsonSchema)]
 #[serde(rename_all = "camelCase")]
 pub struct ListSecretsResponse {
```

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/mod.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/mod.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/src/manager/secrets/update.rs` & `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/update.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/tests/cryptography.rs` & `infisical_python-2.2.0/local_dependencies/infisical/tests/cryptography.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 use dotenv::dotenv;
-use infisical::{client::client_settings::ClientSettings, Client};
+use infisical::{
+    client::{
+        auth_method_settings::{AuthenticationOptions, UniversalAuthMethod},
+        client_settings::ClientSettings,
+    },
+    Client,
+};
 
 struct Environment {
     client_id: String,
     client_secret: String,
     site_url: String,
 }
 
@@ -25,18 +31,33 @@
 
     return environment;
 }
 
 fn create_client() -> Client {
     let environment = get_environment_variables();
 
+    #[allow(deprecated)]
     let settings = ClientSettings {
-        client_id: Some(environment.client_id),
-        client_secret: Some(environment.client_secret),
+        // These fields are deprecated. If they are populated, they will be backfilled into the new auth object.
+        client_id: None,
+        client_secret: None,
         access_token: None,
+
+        auth: AuthenticationOptions {
+            gcp_iam: None,
+            gcp_id_token: None,
+            kubernetes: None,
+            aws_iam: None,
+            access_token: None,
+            universal_auth: Some(UniversalAuthMethod {
+                client_id: environment.client_id,
+                client_secret: environment.client_secret,
+            }),
+        },
+
         site_url: Some(environment.site_url),
         cache_ttl: None,
         user_agent: Some("infisical-cryptography-test-sdk".to_string()),
     };
 
     let client = Client::new(Some(settings));
```

### Comparing `infisical_python-2.1.9/local_dependencies/infisical/tests/secrets.rs` & `infisical_python-2.2.0/local_dependencies/infisical/tests/secrets.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use infisical::client::auth_method_settings::AuthenticationOptions;
 use rand::{distributions::Alphanumeric, Rng};
 
 use dotenv::dotenv;
 use infisical::manager::client_secrets::{create_secret, delete_secret};
 use infisical::manager::secrets::{CreateSecretOptions, DeleteSecretOptions, Secret};
 use infisical::{client::client_settings::ClientSettings, Client};
 
@@ -96,21 +97,26 @@
 
     return environment;
 }
 
 fn create_client() -> Client {
     let environment = get_environment_variables();
 
+    #[allow(deprecated)]
     let settings = ClientSettings {
+        // These fields are deprecated. If they are populated, they will be backfilled into the new auth object.
         client_id: Some(environment.client_id),
         client_secret: Some(environment.client_secret),
         access_token: None,
+
         site_url: Some(environment.site_url),
         cache_ttl: None,
         user_agent: Some("infisical-secrets-test-sdk".to_string()),
+
+        auth: AuthenticationOptions::default(),
     };
 
     let client = Client::new(Some(settings));
 
     return client;
 }
 
@@ -205,30 +211,38 @@
         let mut client = create_client();
         let variables = &get_environment_variables();
         let environment = &"dev";
 
         let options = ListSecretsOptions {
             environment: environment.to_string(),
             project_id: variables.project_id.to_string(),
+            recursive: Some(true),
+            expand_secret_references: None,
             path: None,
             include_imports: None,
             attach_to_process_env: None,
         };
 
         let dummy_secret = create_dummy_secret(&mut client).await;
 
         let secrets = list_secrets(&mut client, &options).await;
 
         match secrets {
             Ok(secrets) => {
                 assert!(secrets.secrets.len() > 0);
 
+                // Find secret in a folder to ensure recursive mode works as intended.
+                let secret_in_folder = secrets.secrets.iter().find(|&s| {
+                    s.secret_key == "SECRET_IN_FOLDER" && s.secret_value == "test-secret"
+                });
+                assert!(secret_in_folder.is_some());
+
                 let mut found_secret = false;
 
-                // Loop through secrets and make sure they are all in the same environment, and the secret with SECRET_NAME exists
+                // Loop through secrets and make sure they are all in the same environment, and the secret with SECRET_NAME exists.
                 for secret in secrets.secrets {
                     assert_eq!(secret.environment, environment.as_ref());
                     assert_eq!(secret.workspace, variables.project_id.as_ref());
 
                     if secret.secret_key == dummy_secret.secret_key {
                         assert_eq!(secret.secret_value, dummy_secret.secret_value);
                         found_secret = true;
```

### Comparing `infisical_python-2.1.9/Cargo.toml` & `infisical_python-2.2.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "infisical-py"
-version = "2.1.9"
+version = "2.2.0"
 edition = "2021"
 rust-version = "1.57"
 
 [lib]
 name = "infisical_py"
 crate-type = ["cdylib"]
```

### Comparing `infisical_python-2.1.9/LICENSE` & `infisical_python-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/example.py` & `infisical_python-2.2.0/example.py`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/infisical_client/infisical_client.py` & `infisical_python-2.2.0/infisical_client/infisical_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         result = self._run_command(Command(list_secrets=options))
 
         secrets = ResponseForListSecretsResponse.from_dict(result).data.secrets
 
         # Setting the env in Rust is not enough for Python apparently, so we have to do this as well.
         if options.attach_to_process_env:
             for secret in secrets:
-                os.environ[secret.secret_key] = secret.secret_value
+              # we need to check if the env variable is already set, if it is we don't want to overwrite it!
+              if os.environ.get(secret.secret_key) is None:
+                  os.environ[secret.secret_key] = secret.secret_value
 
         return secrets
     
     def updateSecret(self, options: UpdateSecretOptions) -> SecretElement:
         result = self._run_command(Command(update_secret=options))
 
         return ResponseForUpdateSecretResponse.from_dict(result).data.secret
```

### Comparing `infisical_python-2.1.9/pyproject.toml` & `infisical_python-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [tool.poetry]
 name = "infisical-python"
-version = "2.1.9"
+version = "2.2.0"
 description = 'Official Infisical SDK for Python (New)'
 authors = ["Daniel Hougaard <daniel@infisical.com>"]
 
 [tool.poetry_bumpversion.file."infisical_client/__init__.py"]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
```

### Comparing `infisical_python-2.1.9/src/client.rs` & `infisical_python-2.2.0/src/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.1.9/Cargo.lock` & `infisical_python-2.2.0/Cargo.lock`

 * *Files 13% similar despite different names*

```diff
@@ -58,18 +58,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "argon2"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c3610892ee6e0cbce8ae2700349fcf8f98adb0dbfbee85aec3c9179d29cc072"
 dependencies = [
@@ -82,29 +97,336 @@
 [[package]]
 name = "assert_matches"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b34d609dfbaf33d6889b2b7106d3ca345eacad44200913df5ba02bfd31d2ba9"
 
 [[package]]
+name = "async-trait"
+version = "0.1.80"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
+
+[[package]]
+name = "aws-config"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1234b742ac4a40a7d3459c6e3c99818271976a5a6ae3732cb415f4a9a94da7b6"
+dependencies = [
+ "aws-credential-types",
+ "aws-runtime",
+ "aws-sdk-sso",
+ "aws-sdk-ssooidc",
+ "aws-sdk-sts",
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-json",
+ "aws-smithy-runtime",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "fastrand",
+ "hex",
+ "http 0.2.12",
+ "hyper",
+ "ring",
+ "time",
+ "tokio",
+ "tracing",
+ "url 2.5.0",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-credential-types"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "e16838e6c9e12125face1c1eff1343c75e3ff540de98ff7ebd61874a89bcfeb9"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-runtime"
+version = "1.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75588e7ee5e8496eed939adac2035a6dbab9f7eb2acdd9ab2d31856dab6f3955"
+dependencies = [
+ "aws-credential-types",
+ "aws-sigv4",
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "fastrand",
+ "http 0.2.12",
+ "http-body 0.4.6",
+ "percent-encoding 2.3.1",
+ "pin-project-lite",
+ "tracing",
+ "uuid",
+]
+
+[[package]]
+name = "aws-sdk-sso"
+version = "1.27.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aef53f254e16c00cfbfd69fa6eca4d858b7c161878db2cd248410af402d1951e"
+dependencies = [
+ "aws-credential-types",
+ "aws-runtime",
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-json",
+ "aws-smithy-runtime",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "http 0.2.12",
+ "once_cell",
+ "regex-lite",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sdk-ssooidc"
+version = "1.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d1b673b2972c38463955e27d76c9d2ebb0452a9ce8059a0e2c9ed67efe69ef35"
+dependencies = [
+ "aws-credential-types",
+ "aws-runtime",
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-json",
+ "aws-smithy-runtime",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "aws-types",
+ "bytes",
+ "http 0.2.12",
+ "once_cell",
+ "regex-lite",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sdk-sts"
+version = "1.27.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d461680731ce37d14396ceeb4ef326998bf9c848123f93a6191958ecd7f6cc0"
+dependencies = [
+ "aws-credential-types",
+ "aws-runtime",
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-json",
+ "aws-smithy-query",
+ "aws-smithy-runtime",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "aws-smithy-xml",
+ "aws-types",
+ "http 0.2.12",
+ "once_cell",
+ "regex-lite",
+ "tracing",
+]
+
+[[package]]
+name = "aws-sigv4"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "58b56f1cbe6fd4d0c2573df72868f20ab1c125ca9c9dbce17927a463433a2e57"
+dependencies = [
+ "aws-credential-types",
+ "aws-smithy-http",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "bytes",
+ "form_urlencoded",
+ "hex",
+ "hmac",
+ "http 0.2.12",
+ "http 1.1.0",
+ "once_cell",
+ "percent-encoding 2.3.1",
+ "sha2",
+ "time",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-async"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "62220bc6e97f946ddd51b5f1361f78996e704677afc518a4ff66b7a72ea1378c"
+dependencies = [
+ "futures-util",
+ "pin-project-lite",
+ "tokio",
+]
+
+[[package]]
+name = "aws-smithy-http"
+version = "0.60.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4a7de001a1b9a25601016d8057ea16e31a45fdca3751304c8edf4ad72e706c08"
+dependencies = [
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "bytes",
+ "bytes-utils",
+ "futures-core",
+ "http 0.2.12",
+ "http-body 0.4.6",
+ "once_cell",
+ "percent-encoding 2.3.1",
+ "pin-project-lite",
+ "pin-utils",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-json"
+version = "0.60.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4683df9469ef09468dad3473d129960119a0d3593617542b7d52086c8486f2d6"
+dependencies = [
+ "aws-smithy-types",
+]
+
+[[package]]
+name = "aws-smithy-query"
+version = "0.60.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2fbd61ceb3fe8a1cb7352e42689cec5335833cd9f94103a61e98f9bb61c64bb"
+dependencies = [
+ "aws-smithy-types",
+ "urlencoding",
+]
+
+[[package]]
+name = "aws-smithy-runtime"
+version = "1.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "607e8b53aeb2bc23fb332159d72a69650cd9643c161d76cd3b7f88ac00b5a1bb"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-http",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "bytes",
+ "fastrand",
+ "h2",
+ "http 0.2.12",
+ "http-body 0.4.6",
+ "http-body 1.0.0",
+ "hyper",
+ "hyper-rustls",
+ "once_cell",
+ "pin-project-lite",
+ "pin-utils",
+ "rustls 0.21.12",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
+name = "aws-smithy-runtime-api"
+version = "1.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b7d790d553d163c7d80a4e06e2906bf24b9172c9ebe045fc3a274e9358ab7bb"
+dependencies = [
+ "aws-smithy-async",
+ "aws-smithy-types",
+ "bytes",
+ "http 0.2.12",
+ "http 1.1.0",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
+ "zeroize",
+]
+
+[[package]]
+name = "aws-smithy-types"
+version = "1.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b6764ba7e1c5ede1c9f9e4046645534f06c2581402461c559b481a420330a83"
+dependencies = [
+ "base64-simd",
+ "bytes",
+ "bytes-utils",
+ "http 0.2.12",
+ "http 1.1.0",
+ "http-body 0.4.6",
+ "http-body 1.0.0",
+ "http-body-util",
+ "itoa",
+ "num-integer",
+ "pin-project-lite",
+ "pin-utils",
+ "ryu",
+ "serde",
+ "time",
+]
+
+[[package]]
+name = "aws-smithy-xml"
+version = "0.60.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d123fbc2a4adc3c301652ba8e149bf4bc1d1725affb9784eb20c953ace06bf55"
+dependencies = [
+ "xmlparser",
+]
+
+[[package]]
+name = "aws-types"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02fa328e19c849b20ef7ada4c9b581dd12351ff35ecc7642d06e69de4f98407c"
+dependencies = [
+ "aws-credential-types",
+ "aws-smithy-async",
+ "aws-smithy-runtime-api",
+ "aws-smithy-types",
+ "http 0.2.12",
+ "rustc_version",
+ "tracing",
+]
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -115,19 +437,35 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+
+[[package]]
+name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64-simd"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "339abbe78e73178762e23bea9dfd08e697eb3f3301cd4be981c0f78ba5859195"
+dependencies = [
+ "outref",
+ "vsimd",
+]
+
+[[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
 name = "bitflags"
@@ -183,27 +521,37 @@
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
+name = "bytes-utils"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7dafe3a8757b027e2be6e4e5601ed563c55989fcf1546e933c66c8eb3a058d35"
+dependencies = [
+ "bytes",
+ "either",
+]
+
+[[package]]
 name = "cbc"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b52a9543ae338f279b96b0b9fed9c8093744685043739079ce85cd58f289a6"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
 
@@ -215,16 +563,19 @@
 
 [[package]]
 name = "chrono"
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
  "num-traits",
  "serde",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
@@ -313,39 +664,74 @@
  "generic-array",
  "rand_core",
  "typenum",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad291aa74992b9b7a7e88c38acbbf6ad7e107f1d90ee8775b7bc1fc3394f485c"
+checksum = "edb49164822f3ee45b17acd4a208cfc1251410cf0cad9a833234c9890774dd9f"
 dependencies = [
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "ctr"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
+name = "darling"
+version = "0.20.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83b2eb4d90d12bdda5ed17de686c2acb4c57914f8f921b8da7e112b5a36f3fe1"
+dependencies = [
+ "darling_core",
+ "darling_macro",
+]
+
+[[package]]
+name = "darling_core"
+version = "0.20.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
+dependencies = [
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "strsim",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "darling_macro"
+version = "0.20.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
+dependencies = [
+ "darling_core",
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
 dependencies = [
  "cfg-if",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "der"
@@ -355,14 +741,24 @@
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
+name = "deranged"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
+dependencies = [
+ "powerfmt",
+ "serde",
+]
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "const-oid",
@@ -380,17 +776,17 @@
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
@@ -426,26 +822,32 @@
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
+name = "fastrand"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
- "percent-encoding",
+ "percent-encoding 2.3.1",
 ]
 
 [[package]]
 name = "futures"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
@@ -496,15 +898,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -541,17 +943,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -569,25 +971,66 @@
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
+name = "google-apis-common"
+version = "6.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "78672323eaeeb181cadd4d07333f1bcc8c2840a55b58afa8ab052664cd4a54ad"
+dependencies = [
+ "base64 0.13.1",
+ "chrono",
+ "http 0.2.12",
+ "hyper",
+ "itertools 0.10.5",
+ "mime",
+ "serde",
+ "serde_json",
+ "serde_with",
+ "tokio",
+ "tower-service",
+ "url 1.7.2",
+ "yup-oauth2",
+]
+
+[[package]]
+name = "google-iamcredentials1"
+version = "5.0.4+20240221"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f28c9ce6d37137e089dc140bc6d09adf1670914e97e425d7d7094a33746a9e5f"
+dependencies = [
+ "anyhow",
+ "google-apis-common",
+ "http 0.2.12",
+ "hyper",
+ "hyper-rustls",
+ "itertools 0.10.5",
+ "mime",
+ "serde",
+ "serde_json",
+ "tokio",
+ "tower-service",
+ "url 1.7.2",
+]
+
+[[package]]
 name = "h2"
 version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http",
+ "http 0.2.12",
  "indexmap 2.2.6",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
@@ -595,17 +1038,17 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -621,14 +1064,20 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
+
+[[package]]
 name = "hkdf"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b5f8eb2ad728638ea2c7d47a21db23b7b58a72ed6a38256b8a1849f15fbbdf7"
 dependencies = [
  "hmac",
 ]
@@ -650,21 +1099,55 @@
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
+name = "http"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
 name = "http-body"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
- "http",
+ "http 0.2.12",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "http-body"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http 1.1.0",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http 1.1.0",
+ "http-body 1.0.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -689,16 +1172,16 @@
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
- "http",
- "http-body",
+ "http 0.2.12",
+ "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
@@ -709,22 +1192,64 @@
 [[package]]
 name = "hyper-rustls"
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
- "http",
+ "http 0.2.12",
  "hyper",
- "rustls",
+ "log",
+ "rustls 0.21.12",
+ "rustls-native-certs",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows-core",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "ident_case"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
+
+[[package]]
+name = "idna"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38f09e0f0b1fb55fdee1f17470ad800da77af5186a1a76c026b679358b7e844e"
+dependencies = [
+ "matches",
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -744,15 +1269,15 @@
 [[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
@@ -761,22 +1286,27 @@
 name = "infisical"
 version = "0.1.0"
 dependencies = [
  "aes",
  "aes-gcm",
  "argon2",
  "assert_matches",
- "base64",
+ "aws-config",
+ "aws-credential-types",
+ "aws-sigv4",
+ "base64 0.21.7",
  "cbc",
  "chrono",
  "dotenv",
  "env_logger 0.10.2",
  "getrandom",
+ "google-iamcredentials1",
  "hkdf",
  "hmac",
+ "http 1.1.0",
  "lazy_static",
  "log",
  "num-bigint",
  "num-traits",
  "pbkdf2",
  "rand",
  "reqwest",
@@ -790,15 +1320,15 @@
  "serde_repr",
  "serial_test",
  "sha1",
  "sha2",
  "subtle",
  "thiserror",
  "tokio",
- "url",
+ "url 2.5.0",
  "uuid",
 ]
 
 [[package]]
 name = "infisical-c"
 version = "0.1.0"
 dependencies = [
@@ -828,15 +1358,15 @@
  "napi",
  "napi-build",
  "napi-derive",
 ]
 
 [[package]]
 name = "infisical-py"
-version = "2.1.9"
+version = "2.2.0"
 dependencies = [
  "env_logger 0.9.3",
  "infisical-json",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-build-config",
@@ -883,14 +1413,23 @@
  "hermit-abi 0.3.9",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
+
+[[package]]
+name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
@@ -936,17 +1475,17 @@
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
  "spin 0.5.2",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
@@ -958,29 +1497,35 @@
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
+name = "matches"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2532096657941c2fea9c289d370a250971c689d4f143798ff67113ec042024a5"
+
+[[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
@@ -995,17 +1540,17 @@
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -1015,17 +1560,17 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "napi"
-version = "2.16.2"
+version = "2.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70d04890ef4ec001fad791be785b8b920e2a3f5a6b1188e7a81dfa6197c0dee4"
+checksum = "dfc300228808a0e6aea5a58115c82889240bcf8dab16fc25ad675b33e454b368"
 dependencies = [
  "bitflags 2.5.0",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
  "tokio",
@@ -1035,57 +1580,56 @@
 name = "napi-build"
 version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1c0f5d67ee408a4685b61f5ab7e58605c8ae3f2b4189f0127d804ff13d5560a"
 
 [[package]]
 name = "napi-derive"
-version = "2.16.2"
+version = "2.16.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aff4a63f26a7aa9fa25df6ea36675890115972b207ae516e86bd0c47e31eba39"
+checksum = "e0e034ddf6155192cf83f267ede763fe6c164dfa9971585436b16173718d94c4"
 dependencies = [
  "cfg-if",
  "convert_case",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.64"
+version = "1.0.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5e76afe642e2424ebe465406e328e4316d82af1f79256231d4b0f184c67550a"
+checksum = "bff2c00437f3b3266391eb5e6aa25d0029187daf5caf05b8e3271468fb5ae73e"
 dependencies = [
  "convert_case",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
  "semver",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "napi-sys"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427802e8ec3a734331fec1035594a210ce1ff4dc5bc1950530920ab717964ea3"
 dependencies = [
  "libloading",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint-dig"
 version = "0.8.4"
@@ -1100,38 +1644,44 @@
  "num-traits",
  "rand",
  "smallvec",
  "zeroize",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1140,14 +1690,23 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi 0.3.9",
  "libc",
 ]
 
 [[package]]
+name = "num_threads"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c7398b9c8b70908f6371f47ed36737907c87c52af34c268fed0bf0ceb92ead9"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
@@ -1167,34 +1726,40 @@
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
+name = "outref"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4030760ffd992bef45b0ae3f10ce1aba99e33464c90d14dd7c039884963ddc7a"
+
+[[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "password-hash"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "346f04948ba92c43e8469c1ee6736c7563d71012b17d40745260fe106aac2166"
@@ -1220,14 +1785,20 @@
 checksum = "88b39c9bfcfc231068454382784bb460aae594343fb030d46e9f50a645418412"
 dependencies = [
  "base64ct",
 ]
 
 [[package]]
 name = "percent-encoding"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31010dd2e1ac33d5b46a5b413495239882813e0369f8ed8a5e266f173602f831"
+
+[[package]]
+name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
@@ -1276,24 +1847,30 @@
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -1362,28 +1939,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -1419,19 +1996,19 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -1450,53 +2027,59 @@
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
+name = "regex-lite"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30b661b2f27137bdbc16f00eda72866a92bb28af1753ffbd56744fb6e2e9cd8e"
+
+[[package]]
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
- "http",
- "http-body",
+ "http 0.2.12",
+ "http-body 0.4.6",
  "hyper",
  "hyper-rustls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
- "percent-encoding",
+ "percent-encoding 2.3.1",
  "pin-project-lite",
- "rustls",
+ "rustls 0.21.12",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
  "tokio-rustls",
  "tower-service",
- "url",
+ "url 2.5.0",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
@@ -1532,31 +2115,54 @@
  "spki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
+
+[[package]]
+name = "rustc_version"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring",
- "rustls-webpki",
+ "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
+name = "rustls"
+version = "0.22.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-pki-types",
+ "rustls-webpki 0.102.4",
+ "subtle",
+ "zeroize",
+]
+
+[[package]]
 name = "rustls-native-certs"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
 dependencies = [
  "openssl-probe",
  "rustls-pemfile",
@@ -1566,32 +2172,38 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
+
+[[package]]
 name = "rustls-platform-verifier"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92c57b5de012da34087f2fe711fa29770f9a7abdde660b01bac3c9dbdee91b84"
 dependencies = [
  "core-foundation",
  "core-foundation-sys",
  "jni",
  "log",
  "once_cell",
- "rustls",
+ "rustls 0.21.12",
  "rustls-native-certs",
  "rustls-platform-verifier-android",
- "rustls-webpki",
+ "rustls-webpki 0.101.7",
  "security-framework",
  "security-framework-sys",
  "webpki-roots",
  "winapi",
 ]
 
 [[package]]
@@ -1607,18 +2219,29 @@
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
+name = "rustls-webpki"
+version = "0.102.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ff448f7e92e913c4b7d4c6d8e4540a1724b319b4152b8aef6d4cf8339712b33e"
+dependencies = [
+ "ring",
+ "rustls-pki-types",
+ "untrusted",
+]
+
+[[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1632,37 +2255,37 @@
 checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "schemars"
-version = "0.8.16"
+version = "0.8.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45a28f4c49489add4ce10783f7911893516f15afe45d015608d41faca6bc4d29"
+checksum = "09c024468a378b7e36765cd36702b7a90cc3cba11654f6685c8f233408e89e92"
 dependencies = [
  "chrono",
  "dyn-clone",
  "indexmap 1.9.3",
  "schemars_derive",
  "serde",
  "serde_json",
  "uuid",
 ]
 
 [[package]]
 name = "schemars_derive"
-version = "0.8.16"
+version = "0.8.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c767fd6fa65d9ccf9cf026122c1b555f2ef9a4f0cea69da4d7dbc3e258d30967"
+checksum = "b1eee588578aff73f856ab961cd2f79e36bc45d7ded33a7562adba4667aecc0e"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde_derive_internals",
- "syn 1.0.109",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "scoped-tls"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1cf6437eb19a8f4a6cc0f7dca544973b0b78843adbfeb3683d1a94a0024a294"
@@ -1686,38 +2309,44 @@
 [[package]]
 name = "sdk-schemas"
 version = "0.1.0"
 dependencies = [
  "anyhow",
  "infisical",
  "infisical-json",
- "itertools",
+ "itertools 0.12.1",
  "schemars",
  "serde_json",
 ]
 
 [[package]]
+name = "seahash"
+version = "4.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
+
+[[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "num-bigint",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "seeded-random"
@@ -1728,80 +2357,80 @@
  "parking_lot",
  "rand",
  "rand_chacha",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_derive_internals"
-version = "0.26.0"
+version = "0.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
+checksum = "18d26a20a969b9e3fdf2fc2d9f21eda6c40e2de84c9408bb5d3b05d499aae711"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_qs"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0431a35568651e363364210c91983c1da5eb29404d9f0928b67d4ebcfa7d330c"
 dependencies = [
- "percent-encoding",
+ "percent-encoding 2.3.1",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_repr"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
@@ -1809,14 +2438,42 @@
  "form_urlencoded",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_with"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07ff71d2c147a7b57362cead5e22f772cd52f6ab31cfcd9edcd7f6aeb2a0afbe"
+dependencies = [
+ "base64 0.13.1",
+ "chrono",
+ "hex",
+ "indexmap 1.9.3",
+ "serde",
+ "serde_json",
+ "serde_with_macros",
+ "time",
+]
+
+[[package]]
+name = "serde_with_macros"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "881b6f881b17d13214e5d494c939ebab463d01264ce1811e9d4ac3a882e7695f"
+dependencies = [
+ "darling",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "serial_test"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e56dd856803e253c8f298af3f4d7eb0ae5e23a737252cd90bb4f3b435033b2d"
 dependencies = [
  "dashmap",
  "futures",
@@ -1830,15 +2487,15 @@
 name = "serial_test_derive"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91d129178576168c589c9ec973feedf7d3126c01ac2bf08795109aa35b69fb8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sha1"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
@@ -1857,17 +2514,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "signature"
 version = "2.2.0"
@@ -1891,17 +2548,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -1922,14 +2579,20 @@
 checksum = "d91ed6c858b01f942cd56b37a94b3e0a1798290327d1236e4d9cf4eaca44d29d"
 dependencies = [
  "base64ct",
  "der",
 ]
 
 [[package]]
+name = "strsim"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
+
+[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
@@ -1940,17 +2603,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1993,30 +2656,63 @@
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "time"
+version = "0.3.36"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
+dependencies = [
+ "deranged",
+ "itoa",
+ "libc",
+ "num-conv",
+ "num_threads",
+ "powerfmt",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
+
+[[package]]
+name = "time-macros"
+version = "0.2.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
+dependencies = [
+ "num-conv",
+ "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -2053,39 +2749,38 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls",
+ "rustls 0.21.12",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
@@ -2093,18 +2788,30 @@
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
  "pin-project-lite",
+ "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
+name = "tracing-attributes"
+version = "0.1.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
@@ -2168,24 +2875,41 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "url"
+version = "1.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd4e7c0d531266369519a4aa4f399d748bd37043b00bde1e4ff1f60a120b355a"
+dependencies = [
+ "idna 0.1.5",
+ "matches",
+ "percent-encoding 1.0.1",
+]
+
+[[package]]
+name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
- "idna",
- "percent-encoding",
+ "idna 0.5.0",
+ "percent-encoding 2.3.1",
 ]
 
 [[package]]
+name = "urlencoding"
+version = "2.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "daf8dba3b7eb870caf1ddeed7bc9d2a049f3cfdfae7cb521b087cc33ae4c49da"
+
+[[package]]
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "serde",
 ]
@@ -2193,14 +2917,20 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "vsimd"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c3082ca00d5a5ef149bb8b555a72ae84c9c59f7250f013ac822ac2e49b19c64"
+
+[[package]]
 name = "walkdir"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
@@ -2240,15 +2970,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2274,15 +3004,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -2343,28 +3073,37 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
@@ -2506,11 +3245,44 @@
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "xmlparser"
+version = "0.13.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "66fee0b777b0f5ac1c69bb06d361268faafa61cd4682ae064a171c16c433e9e4"
+
+[[package]]
+name = "yup-oauth2"
+version = "8.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b61da40aeb0907a65f7fb5c1de83c5a224d6a9ebb83bf918588a2bb744d636b8"
+dependencies = [
+ "anyhow",
+ "async-trait",
+ "base64 0.21.7",
+ "futures",
+ "http 0.2.12",
+ "hyper",
+ "hyper-rustls",
+ "itertools 0.12.1",
+ "log",
+ "percent-encoding 2.3.1",
+ "rustls 0.22.4",
+ "rustls-pemfile",
+ "seahash",
+ "serde",
+ "serde_json",
+ "time",
+ "tokio",
+ "tower-service",
+ "url 2.5.0",
+]
+
+[[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `infisical_python-2.1.9/infisical_client/schemas.py` & `infisical_python-2.2.0/infisical_client/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,241 @@
 from dataclasses import dataclass
-from typing import Optional, Any, List, TypeVar, Type, cast, Callable
+from typing import Any, Optional, List, TypeVar, Type, cast, Callable
 
 
 T = TypeVar("T")
 
 
-def from_none(x: Any) -> Any:
-    assert x is None
+def from_str(x: Any) -> str:
+    assert isinstance(x, str)
     return x
 
 
-def from_str(x: Any) -> str:
-    assert isinstance(x, str)
+def from_none(x: Any) -> Any:
+    assert x is None
     return x
 
 
 def from_union(fs, x):
     for f in fs:
         try:
             return f(x)
         except:
             pass
     assert False
 
 
+def to_class(c: Type[T], x: Any) -> dict:
+    assert isinstance(x, c)
+    return cast(Any, x).to_dict()
+
+
 def from_int(x: Any) -> int:
     assert isinstance(x, int) and not isinstance(x, bool)
     return x
 
 
 def from_bool(x: Any) -> bool:
     assert isinstance(x, bool)
     return x
 
 
-def to_class(c: Type[T], x: Any) -> dict:
-    assert isinstance(x, c)
-    return cast(Any, x).to_dict()
-
-
 def from_list(f: Callable[[Any], T], x: Any) -> List[T]:
     assert isinstance(x, list)
     return [f(y) for y in x]
 
 
 @dataclass
+class AWSIamAuthMethod:
+    identity_id: str
+    """The Infisical Identity ID that you want to authenticate to Infisical with."""
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'AWSIamAuthMethod':
+        assert isinstance(obj, dict)
+        identity_id = from_str(obj.get("identityId"))
+        return AWSIamAuthMethod(identity_id)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        result["identityId"] = from_str(self.identity_id)
+        return result
+
+
+@dataclass
+class GCPIamAuthMethod:
+    identity_id: str
+    service_account_key_file_path: str
+    """The path to the GCP Service Account key file.
+    
+    You can generate this key file by going to the GCP Console -> IAM & Admin -> Service
+    Accounts -> *Select your service account* -> Keys tab -> Add key.
+    Note: The key must be in JSON format.
+    """
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'GCPIamAuthMethod':
+        assert isinstance(obj, dict)
+        identity_id = from_str(obj.get("identityId"))
+        service_account_key_file_path = from_str(obj.get("serviceAccountKeyFilePath"))
+        return GCPIamAuthMethod(identity_id, service_account_key_file_path)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        result["identityId"] = from_str(self.identity_id)
+        result["serviceAccountKeyFilePath"] = from_str(self.service_account_key_file_path)
+        return result
+
+
+@dataclass
+class GCPIDTokenAuthMethod:
+    identity_id: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'GCPIDTokenAuthMethod':
+        assert isinstance(obj, dict)
+        identity_id = from_str(obj.get("identityId"))
+        return GCPIDTokenAuthMethod(identity_id)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        result["identityId"] = from_str(self.identity_id)
+        return result
+
+
+@dataclass
+class KubernetesAuthMethod:
+    identity_id: str
+    """The Infisical Identity ID that you want to authenticate to Infisical with."""
+    service_account_token_path: Optional[str] = None
+    """The path to the Kubernetes Service Account token file.
+    
+    This is usually located at /var/run/secrets/kubernetes.io/serviceaccount/token.
+    """
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'KubernetesAuthMethod':
+        assert isinstance(obj, dict)
+        identity_id = from_str(obj.get("identityId"))
+        service_account_token_path = from_union([from_none, from_str], obj.get("serviceAccountTokenPath"))
+        return KubernetesAuthMethod(identity_id, service_account_token_path)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        result["identityId"] = from_str(self.identity_id)
+        if self.service_account_token_path is not None:
+            result["serviceAccountTokenPath"] = from_union([from_none, from_str], self.service_account_token_path)
+        return result
+
+
+@dataclass
+class UniversalAuthMethod:
+    client_id: str
+    client_secret: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'UniversalAuthMethod':
+        assert isinstance(obj, dict)
+        client_id = from_str(obj.get("clientId"))
+        client_secret = from_str(obj.get("clientSecret"))
+        return UniversalAuthMethod(client_id, client_secret)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        result["clientId"] = from_str(self.client_id)
+        result["clientSecret"] = from_str(self.client_secret)
+        return result
+
+
+@dataclass
+class AuthenticationOptions:
+    """Configure the authentication method to use.
+    
+    Make sure to only set one one method at a time to avoid conflicts and unexpected behavior.
+    """
+    access_token: Optional[str] = None
+    aws_iam: Optional[AWSIamAuthMethod] = None
+    gcp_iam: Optional[GCPIamAuthMethod] = None
+    gcp_id_token: Optional[GCPIDTokenAuthMethod] = None
+    kubernetes: Optional[KubernetesAuthMethod] = None
+    universal_auth: Optional[UniversalAuthMethod] = None
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'AuthenticationOptions':
+        assert isinstance(obj, dict)
+        access_token = from_union([from_none, from_str], obj.get("accessToken"))
+        aws_iam = from_union([AWSIamAuthMethod.from_dict, from_none], obj.get("awsIam"))
+        gcp_iam = from_union([GCPIamAuthMethod.from_dict, from_none], obj.get("gcpIam"))
+        gcp_id_token = from_union([GCPIDTokenAuthMethod.from_dict, from_none], obj.get("gcpIdToken"))
+        kubernetes = from_union([KubernetesAuthMethod.from_dict, from_none], obj.get("kubernetes"))
+        universal_auth = from_union([UniversalAuthMethod.from_dict, from_none], obj.get("universalAuth"))
+        return AuthenticationOptions(access_token, aws_iam, gcp_iam, gcp_id_token, kubernetes, universal_auth)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        if self.access_token is not None:
+            result["accessToken"] = from_union([from_none, from_str], self.access_token)
+        if self.aws_iam is not None:
+            result["awsIam"] = from_union([lambda x: to_class(AWSIamAuthMethod, x), from_none], self.aws_iam)
+        if self.gcp_iam is not None:
+            result["gcpIam"] = from_union([lambda x: to_class(GCPIamAuthMethod, x), from_none], self.gcp_iam)
+        if self.gcp_id_token is not None:
+            result["gcpIdToken"] = from_union([lambda x: to_class(GCPIDTokenAuthMethod, x), from_none], self.gcp_id_token)
+        if self.kubernetes is not None:
+            result["kubernetes"] = from_union([lambda x: to_class(KubernetesAuthMethod, x), from_none], self.kubernetes)
+        if self.universal_auth is not None:
+            result["universalAuth"] = from_union([lambda x: to_class(UniversalAuthMethod, x), from_none], self.universal_auth)
+        return result
+
+
+@dataclass
 class ClientSettings:
     access_token: Optional[str] = None
+    """**DEPRECATED**: The access token field is deprecated. Please use the new auth object
+    field instead.
+    """
+    auth: Optional[AuthenticationOptions] = None
+    """Configure the authentication method to use.
+    
+    Make sure to only set one one method at a time to avoid conflicts and unexpected behavior.
+    """
     cache_ttl: Optional[int] = None
+    """cacheTTL controls how often the cache should refresh, default is 300 seconds. Set to 0 to
+    disable the cache.
+    """
     client_id: Optional[str] = None
+    """**DEPRECATED**: The client secret field is deprecated. Please use the new auth object
+    field instead.
+    """
     client_secret: Optional[str] = None
+    """**DEPRECATED**: The client secret field is deprecated. Please use the new auth object
+    field instead.
+    """
     site_url: Optional[str] = None
+    """The URL of the site to connect to. Defaults to "https://app.infisical.com"."""
     user_agent: Optional[str] = None
 
     @staticmethod
     def from_dict(obj: Any) -> 'ClientSettings':
         assert isinstance(obj, dict)
         access_token = from_union([from_none, from_str], obj.get("accessToken"))
+        auth = from_union([AuthenticationOptions.from_dict, from_none], obj.get("auth"))
         cache_ttl = from_union([from_none, from_int], obj.get("cacheTtl"))
         client_id = from_union([from_none, from_str], obj.get("clientId"))
         client_secret = from_union([from_none, from_str], obj.get("clientSecret"))
         site_url = from_union([from_none, from_str], obj.get("siteUrl"))
         user_agent = from_union([from_none, from_str], obj.get("userAgent"))
-        return ClientSettings(access_token, cache_ttl, client_id, client_secret, site_url, user_agent)
+        return ClientSettings(access_token, auth, cache_ttl, client_id, client_secret, site_url, user_agent)
 
     def to_dict(self) -> dict:
         result: dict = {}
         if self.access_token is not None:
             result["accessToken"] = from_union([from_none, from_str], self.access_token)
+        if self.auth is not None:
+            result["auth"] = from_union([lambda x: to_class(AuthenticationOptions, x), from_none], self.auth)
         if self.cache_ttl is not None:
             result["cacheTtl"] = from_union([from_none, from_int], self.cache_ttl)
         if self.client_id is not None:
             result["clientId"] = from_union([from_none, from_str], self.client_id)
         if self.client_secret is not None:
             result["clientSecret"] = from_union([from_none, from_str], self.client_secret)
         if self.site_url is not None:
@@ -247,37 +411,45 @@
 
 
 @dataclass
 class ListSecretsOptions:
     environment: str
     project_id: str
     attach_to_process_env: Optional[bool] = None
+    expand_secret_references: Optional[bool] = None
     include_imports: Optional[bool] = None
     path: Optional[str] = None
+    recursive: Optional[bool] = None
 
     @staticmethod
     def from_dict(obj: Any) -> 'ListSecretsOptions':
         assert isinstance(obj, dict)
         environment = from_str(obj.get("environment"))
         project_id = from_str(obj.get("projectId"))
         attach_to_process_env = from_union([from_none, from_bool], obj.get("attachToProcessEnv"))
+        expand_secret_references = from_union([from_none, from_bool], obj.get("expandSecretReferences"))
         include_imports = from_union([from_none, from_bool], obj.get("includeImports"))
         path = from_union([from_none, from_str], obj.get("path"))
-        return ListSecretsOptions(environment, project_id, attach_to_process_env, include_imports, path)
+        recursive = from_union([from_none, from_bool], obj.get("recursive"))
+        return ListSecretsOptions(environment, project_id, attach_to_process_env, expand_secret_references, include_imports, path, recursive)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["environment"] = from_str(self.environment)
         result["projectId"] = from_str(self.project_id)
         if self.attach_to_process_env is not None:
             result["attachToProcessEnv"] = from_union([from_none, from_bool], self.attach_to_process_env)
+        if self.expand_secret_references is not None:
+            result["expandSecretReferences"] = from_union([from_none, from_bool], self.expand_secret_references)
         if self.include_imports is not None:
             result["includeImports"] = from_union([from_none, from_bool], self.include_imports)
         if self.path is not None:
             result["path"] = from_union([from_none, from_str], self.path)
+        if self.recursive is not None:
+            result["recursive"] = from_union([from_none, from_bool], self.recursive)
         return result
 
 
 @dataclass
 class UpdateSecretOptions:
     environment: str
     project_id: str
```

### Comparing `infisical_python-2.1.9/PKG-INFO` & `infisical_python-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infisical-python
-Version: 2.1.9
+Version: 2.2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Official Infisical SDK for Python (New)
 Maintainer-email: Daniel Hougaard <daniel@infisical.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Documentation, https://github.com/Infisical/sdk/tree/main/crates/infisical-py#readme
-Project-URL: Issues, https://github.com/infisical/sdk/issues
 Project-URL: Source, https://github.com/infisical/sdk
+Project-URL: Issues, https://github.com/infisical/sdk/issues
 
 <h1 align="center">
     <a href="https://github.com/Infisical/infisical">
         <img width="300" src="https://raw.githubusercontent.com/Infisical/infisical-node/main/img/logoname-white.svg#gh-dark-mode-only" alt="infisical">
     </a>
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: infisical-python Version: 2.1.9 Classifier:
+Metadata-Version: 2.1 Name: infisical-python Version: 2.2.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development Classifier: Typing :: Typed
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -12,15 +12,15 @@
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy License-File: LICENSE Summary: Official Infisical SDK
 for Python (New) Maintainer-email: Daniel Hougaard
 infisical.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: Documentation, https://github.com/
-Infisical/sdk/tree/main/crates/infisical-py#readme Project-URL: Issues, https:/
-/github.com/infisical/sdk/issues Project-URL: Source, https://github.com/
-infisical/sdk
+Infisical/sdk/tree/main/crates/infisical-py#readme Project-URL: Source, https:/
+/github.com/infisical/sdk Project-URL: Issues, https://github.com/infisical/
+sdk/issues
                            ************ _[[_ii_nn_ff_ii_ss_ii_cc_aa_ll_]] ************
   Open-source, end-to-end encrypted tool to manage secrets and configs across
                          your team and infrastructure.
 # Documentation [You can find the documentation here](https://infisical.com/
 docs/sdks/languages/python)
```

