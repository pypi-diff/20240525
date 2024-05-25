# Comparing `tmp/pacspeddbase-0.1.0.tar.gz` & `tmp/pacspeddbase-0.2.tar.gz`

## Comparing `pacspeddbase-0.1.0.tar` & `pacspeddbase-0.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      249 1970-01-01 00:00:00.000000 pacspeddbase-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-05-24 17:43:49.000000 pacspeddbase-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-24 17:43:49.000000 pacspeddbase-0.1.0/.gitignore
--rw-r--r--   0     1001      127     9435 2024-05-24 17:43:49.000000 pacspeddbase-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     1117 2024-05-24 17:43:49.000000 pacspeddbase-0.1.0/upload-pypi.py
--rw-r--r--   0     1001      127     8094 2024-05-24 17:43:49.000000 pacspeddbase-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      392 2024-05-24 17:43:49.000000 pacspeddbase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 pacspeddbase-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      249 1970-01-01 00:00:00.000000 pacspeddbase-0.2/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-05-25 08:09:45.000000 pacspeddbase-0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-25 08:09:45.000000 pacspeddbase-0.2/.gitignore
+-rw-r--r--   0     1001      127    11951 2024-05-25 08:09:45.000000 pacspeddbase-0.2/README.rst
+-rwxr-xr-x   0     1001      127  7427504 2024-05-25 08:09:45.000000 pacspeddbase-0.2/scripts/ubuntu-amd64/upload-pypi
+-rw-r--r--   0     1001      127     1212 2024-05-25 08:09:45.000000 pacspeddbase-0.2/scripts/upload-pypi.py
+-rw-r--r--   0     1001      127    11114 2024-05-25 08:09:45.000000 pacspeddbase-0.2/src/lib.rs
+-rw-r--r--   0     1001      127     8094 2024-05-25 08:09:45.000000 pacspeddbase-0.2/Cargo.lock
+-rw-r--r--   0     1001      127      408 2024-05-25 08:09:45.000000 pacspeddbase-0.2/pyproject.toml
+-rw-r--r--   0        0        0    12264 1970-01-01 00:00:00.000000 pacspeddbase-0.2/PKG-INFO
```

### Comparing `pacspeddbase-0.1.0/.github/workflows/CI.yml` & `pacspeddbase-0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pacspeddbase-0.1.0/.gitignore` & `pacspeddbase-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pacspeddbase-0.1.0/src/lib.rs` & `pacspeddbase-0.2/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -251,14 +251,63 @@
                 .stderr(Stdio::inherit())
                 .output()
                 .map_err(|e| pyo3::exceptions::PyRuntimeError::new_err(format!("Failed to Copy Files: {}", e)))?
         };
         Ok(())
     }
 
+    /// List Files in Dir, but in Better output
+    /// 
+    /// Args:
+    ///     path: The Path That you want Show
+    fn listdir(&self, path: &str) -> PyResult<()> {
+        let _output = if cfg!(target_os = "windows") {
+            Command::new("dir")
+                .arg(path)
+                .stdout(Stdio::inherit())
+                .stderr(Stdio::inherit())
+                .output()
+                .map_err(|e| pyo3::exceptions::PyRuntimeError::new_err(format!("Failed to List Files: {}", e)))?
+        } else {
+            Command::new("ls")
+                .arg("-A")
+                .arg(path)
+                .stdout(Stdio::inherit())
+                .stderr(Stdio::inherit())
+                .output()
+                .map_err(|e| pyo3::exceptions::PyRuntimeError::new_err(format!("Failed to List Files: {}", e)))?
+        };
+
+        Ok(())
+    }
+
+    /// Source/Call files
+    /// 
+    /// Args:
+    ///  Path (str): The Path to Source
+    fn source(&self, path: &str) -> PyResult<()> {
+        let _output = if cfg!(target_os = "windows") {
+            Command::new("call")
+                .arg(path)
+                .stdout(Stdio::inherit())
+                .stderr(Stdio::inherit())
+                .output()
+                .map_err(|e| pyo3::exceptions::PyRuntimeError::new_err(format!("Failed to Call File: {}", e)))?
+        } else {
+            Command::new("source")
+                .arg(path)
+                .stdout(Stdio::inherit())
+                .stderr(Stdio::inherit())
+                .output()
+                .map_err(|e| pyo3::exceptions::PyRuntimeError::new_err(format!("Failed to Source File: {}", e)))?
+        };
+
+        Ok(())
+    }
+
 }
 
 #[pyclass]
 struct Args {}
 
 #[pymethods]
 impl Args {
```

### Comparing `pacspeddbase-0.1.0/upload-pypi.py` & `pacspeddbase-0.2/scripts/upload-pypi.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 if __name__ == '__main__':
     option = sys.argv[1]
     if option in ['view', 'show', 'list']:
         subprocess.run(['gh', 'workflow', 'view'])
     elif option in ['setup', 'pypi']:
         subprocess.run(['python', '-m', 'pip', 'install', 'twine'])
         token = sys.argv[2]
-        HOME = os.environ.get(['HOME'])
+        HOME = os.environ.get('HOME')
         PYPIRC = os.path.join(HOME, '.pypirc')
         with open(PYPIRC, 'w') as f:
-            text1 = "[pypi]"
-            text2 = "username = __token__"
-            text3 = f"password = {token}"
+            text1 = "[pypi]\n"
+            text2 = "username = __token__\n"
+            text3 = f"password = {token}\n"
             f.write(text1)
             f.write(text2)
             f.write(text3)
     elif option in ['upload', 'publish']:
         pid = sys.argv[2]
         cdir = os.getcwd()
         build = os.path.join(cdir, 'build')
+        os.makedirs(build, exist_ok=True)
         os.chdir(build)
         subprocess.run(['gh', 'run', 'download', pid])
         folder = os.listdir(build)
         for fold in folder:
             files = os.listdir(fold)
             for file in files:
                 filepath = os.path.join(fold, file)
-                subprocess.run(['python', '-m', 'twine', 'upload', filepath])
+                subprocess.run(['python', '-m', 'twine', 'upload', filepath])
+        os.chdir(cdir)
+        os.remove(build)
```

### Comparing `pacspeddbase-0.1.0/Cargo.lock` & `pacspeddbase-0.2/Cargo.lock`

 * *Files identical despite different names*

