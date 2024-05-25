# Comparing `tmp/jeddinformatics-0.5.1.tar.gz` & `tmp/jeddinformatics-0.6.1.tar.gz`

## Comparing `jeddinformatics-0.5.1.tar` & `jeddinformatics-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/requirements.txt
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/.github/workflows/lint_and_test_and_deploy.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/.dirignore
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/.fileignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/__main__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/config.json
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/convert_and_plot.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/generate_types.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/highchart_json_to_csv.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/oncodb_to_csv.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/plot_data.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/src/jeddinformatics/schema.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/tests/test_stub.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/.gitignore
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/LICENSE
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 jeddinformatics-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/requirements.txt
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/.github/workflows/lint_and_test_and_deploy.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/.dirignore
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/.fileignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/__main__.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/config.json
+-rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/convert_and_plot.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/generate_types.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/highchart_json_to_csv.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/oncodb_to_csv.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/plot_data.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/src/jeddinformatics/schema.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/tests/test_stub.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/README.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 jeddinformatics-0.6.1/PKG-INFO
```

### Comparing `jeddinformatics-0.5.1/.github/workflows/lint_and_test_and_deploy.yml` & `jeddinformatics-0.6.1/.github/workflows/lint_and_test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `jeddinformatics-0.5.1/src/jeddinformatics/config.json` & `jeddinformatics-0.6.1/src/jeddinformatics/config.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {"'mappings'": "{'log2(TPM)': 'log<sub>2</sub>(TPM)'}"}*

```diff
@@ -13,15 +13,15 @@
     "mappings": {
         "Normal": "NC",
         "OV": "OV",
         "Ovarian Cancer": "OV",
         "Some title": "Translated title",
         "UCEC": "UCEC",
         "Uterine Cancer": "UCEC",
-        "log2(TPM)": "log\u2082(TPM)",
+        "log2(TPM)": "log<sub>2</sub>(TPM)",
         "normal": "NC"
     },
     "plot_height": 540,
     "plot_width": 960,
     "point_size": 6,
     "precedence": [
         "NC",
```

### Comparing `jeddinformatics-0.5.1/src/jeddinformatics/convert_and_plot.py` & `jeddinformatics-0.6.1/src/jeddinformatics/convert_and_plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -177,14 +177,15 @@
             ignored_dir_patterns = [line.strip() for line in ignore_dir_file]
     except Exception as e:
         logger.warning(
             f"ignored dirs '{ignored_dir_patterns}' couldn't be parsed with {e}, using default of none"
         )
         ignored_dir_patterns = []
 
+    merged_cancer_sources: dict[str: list[str]] = {}
     for root, _, files in os.walk(root_directory):
         for file in files:
             file_path: str = os.path.join(root, file)
             matching_ignored_file_patterns = [
                 ignored_file_pattern
                 for ignored_file_pattern in ignored_file_patterns
                 if fnmatch.fnmatch(file, ignored_file_pattern)
@@ -235,26 +236,43 @@
                 process_txt(
                     file_path=file_path,
                     config=config,
                     cancer_type=cancer_type,
                     is_gene=is_gene,
                 )
                 count_txt += 1
+
+            if file == "data.csv":
+                dest = os.sep.join(path_components[0:-2])
+                prev = merged_cancer_sources.get(dest, [])
+                prev.append(file_path)
+                merged_cancer_sources.update({dest: prev})
     logger.info(
         f"finished processing {count_json} JSON files and {count_txt} TXT files"
     )
+    for source in merged_cancer_sources:
+        plot_data.plot_formatted_csvs(
+            config=config,
+            inputs=merged_cancer_sources[source],
+            output=f"{source}/merged.png",
+            translation_func=translate_in_mapping,
+            cancer_type=source.split(os.sep)[-1],
+            is_gene=source.split(os.sep)[-3].lower().find("gene") != -1,
+        )
 
 
 # Assumed structure:
 # ```
 #  {gene or protein expression}
 #   └───{source database}
 #        └───{type of cancer}
-#             └───{gene or protein name}
-#                  └───{data.json or data.txt}
+#             |───{gene or protein name}
+#             |    |───{graph per graph or protein}
+#             |    └───{data.json or data.txt}
+#             └───{merged graph per cancer in database}
 # ```
 
 
 def main():
     with logger.catch(onerror=lambda _: sys.exit(1)):
         logger.remove(0)
         logger.add(sys.stdout, level="INFO")
```

### Comparing `jeddinformatics-0.5.1/src/jeddinformatics/highchart_json_to_csv.py` & `jeddinformatics-0.6.1/src/jeddinformatics/highchart_json_to_csv.py`

 * *Files identical despite different names*

### Comparing `jeddinformatics-0.5.1/src/jeddinformatics/oncodb_to_csv.py` & `jeddinformatics-0.6.1/src/jeddinformatics/oncodb_to_csv.py`

 * *Files identical despite different names*

### Comparing `jeddinformatics-0.5.1/src/jeddinformatics/schema.json` & `jeddinformatics-0.6.1/src/jeddinformatics/schema.json`

 * *Files identical despite different names*

### Comparing `jeddinformatics-0.5.1/.gitignore` & `jeddinformatics-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jeddinformatics-0.5.1/LICENSE` & `jeddinformatics-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jeddinformatics-0.5.1/README.md` & `jeddinformatics-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,27 @@
 This will install the required packages
 
 ## Running on errything
 ```bash
 python3 main.py <your data folder>
 ```
 
-## TODO
-- [ ] make sure non cancer is always first
-- [ ] change boxes and whiskers to be a different colour
-- [ ] remove shading
-
 ## Config files
 ```json
 {
     "$schema": "https://raw.githubusercontent.com/wolffshots/jeddinformatics/main/src/jeddinformatics/schema.json",
     "mappings": {
         "normal": "NC",
         "Normal": "NC",
         "OV": "OV",
         "UCEC": "UCEC",
         "Ovarian Cancer": "OV",
         "Uterine Cancer": "UCEC",
         "Some title": "Translated title",
-        "log2(TPM)": "log₂(TPM)"
+        "log2(TPM)": "log<sub>2</sub>(TPM)"
     },
     "colors": {
         "NC": "blue",
         "OV": "green",
         "UCEC": "red",
         "box": "black",
         "plot_background_color": "lightgray",
```

### Comparing `jeddinformatics-0.5.1/pyproject.toml` & `jeddinformatics-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jeddinformatics"
-version = "0.5.1"
+version = "0.6.1"
 author = [
   { name="jadon", email="16850875+wolffshots@users.noreply.github.com" }
 ]
 description = "Convert bioinformatics data to plots"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `jeddinformatics-0.5.1/PKG-INFO` & `jeddinformatics-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jeddinformatics
-Version: 0.5.1
+Version: 0.6.1
 Summary: Convert bioinformatics data to plots
 Project-URL: Homepage, https://github.com/wolffshots/jeddinformatics
 Project-URL: Issues, https://github.com/wolffshots/jeddinformatics/issues
 License-File: LICENSE
 Keywords: bioinformatics,plotly
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -28,32 +28,27 @@
 This will install the required packages
 
 ## Running on errything
 ```bash
 python3 main.py <your data folder>
 ```
 
-## TODO
-- [ ] make sure non cancer is always first
-- [ ] change boxes and whiskers to be a different colour
-- [ ] remove shading
-
 ## Config files
 ```json
 {
     "$schema": "https://raw.githubusercontent.com/wolffshots/jeddinformatics/main/src/jeddinformatics/schema.json",
     "mappings": {
         "normal": "NC",
         "Normal": "NC",
         "OV": "OV",
         "UCEC": "UCEC",
         "Ovarian Cancer": "OV",
         "Uterine Cancer": "UCEC",
         "Some title": "Translated title",
-        "log2(TPM)": "log₂(TPM)"
+        "log2(TPM)": "log<sub>2</sub>(TPM)"
     },
     "colors": {
         "NC": "blue",
         "OV": "green",
         "UCEC": "red",
         "box": "black",
         "plot_background_color": "lightgray",
```

