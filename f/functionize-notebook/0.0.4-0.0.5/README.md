# Comparing `tmp/functionize_notebook-0.0.4.tar.gz` & `tmp/functionize_notebook-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functionize_notebook-0.0.4.tar", last modified: Sun May 19 14:26:00 2024, max compression
+gzip compressed data, was "functionize_notebook-0.0.5.tar", last modified: Sat May 25 04:17:46 2024, max compression
```

## Comparing `functionize_notebook-0.0.4.tar` & `functionize_notebook-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:26:00.974321 functionize_notebook-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-19 14:26:00.974321 functionize_notebook-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:26:00.974321 functionize_notebook-0.0.4/functionize_notebook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-19 14:26:00.000000 functionize_notebook-0.0.4/functionize_notebook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 14:26:00.000000 functionize_notebook-0.0.4/functionize_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 14:26:00.000000 functionize_notebook-0.0.4/functionize_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 14:26:00.000000 functionize_notebook-0.0.4/functionize_notebook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 14:26:00.000000 functionize_notebook-0.0.4/functionize_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:26:00.974321 functionize_notebook-0.0.4/notebook_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/notebook_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 14:26:00.974321 functionize_notebook-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-19 14:25:52.000000 functionize_notebook-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:17:46.857419 functionize_notebook-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-25 04:17:46.857419 functionize_notebook-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:17:46.857419 functionize_notebook-0.0.5/functionize_notebook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-25 04:17:46.000000 functionize_notebook-0.0.5/functionize_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-25 04:17:46.000000 functionize_notebook-0.0.5/functionize_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 04:17:46.000000 functionize_notebook-0.0.5/functionize_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 04:17:46.000000 functionize_notebook-0.0.5/functionize_notebook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 04:17:46.000000 functionize_notebook-0.0.5/functionize_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:17:46.857419 functionize_notebook-0.0.5/notebook_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/notebook_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 04:17:46.861420 functionize_notebook-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-25 04:17:42.000000 functionize_notebook-0.0.5/setup.py
```

### Comparing `functionize_notebook-0.0.4/LICENSE.txt` & `functionize_notebook-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `functionize_notebook-0.0.4/PKG-INFO` & `functionize_notebook-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.4
+Version: 0.0.5
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -59,10 +59,22 @@
 ```Python
 sum = calculateSum(5, 10, a = 8, c = 9)
 ```
 This will overide value of a. Now a = 8. Variable c = 9 is also injected to notebook.
 
 You can also pass other datatype. However, Any modifications made by notebook won't be reflected on the object. You can still return the object to get the modifications.
 
+## Export notebook
+
+Example: You want to rerun notebook with different inputs.
+
+```Python
+for i in range(100):
+   calculateSum.export(f"outputNb-{str(i)}.ipynb", 5 * i, 10 + i)
+
+```
+
+`export` return the same result with running normally.
+
 More information and code samples available in the [examples folder](./examples/).
```

### Comparing `functionize_notebook-0.0.4/README.md` & `functionize_notebook-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -44,10 +44,22 @@
 ```Python
 sum = calculateSum(5, 10, a = 8, c = 9)
 ```
 This will overide value of a. Now a = 8. Variable c = 9 is also injected to notebook.
 
 You can also pass other datatype. However, Any modifications made by notebook won't be reflected on the object. You can still return the object to get the modifications.
 
+## Export notebook
+
+Example: You want to rerun notebook with different inputs.
+
+```Python
+for i in range(100):
+   calculateSum.export(f"outputNb-{str(i)}.ipynb", 5 * i, 10 + i)
+
+```
+
+`export` return the same result with running normally.
+
 More information and code samples available in the [examples folder](./examples/).
```

### Comparing `functionize_notebook-0.0.4/functionize_notebook.egg-info/PKG-INFO` & `functionize_notebook-0.0.5/functionize_notebook.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.4
+Version: 0.0.5
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -59,10 +59,22 @@
 ```Python
 sum = calculateSum(5, 10, a = 8, c = 9)
 ```
 This will overide value of a. Now a = 8. Variable c = 9 is also injected to notebook.
 
 You can also pass other datatype. However, Any modifications made by notebook won't be reflected on the object. You can still return the object to get the modifications.
 
+## Export notebook
+
+Example: You want to rerun notebook with different inputs.
+
+```Python
+for i in range(100):
+   calculateSum.export(f"outputNb-{str(i)}.ipynb", 5 * i, 10 + i)
+
+```
+
+`export` return the same result with running normally.
+
 More information and code samples available in the [examples folder](./examples/).
```

### Comparing `functionize_notebook-0.0.4/notebook_wrapper/__init__.py` & `functionize_notebook-0.0.5/notebook_wrapper/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,20 +32,27 @@
 
         pass
 
     def __call__(self, *args, **kwargs):
         return self.run(*args, *kwargs)
 
     def run(self, *args, **kwargs) -> Any | List[Any]:
+        return self.export(None, *args, **kwargs)
+
+    def export(self, _outputNotebook: str | Path | None, *args, **kwargs):
+        if isinstance(_outputNotebook, str):
+            _outputNotebook = Path(_outputNotebook)
+
         # map input
         variableMapping = dict(zip(self.inputVariable, args))
         variableMapping.update(kwargs)
 
         nb = nbformat.read(self.notebook, as_version=nbformat.NO_CONVERT)
 
+        inputIndex = -1
         if len(variableMapping) > 0:
             # add saving path for input
             inputPath = Path(
                 tempfile.gettempdir(),
                 "BHTuNbWrapper",
                 self.notebook.stem,
                 "input",
@@ -60,72 +67,57 @@
                 if inputPath.exists():
                     break
                 else:
                     sleep(0.2)
             else:
                 raise IOError(inputPath.__str__() + " took too much time to write.")
 
-            # identify input cell
-            inputIndex = 0
-            for i, cell in enumerate(nb.cells):
-                if "tags" in cell.metadata and self.inputTag in cell.metadata["tags"]:
-                    inputIndex = i
-                    break
-                pass
-
-            # add input cell to nb
-            newCell = nbbase.new_code_cell(
-                source="""
-                from pathlib import Path
-                import pickle
-                
-                inputVariables = pickle.loads(Path("%s").read_bytes())
-                for key, value in inputVariables.items():
-                    globals()[key] = value
-                    pass
-            """
-                % inputPath
-            )
-
-            nb.cells.insert(inputIndex + 1, newCell)
+            inputIndex = self._insertInputCell(inputPath)
 
+        outputIndex = -1
         if self.outputVariable is not None:
             # add saving path for output
             outputPath = Path(
                 tempfile.gettempdir(),
                 "BHTuNbWrapper",
                 self.notebook.stem,
                 "output",
                 datetime.now().__str__() + ".pkl",
             )
             outputPath.parent.mkdir(parents=True, exist_ok=True)
 
-            # add output cell to nb
-            if isinstance(self.outputVariable, List):
-                requestVars = "[" + ",".join(self.outputVariable) + "]"
-            else:
-                requestVars = self.outputVariable
-
-            newCell = nbbase.new_code_cell(
-                source="""
-                from pathlib import Path
-                import pickle
-                
-                outputVariable = %s
-                Path("%s").write_bytes(pickle.dumps(outputVariable))
-            """
-                % (requestVars, outputPath)
-            )
-
-            nb.cells.append(newCell)
+            outputIndex = self._insertOutputCell(outputPath)
             pass
 
         ep = ExecutePreprocessor(timeout=None)
         resultNb, _ = ep.preprocess(nb, {"metadata": {"path": self.notebook.parent}})
 
+        if _outputNotebook is not None:
+            if inputIndex >= 0:
+                resultNb.cells.pop(inputIndex)
+
+                # Add markdown cell noting injected variables
+                mdText = "`functionize-notebook` has modified this notebook during execution. The following variables have been injected:\n\n"
+                for variable, varValue in variableMapping.items():
+                    try:
+                        varStr = str(varValue)
+                    except Exception:
+                        varStr = "This variable could not be represent in text."
+                    mdText += f"- {variable}: {varStr}\n"
+                
+                mdCell = nbbase.new_markdown_cell(source=mdText)
+                resultNb.cells.insert(inputIndex, mdCell)
+                
+            if outputIndex >= 0:
+                resultNb.cells.pop(outputIndex)
+
+            with open(_outputNotebook, "w") as f:
+                nbformat.write(resultNb, f)
+                pass
+
         if self.outputVariable is not None:
             # wait for nb output
             for _ in range(50):
                 if outputPath.exists():
                     break
                 else:
                     sleep(0.2)
@@ -133,7 +125,60 @@
                 raise IOError(outputPath.__str__() + " took too much time to write.")
 
             res = pickle.loads(outputPath.read_bytes())
 
             return res
         else:
             return None
+
+    def _insertInputCell(self, inputPath: Path):
+        nb = nbformat.read(self.notebook, as_version=nbformat.NO_CONVERT)
+
+        # identify input cell
+        inputIndex = 0
+        for i, cell in enumerate(nb.cells):
+            if "tags" in cell.metadata and self.inputTag in cell.metadata["tags"]:
+                inputIndex = i
+                break
+            pass
+
+        newCell = nbbase.new_code_cell(
+            source="""
+                from pathlib import Path
+                import pickle
+                
+                inputVariables = pickle.loads(Path("%s").read_bytes())
+                for key, value in inputVariables.items():
+                    globals()[key] = value
+                    pass
+            """
+            % inputPath
+        )
+
+        nb.cells.insert(inputIndex + 1, newCell)
+
+        return inputIndex + 1
+
+    def _insertOutputCell(
+        self,
+        outputPath: Path,
+    ):
+        nb = nbformat.read(self.notebook, as_version=nbformat.NO_CONVERT)
+
+        if isinstance(self.outputVariable, List):
+            requestVars = "[" + ",".join(self.outputVariable) + "]"
+        else:
+            requestVars = self.outputVariable
+        newCell = nbbase.new_code_cell(
+            source="""
+                from pathlib import Path
+                import pickle
+                
+                outputVariable = %s
+                Path("%s").write_bytes(pickle.dumps(outputVariable))
+            """
+            % (requestVars, outputPath)
+        )
+
+        nb.cells.append(newCell)
+
+        return len(nb.cells) - 1
```

### Comparing `functionize_notebook-0.0.4/setup.py` & `functionize_notebook-0.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from distutils.core import setup
 from setuptools import find_packages
 
+
+version = "0.0.1"
+# Extract version from CHANGES.md
+with open("./CHANGES.md", "r") as file:
+        for line in file:
+            if line.strip():
+                version = line.strip()
+                break
+
+
 setup(
     name="functionize-notebook",
-    version="0.0.4",
+    version=version,
     author="Bui Hoang Tu",
     author_email="bhtu.work@gmail.com",
     url="https://github.com/BuiHoangTu/functionize-notebook/tree/release",
     license="MIT",
     packages=find_packages(),
     package_dir={"notebook_wrapper": "notebook_wrapper"},
     description="run notebook like a function",
```

