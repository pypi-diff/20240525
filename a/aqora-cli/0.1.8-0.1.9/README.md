# Comparing `tmp/aqora_cli-0.1.8.tar.gz` & `tmp/aqora_cli-0.1.9.tar.gz`

## Comparing `aqora_cli-0.1.8.tar` & `aqora_cli-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0     1001      127      259 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/config/Cargo.toml
--rw-r--r--   0     1001      127    13333 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/config/src/lib.rs
--rw-r--r--   0     1001      127      558 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/runner/Cargo.toml
--rw-r--r--   0     1001      127       34 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/runner/src/lib.rs
--rw-r--r--   0     1001      127    14686 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/runner/src/pipeline.rs
--rw-r--r--   0     1001      127    18534 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/runner/src/python.rs
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 aqora_cli-0.1.8/Cargo.toml
--rw-r--r--   0     1001      127     2674 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/.github/workflows/cd.yaml
--rw-r--r--   0     1001      127      589 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/.github/workflows/ci.yaml
--rw-r--r--   0     1001      127       24 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/.gitignore
--rw-r--r--   0     1001      127    66049 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/Cargo.lock
--rw-r--r--   0     1001      127      107 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/Makefile
--rw-r--r--   0     1001      127      351 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/README.md
--rw-r--r--   0     1001      127     6248 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/install.py
--rw-r--r--   0     1001      127     1682 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/colors.rs
--rw-r--r--   0     1001      127     1729 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/clean.rs
--rw-r--r--   0     1001      127      982 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/global_args.rs
--rw-r--r--   0     1001      127     2413 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/info.rs
--rw-r--r--   0     1001      127     8894 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/install.rs
--rw-r--r--   0     1001      127     6593 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/login.rs
--rw-r--r--   0     1001      127     2576 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/mod.rs
--rw-r--r--   0     1001      127      871 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/python.rs
--rw-r--r--   0     1001      127      984 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/shell.rs
--rw-r--r--   0     1001      127     2867 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/template.rs
--rw-r--r--   0     1001      127    21212 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/test.rs
--rw-r--r--   0     1001      127    33639 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/upload.rs
--rw-r--r--   0     1001      127      318 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/commands/version.rs
--rw-r--r--   0     1001      127     1550 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/compress.rs
--rw-r--r--   0     1001      127     6323 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/credentials.rs
--rw-r--r--   0     1001      127     7033 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/dirs.rs
--rw-r--r--   0     1001      127     1704 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/download.rs
--rw-r--r--   0     1001      127     2313 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/error.rs
--rw-r--r--   0     1001      127     4294 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/evaluate.rs
--rw-r--r--   0     1001      127      149 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/competition_by_slug.graphql
--rw-r--r--   0     1001      127      201 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/get_competition_template.graphql
--rw-r--r--   0     1001      127      249 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/get_competition_use_case.graphql
--rw-r--r--   0     1001      127      397 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/latest_submission_version.graphql
--rw-r--r--   0     1001      127      271 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/oauth2_refresh.graphql
--rw-r--r--   0     1001      127      298 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/oauth2_token.graphql
--rw-r--r--   0     1001      127    16106 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/schema.graphql
--rw-r--r--   0     1001      127      340 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/submission_upload_info.graphql
--rw-r--r--   0     1001      127      322 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/update_submission.graphql
--rw-r--r--   0     1001      127      316 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/update_use_case.graphql
--rw-r--r--   0     1001      127      165 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/validate_submission.graphql
--rw-r--r--   0     1001      127      159 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/validate_use_case.graphql
--rw-r--r--   0     1001      127       56 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql/viewer_info.graphql
--rw-r--r--   0     1001      127     2545 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/graphql_client.rs
--rw-r--r--   0     1001      127      688 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/html/login_response.html
--rw-r--r--   0     1001      127     1802 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/id.rs
--rw-r--r--   0     1001      127      346 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/lib.rs
--rw-r--r--   0     1001      127      348 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/main.rs
--rw-r--r--   0     1001      127      524 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/manifest.rs
--rw-r--r--   0     1001      127      494 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/module.rs
--rw-r--r--   0     1001      127     1516 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/process.rs
--rw-r--r--   0     1001      127     1652 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/python.rs
--rw-r--r--   0     1001      127     2532 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/readme.rs
--rw-r--r--   0     1001      127     3293 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/revert_file.rs
--rw-r--r--   0     1001      127      561 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/src/shutdown.rs
--rw-r--r--   0     1001      127      678 2024-03-28 16:22:43.000000 aqora_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 aqora_cli-0.1.8/PKG-INFO
+-rw-r--r--   0     1001      127      259 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/config/Cargo.toml
+-rw-r--r--   0     1001      127    13333 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/config/src/lib.rs
+-rw-r--r--   0     1001      127      558 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/runner/Cargo.toml
+-rw-r--r--   0     1001      127       34 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/runner/src/lib.rs
+-rw-r--r--   0     1001      127    14686 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/runner/src/pipeline.rs
+-rw-r--r--   0     1001      127    18619 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/runner/src/python.rs
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 aqora_cli-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      127     2674 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/.github/workflows/cd.yaml
+-rw-r--r--   0     1001      127      589 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127       24 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/.gitignore
+-rw-r--r--   0     1001      127    66049 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/Cargo.lock
+-rw-r--r--   0     1001      127      107 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/Makefile
+-rw-r--r--   0     1001      127      351 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/README.md
+-rw-r--r--   0     1001      127     6248 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/install.py
+-rw-r--r--   0     1001      127     1682 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/colors.rs
+-rw-r--r--   0     1001      127     1729 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/clean.rs
+-rw-r--r--   0     1001      127      982 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/global_args.rs
+-rw-r--r--   0     1001      127     2413 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/info.rs
+-rw-r--r--   0     1001      127     8894 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/install.rs
+-rw-r--r--   0     1001      127     6624 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/login.rs
+-rw-r--r--   0     1001      127     2576 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/mod.rs
+-rw-r--r--   0     1001      127      871 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/python.rs
+-rw-r--r--   0     1001      127      984 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/shell.rs
+-rw-r--r--   0     1001      127     2867 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/template.rs
+-rw-r--r--   0     1001      127    21533 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/test.rs
+-rw-r--r--   0     1001      127    34185 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/upload.rs
+-rw-r--r--   0     1001      127      318 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/commands/version.rs
+-rw-r--r--   0     1001      127     1550 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/compress.rs
+-rw-r--r--   0     1001      127     6323 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/credentials.rs
+-rw-r--r--   0     1001      127     7033 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/dirs.rs
+-rw-r--r--   0     1001      127     1704 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/download.rs
+-rw-r--r--   0     1001      127     2313 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/error.rs
+-rw-r--r--   0     1001      127     4294 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/evaluate.rs
+-rw-r--r--   0     1001      127      149 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/competition_by_slug.graphql
+-rw-r--r--   0     1001      127      201 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/get_competition_template.graphql
+-rw-r--r--   0     1001      127      249 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/get_competition_use_case.graphql
+-rw-r--r--   0     1001      127      397 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/latest_submission_version.graphql
+-rw-r--r--   0     1001      127      271 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/oauth2_refresh.graphql
+-rw-r--r--   0     1001      127      298 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/oauth2_token.graphql
+-rw-r--r--   0     1001      127    16106 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/schema.graphql
+-rw-r--r--   0     1001      127      340 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/submission_upload_info.graphql
+-rw-r--r--   0     1001      127      322 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/update_submission.graphql
+-rw-r--r--   0     1001      127      316 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/update_use_case.graphql
+-rw-r--r--   0     1001      127      165 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/validate_submission.graphql
+-rw-r--r--   0     1001      127      159 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/validate_use_case.graphql
+-rw-r--r--   0     1001      127       56 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql/viewer_info.graphql
+-rw-r--r--   0     1001      127     2545 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/graphql_client.rs
+-rw-r--r--   0     1001      127      688 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/html/login_response.html
+-rw-r--r--   0     1001      127     1802 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/id.rs
+-rw-r--r--   0     1001      127      346 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      127      348 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/main.rs
+-rw-r--r--   0     1001      127      524 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/manifest.rs
+-rw-r--r--   0     1001      127      494 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/module.rs
+-rw-r--r--   0     1001      127     1516 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/process.rs
+-rw-r--r--   0     1001      127     1652 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/python.rs
+-rw-r--r--   0     1001      127     2532 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/readme.rs
+-rw-r--r--   0     1001      127     3346 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/revert_file.rs
+-rw-r--r--   0     1001      127      561 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/src/shutdown.rs
+-rw-r--r--   0     1001      127      678 2024-04-18 15:43:28.000000 aqora_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 aqora_cli-0.1.9/PKG-INFO
```

### Comparing `aqora_cli-0.1.8/config/src/lib.rs` & `aqora_cli-0.1.9/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/runner/Cargo.toml` & `aqora_cli-0.1.9/runner/Cargo.toml`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/runner/src/pipeline.rs` & `aqora_cli-0.1.9/runner/src/pipeline.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/runner/src/python.rs` & `aqora_cli-0.1.9/runner/src/python.rs`

 * *Files 1% similar despite different names*

```diff
@@ -226,40 +226,39 @@
     async fn ensure_venv(
         uv_path: impl AsRef<Path>,
         venv_path: impl AsRef<Path>,
         cache_path: Option<impl AsRef<Path>>,
         color: ColorChoice,
     ) -> Result<(), EnvError> {
         let path = venv_path.as_ref();
-        if path.join("pyvenv.cfg").exists() {
-            return Ok(());
+        if !path.join("pyvenv.cfg").exists() {
+            let mut cmd = Command::new(uv_path.as_ref());
+            cmd.arg("venv")
+                .arg("--python")
+                .arg(PYTHON_VERSION.as_str())
+                .arg(venv_path.as_ref());
+            if let Some(cache_path) = cache_path.as_ref() {
+                cmd.arg("--cache-dir").arg(cache_path.as_ref());
+            }
+            color.apply(&mut cmd);
+            let output = cmd.output().await?;
+            if !output.status.success() {
+                return Err(EnvError::VenvFailed(
+                    String::from_utf8_lossy(&output.stderr).to_string(),
+                ));
+            }
         }
         let mut cmd = Command::new(uv_path.as_ref());
-        cmd.arg("venv")
-            .arg("--python")
-            .arg(PYTHON_VERSION.as_str())
-            .arg(venv_path.as_ref());
-        if let Some(cache_path) = cache_path.as_ref() {
-            cmd.arg("--cache-dir").arg(cache_path.as_ref());
-        }
-        color.apply(&mut cmd);
-        let output = cmd.output().await?;
-        if !output.status.success() {
-            return Err(EnvError::VenvFailed(
-                String::from_utf8_lossy(&output.stderr).to_string(),
-            ));
-        }
-        let mut cmd = Command::new(uv_path.as_ref());
-        cmd.env("VIRTUAL_ENV", venv_path.as_ref())
+        cmd.env("VIRTUAL_ENV", path)
             .arg("pip")
             .arg("install")
             .arg("uv")
             .arg("setuptools")
             .arg("wheel")
-            .arg("build");
+            .arg("build>=1.2,<1.3");
         if let Some(cache_path) = cache_path.as_ref() {
             cmd.arg("--cache-dir").arg(cache_path.as_ref());
         }
         color.apply(&mut cmd);
         let output = cmd.output().await?;
         if output.status.success() {
             Ok(())
@@ -326,14 +325,16 @@
     }
 
     pub fn build_package(&self, input: impl AsRef<Path>, output: impl AsRef<Path>) -> Command {
         let mut cmd = self.python_cmd();
         cmd.arg("-m")
             .arg("build")
             .arg("--sdist")
+            .arg("--installer")
+            .arg("uv")
             .arg("--outdir")
             .arg(output.as_ref().as_os_str())
             .arg(input.as_ref().as_os_str());
         cmd
     }
 
     pub fn import_path<'py>(&self, py: Python<'py>, path: &PathStr) -> PyResult<&'py PyAny> {
```

### Comparing `aqora_cli-0.1.8/Cargo.toml` & `aqora_cli-0.1.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/.github/workflows/cd.yaml` & `aqora_cli-0.1.9/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/.github/workflows/ci.yaml` & `aqora_cli-0.1.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/Cargo.lock` & `aqora_cli-0.1.9/Cargo.lock`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/install.py` & `aqora_cli-0.1.9/install.py`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/colors.rs` & `aqora_cli-0.1.9/src/colors.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/clean.rs` & `aqora_cli-0.1.9/src/commands/clean.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/global_args.rs` & `aqora_cli-0.1.9/src/commands/global_args.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/info.rs` & `aqora_cli-0.1.9/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/install.rs` & `aqora_cli-0.1.9/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/login.rs` & `aqora_cli-0.1.9/src/commands/login.rs`

 * *Files 4% similar despite different names*

```diff
@@ -117,18 +117,19 @@
     let router = Router::<ServerState<LoginResponse>>::new()
         .route("/", get(login_callback))
         .with_state(state);
     let authorize_url = global.authorize_url(client_id, &redirect_uri, &session)?;
     let cloned_progress = progress.clone();
     tokio::spawn(async move {
         tokio::time::sleep(std::time::Duration::from_millis(500)).await;
-        cloned_progress.set_message("Opening {authorize_url}...");
+        cloned_progress.set_message(format!("Opening {authorize_url}..."));
         if open::that(authorize_url.as_str()).is_err() {
-            cloned_progress
-                .set_message("Failed to open browser, please open {authorize_url} manually");
+            cloned_progress.set_message(format!(
+                "Failed to open browser, please open {authorize_url} manually"
+            ));
         }
         cloned_progress.set_message("Waiting for browser response...");
     });
     let res = tokio::select! {
         state = rx => state?,
         res = axum::serve(listener, router).with_graceful_shutdown(shutdown_signal()).into_future() => {
             return res.map(|_| None).map_err(|e| {
```

### Comparing `aqora_cli-0.1.8/src/commands/mod.rs` & `aqora_cli-0.1.9/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/python.rs` & `aqora_cli-0.1.9/src/commands/python.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/shell.rs` & `aqora_cli-0.1.9/src/commands/shell.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/template.rs` & `aqora_cli-0.1.9/src/commands/template.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/commands/test.rs` & `aqora_cli-0.1.9/src/commands/test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 use aqora_runner::{
     pipeline::{EvaluateAllInfo, EvaluateInputInfo, EvaluationError, Pipeline, PipelineConfig},
     python::PyEnv,
 };
 use clap::Args;
 use futures::prelude::*;
 use indicatif::{MultiProgress, ProgressBar};
+use owo_colors::{OwoColorize, Stream as OwoStream};
 use pyo3::prelude::*;
 use pyo3::{exceptions::PyException, Python};
 use std::{
     collections::HashMap,
     path::Path,
     pin::Pin,
     sync::{atomic::AtomicU32, Arc},
@@ -150,38 +151,42 @@
         }
         use_case
     };
     let config = PipelineConfig {
         data: data_path.canonicalize()?,
     };
 
-    let mut pipeline_pb = ProgressBar::new_spinner().with_message("Running pipeline...");
+    let mut pipeline_pb = ProgressBar::new_spinner().with_message("Starting pipeline...");
     pipeline_pb.enable_steady_tick(std::time::Duration::from_millis(100));
     pipeline_pb = m.add(pipeline_pb);
 
     let env = init_venv(
         &global.project,
         global.uv.as_ref(),
         &pipeline_pb,
         global.color,
     )
     .await?;
 
+    pipeline_pb.set_message("Importing pipeline..");
+
     let pipeline = match Pipeline::import(&env, &modified_use_case, config) {
         Ok(pipeline) => pipeline,
         Err(err) => {
             pipeline_pb.finish_with_message("Failed to import pipeline");
             Python::with_gil(|py| err.print_and_set_sys_last_vars(py));
             return Err(error::user(
                 "Failed to import pipeline",
                 "Check the above error and try again",
             ));
         }
     };
 
+    pipeline_pb.set_message("Running tests...");
+
     let (num_inputs, generator) = if tests.is_empty() {
         match pipeline.generator() {
             Ok(generator) => {
                 let num_inputs = Arc::new(AtomicU32::new(0));
                 let inputs_cloned = num_inputs.clone();
                 (
                     num_inputs,
@@ -247,15 +252,20 @@
             Some(last_run_dir.clone()),
             None,
             pipeline_pb.clone(),
         ))
         .await
     {
         Ok(Some(score)) => {
-            pipeline_pb.finish_with_message(format!("Done: {score}"));
+            pipeline_pb.println(format!(
+                "{}: {}",
+                "Score".if_supports_color(OwoStream::Stdout, |text| { text.bold() }),
+                score
+            ));
+            pipeline_pb.finish_and_clear();
             Ok(score)
         }
         Ok(None) => {
             pipeline_pb.finish_with_message("Failed to run pipeline");
             Err(error::system(
                 "No score returned. Use case may not have any inputs",
                 "",
```

### Comparing `aqora_cli-0.1.8/src/commands/upload.rs` & `aqora_cli-0.1.9/src/commands/upload.rs`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,15 @@
         &use_case_pb,
         global.color,
     )
     .await?;
 
     let pyproject_toml = std::fs::read_to_string(pyproject_path(&global.project))?;
 
-    let package_name = format!("use-case-{}", competition.id.to_package_id());
+    let package_name = format!("use_case_{}", competition.id.to_package_id());
     let data_path = global.project.join(&config.data);
     if !data_path.exists() {
         return Err(error::user(
             &format!("{} does not exist", data_path.display()),
             "Please make sure the data directory exists",
         ));
     }
@@ -589,29 +589,34 @@
             url
         } else {
             return Err(error::system(
                 "No upload URL found",
                 "This is a bug, please report it",
             ));
         };
-        let package_tar_file = tempdir
-            .path()
-            .join(format!("{package_name}-{version}.tar.gz"));
+        let package_build_path = tempdir.path().join("dist");
+        let package_tar_file = package_build_path.join(format!("{package_name}-{version}.tar.gz"));
         let mut package_pb = ProgressBar::new_spinner().with_message("Building package");
         package_pb.enable_steady_tick(std::time::Duration::from_millis(100));
         package_pb = m.add(package_pb);
 
         let package_pb_cloned = package_pb.clone();
         let client = s3_client.clone();
         async move {
             let project_file = RevertFile::save(pyproject_path(&global.project))?;
             let mut new_project = project.clone();
             new_project.set_name(package_name);
             std::fs::write(&project_file, new_project.toml()?)?;
-            build_package(&env, &global.project, tempdir.path(), &package_pb_cloned).await?;
+            build_package(
+                &env,
+                &global.project,
+                package_build_path,
+                &package_pb_cloned,
+            )
+            .await?;
             project_file.revert()?;
 
             package_pb_cloned.set_message("Uploading package");
             upload_file(&client, package_tar_file, upload_url, "application/gzip").await
         }
         .map(move |res| {
             if res.is_ok() {
@@ -644,14 +649,22 @@
 pub async fn upload_submission(
     args: Upload,
     global: GlobalArgs,
     mut project: PyProject,
 ) -> Result<()> {
     let m = MultiProgress::new();
 
+    let use_case_toml_path = project_use_case_toml_path(&global.project);
+    if !use_case_toml_path.exists() {
+        return Err(error::user(
+            "Project not setup",
+            "Run `aqora install` first.",
+        ));
+    }
+
     project.validate_version().map_err(|err| {
         error::user(
             &format!("Invalid project version: {err}"),
             "Please make sure the project is valid",
         )
     })?;
 
@@ -792,14 +805,15 @@
                 ));
             }
         } else {
             let time = last_run_result.time;
             let mut should_run_tests = false;
             for entry in ignore::WalkBuilder::new(&global.project)
                 .hidden(false)
+                .require_git(false)
                 .build()
                 .skip(1)
                 .flatten()
             {
                 if let Some(modified) = entry.metadata().ok().and_then(|meta| meta.modified().ok())
                 {
                     if chrono::DateTime::<chrono::Utc>::from(modified) > time {
@@ -865,15 +879,15 @@
         .node;
 
     use_case_pb.finish_with_message("Version updated");
 
     let s3_client = reqwest::Client::new();
 
     let package_name = format!(
-        "submission-{}-{}",
+        "submission_{}_{}",
         competition_id.to_package_id(),
         entity_id.to_package_id()
     );
 
     let evaluation_fut = {
         let upload_url = if let Some(url) = project_version
             .files
@@ -940,29 +954,34 @@
             url
         } else {
             return Err(error::system(
                 "No upload URL found",
                 "This is a bug, please report it",
             ));
         };
-        let package_tar_file = tempdir
-            .path()
-            .join(format!("{package_name}-{version}.tar.gz"));
+        let package_build_path = tempdir.path().join("dist");
+        let package_tar_file = package_build_path.join(format!("{package_name}-{version}.tar.gz"));
         let mut package_pb = ProgressBar::new_spinner().with_message("Building package");
         package_pb.enable_steady_tick(std::time::Duration::from_millis(100));
         package_pb = m.add(package_pb);
 
         let package_pb_cloned = package_pb.clone();
         let client = s3_client.clone();
         async move {
             let project_file = RevertFile::save(pyproject_path(&global.project))?;
             let mut new_project = project.clone();
             new_project.set_name(package_name);
             std::fs::write(&project_file, new_project.toml()?)?;
-            build_package(&env, &global.project, tempdir.path(), &package_pb_cloned).await?;
+            build_package(
+                &env,
+                &global.project,
+                package_build_path,
+                &package_pb_cloned,
+            )
+            .await?;
             project_file.revert()?;
 
             package_pb_cloned.set_message("Uploading package");
             upload_file(&client, package_tar_file, upload_url, "application/gzip").await
         }
         .map(move |res| {
             if res.is_ok() {
```

### Comparing `aqora_cli-0.1.8/src/compress.rs` & `aqora_cli-0.1.9/src/compress.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/credentials.rs` & `aqora_cli-0.1.9/src/credentials.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/dirs.rs` & `aqora_cli-0.1.9/src/dirs.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/download.rs` & `aqora_cli-0.1.9/src/download.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/error.rs` & `aqora_cli-0.1.9/src/error.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/evaluate.rs` & `aqora_cli-0.1.9/src/evaluate.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/graphql/schema.graphql` & `aqora_cli-0.1.9/src/graphql/schema.graphql`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/graphql_client.rs` & `aqora_cli-0.1.9/src/graphql_client.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/html/login_response.html` & `aqora_cli-0.1.9/src/html/login_response.html`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/id.rs` & `aqora_cli-0.1.9/src/id.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/manifest.rs` & `aqora_cli-0.1.9/src/manifest.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/process.rs` & `aqora_cli-0.1.9/src/process.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/python.rs` & `aqora_cli-0.1.9/src/python.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/readme.rs` & `aqora_cli-0.1.9/src/readme.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/src/revert_file.rs` & `aqora_cli-0.1.9/src/revert_file.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         let path = path.into();
         let mut tmp_prefix = OsString::from(".");
         tmp_prefix.push(path.file_name().unwrap_or_else(|| "tmp".as_ref()));
         let backed_up = NamedTempFile::with_prefix_in(
             tmp_prefix,
             path.parent().unwrap_or_else(|| ".".as_ref()),
         )?;
-        std::fs::copy(&path, backed_up.path())?;
+        std::fs::rename(&path, backed_up.path())?;
+        std::fs::copy(backed_up.path(), &path)?;
         let mut files = REVERT_FILES.lock().map_err(|_| {
             std::io::Error::new(std::io::ErrorKind::Other, "Could not lock REVERT_FILES")
         })?;
         files.insert(
             path.clone(),
             Self {
                 backed_up,
@@ -39,15 +40,15 @@
         Ok(RevertFileHandle {
             path,
             reverted: false,
         })
     }
 
     fn do_revert(&mut self) -> std::io::Result<()> {
-        std::fs::copy(self.backed_up.path(), &self.path)?;
+        std::fs::rename(self.backed_up.path(), &self.path)?;
         self.reverted = true;
         Ok(())
     }
 
     pub fn revert(mut self) -> std::io::Result<()> {
         self.do_revert()?;
         Ok(())
```

### Comparing `aqora_cli-0.1.8/src/shutdown.rs` & `aqora_cli-0.1.9/src/shutdown.rs`

 * *Files identical despite different names*

### Comparing `aqora_cli-0.1.8/pyproject.toml` & `aqora_cli-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "aqora-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = "The aqora command line interface"
 authors = [{ name = "S.A.S Aqora Quantum", email = "hello@aqora.io" }]
 requires-python = ">=3.8"
 # keywords = []
 # classifiers = []
 
 dependencies = [
```

### Comparing `aqora_cli-0.1.8/PKG-INFO` & `aqora_cli-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aqora-cli
-Version: 0.1.8
+Version: 0.1.9
 Requires-Dist: build >=1.1.1, <2.0.0
 Requires-Dist: setuptools >=61.0
 Requires-Dist: ujson >=5.9.0, <6.0.0
 Requires-Dist: uv >=0.1.18, <0.2.0
 Summary: The aqora command line interface
 Author-email: "S.A.S Aqora Quantum" <hello@aqora.io>
 Requires-Python: >=3.8
```

