# Comparing `tmp/reasoner_validator-4.2.0.tar.gz` & `tmp/reasoner_validator-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.2.0.tar", max compression
+gzip compressed data, was "reasoner_validator-4.2.1.tar", max compression
```

## Comparing `reasoner_validator-4.2.0.tar` & `reasoner_validator-4.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1153 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/README.md
--rw-r--r--   0        0        0      131 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    43520 2024-05-18 00:03:47.909612 reasoner_validator-4.2.0/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2368 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    97394 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0     4264 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/biolink/ontology.py
--rw-r--r--   0        0        0    47438 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/github.py
--rw-r--r--   0        0        0     3995 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/message.py
--rw-r--r--   0        0        0    47007 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/report.py
--rw-r--r--   0        0        0    15057 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0     4754 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/utils/__init__.py
--rw-r--r--   0        0        0      886 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/utils/http.py
--rw-r--r--   0        0        0    14745 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    38175 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3594 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/tests/conftest.py
--rw-r--r--   0        0        0   151988 2024-05-18 00:03:47.913612 reasoner_validator-4.2.0/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0     2268 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_ontology.py
--rw-r--r--   0        0        0    49075 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_semver.py
--rw-r--r--   0        0        0     2327 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36726 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_validate.py
--rw-r--r--   0        0        0    30435 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_validation_report.py
--rw-r--r--   0        0        0     3421 2024-05-18 00:03:47.917612 reasoner_validator-4.2.0/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/README.md
+-rw-r--r--   0        0        0      131 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    43781 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2368 2024-05-24 19:36:52.212980 reasoner_validator-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    97394 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0     4264 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/biolink/ontology.py
+-rw-r--r--   0        0        0    47770 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3995 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/message.py
+-rw-r--r--   0        0        0    47007 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/report.py
+-rw-r--r--   0        0        0    15057 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0     4754 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/utils/__init__.py
+-rw-r--r--   0        0        0      886 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/utils/http.py
+-rw-r--r--   0        0        0    14745 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    42668 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3594 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/tests/conftest.py
+-rw-r--r--   0        0        0   151988 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-24 19:36:52.216980 reasoner_validator-4.2.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0     3204 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_ontology.py
+-rw-r--r--   0        0        0    50742 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_semver.py
+-rw-r--r--   0        0        0     2327 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36726 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_validate.py
+-rw-r--r--   0        0        0    30435 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-24 19:36:52.220980 reasoner_validator-4.2.1/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.2.1/PKG-INFO
```

### Comparing `reasoner_validator-4.2.0/LICENSE` & `reasoner_validator-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/README.md` & `reasoner_validator-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/docs/Makefile` & `reasoner_validator-4.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/docs/conf.py` & `reasoner_validator-4.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/docs/index.rst` & `reasoner_validator-4.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/docs/make.bat` & `reasoner_validator-4.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/docs/validation_codes_dictionary.md` & `reasoner_validator-4.2.1/docs/validation_codes_dictionary.md`

 * *Files 0% similar despite different names*

```diff
@@ -898,14 +898,20 @@
 
 ### warning.trapi.response.message.knowledge_graph.empty
 
 **Message:** Response returned an empty Message Knowledge Graph?
 
 **Description:** An empty Knowledge Graph is allowed but merits a boundary response warning?
 
+### warning.trapi.response.message.knowledge_graph.node.category.imprecise
+
+**Message:** The category of the knowledge graph node matching an input node identifier is more generic than expected.
+
+**Context:** identifier, expected_category, observed_categories
+
 ### warning.trapi.response.message.results.empty
 
 **Message:** Response returned empty Message.results?
 
 **Description:** Empty Results is allowed but merits a boundary response warning?
 
 ### warning.trapi.response.workflow.runner_parameters.missing
```

### Comparing `reasoner_validator-4.2.0/pyproject.toml` & `reasoner_validator-4.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.2.0"
+version = "4.2.1"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.2.0/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.2.1/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/biolink/ontology.py` & `reasoner_validator-4.2.1/reasoner_validator/biolink/ontology.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/codes.yaml` & `reasoner_validator-4.2.1/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -690,14 +690,22 @@
           $message: "TRAPI Response is missing its Biolink Model version"
           $description:  "The TRAPI Response should specify its Biolink Model version compliance."
       message:
         knowledge_graph:
           empty:
             $message: "Response returned an empty Message Knowledge Graph?"
             $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
+          node:
+            category:
+              imprecise:
+                $message: "The category of the knowledge graph node matching an input node identifier is more generic than expected."
+                $context:
+                  - identifier
+                  - expected_category
+                  - observed_categories
         results:
           empty:
             $message: "Response returned empty Message.results?"
             $description: "Empty Results is allowed but merits a boundary response warning?"
       workflow:
         runner_parameters:
           missing:
```

### Comparing `reasoner_validator-4.2.0/reasoner_validator/github.py` & `reasoner_validator-4.2.1/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/message.py` & `reasoner_validator-4.2.1/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/report.py` & `reasoner_validator-4.2.1/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.2.1/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.2.1/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/utils/__init__.py` & `reasoner_validator-4.2.1/reasoner_validator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/utils/http.py` & `reasoner_validator-4.2.1/reasoner_validator/utils/http.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/validation_codes.py` & `reasoner_validator-4.2.1/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/validator.py` & `reasoner_validator-4.2.1/reasoner_validator/validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Tuple, List, Dict
+from typing import Optional, Tuple, List, Dict, Set
 
 from reasoner_validator.biolink import (
     BiolinkValidator,
     get_biolink_model_toolkit
 )
 
 from reasoner_validator.report import TRAPIGraphType
@@ -62,15 +62,15 @@
             strict_validation=strict_validation
         )
         self._is_trapi_1_4_or_later: Optional[bool] = None
         self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
 
     def is_trapi_1_4_or_later(self) -> bool:
         assert self.trapi_version
-        try:  # try block ... Sanity check: in case the trapi_version is somehow invalid?
+        try:  # try block ... Sanity check: in testcase the trapi_version is somehow invalid?
             target_major_version: SemVer = \
                 SemVer.from_string(self.trapi_version, core_fields=['major', 'minor'],  ext_fields=[])
             self._is_trapi_1_4_or_later = target_major_version >= TRAPI_1_4_0_SEMVER
         except SemVerError as sve:
             logger.error(f"Current TRAPI release '{self.trapi_version}' seems invalid: {str(sve)}. Reset to latest?")
             self.trapi_version = LATEST_TRAPI_RELEASE
             self._is_trapi_1_4_or_later = True
@@ -398,71 +398,122 @@
                     # The 'output_node_binding' is (subject) 'a' or (object) 'b' keys in
                     # the QueryGraph.Nodes to be bound
                     # In principle, we detect which node in the QueryGraph has 'ids' associated with its node record
                     # and assume that the other edge node is the desired target (in the OneHop), so the 'ids'
                     # there should be in the output
 
                     # object_ids = [r['node_bindings'][output_node_binding][0]['id'] for r in results_sample]
-                    # if case[output_element] not in object_ids:
+                    # if testcase[output_element] not in object_ids:
                     #     # The 'get_aliases' method uses the Translator NodeNormalizer to check if any of
-                    #     # the aliases of the case[output_element] identifier are in the object_ids list
-                    #     output_aliases = get_aliases(case[output_element])
+                    #     # the aliases of the testcase[output_element] identifier are in the object_ids list
+                    #     output_aliases = get_aliases(testcase[output_element])
                     #     if not any([alias == object_id for alias in output_aliases for object_id in object_ids]):
                     #         validator.report(
                     #             code=error.results.missing_bindings,
-                    #             identifier=case[output_element],
+                    #             identifier=testcase[output_element],
                     #             output_node_binding=output_node_binding
                     #         )
                     #         # data_dump=f"Resolved aliases:\n{','.join(output_aliases)}\n" +
                     #         #           f"Result object IDs:\n{_output(object_ids,flat=True)}"
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
-    def case_node_found(self, target: str, identifiers: List[str], case: Dict, nodes: Dict) -> bool:
+    def category_matched(self, source_categories: List[str], target_categories: List[str]) -> bool:
         """
-        Check for presence of the target identifier,
-        with expected categories, in the "nodes" catalog.
+        For each 'source' Biolink Model category given (list of CURIEs as strings?),
+        first get the union set of all parent (ancestral) categories, then check if
+        at least one of these categories is matched to the list of target categories.
+
+        :param source_categories: List[str], list of 'source' categories whose category hierarchy is to be matched.
+        :param target_categories: List[str], list of 'target' categories to be matched against 'source'
+                                             (or 'source parent' categories
+        :return: bool, True if a category match is found (as described above)
+        """
+        source_category_set: Set = set()
+        # gather all the possible exact and ancestor (parent)
+        # categories of source_categories to match...
+        for source_category in source_categories:
+            source_category_set.update(self.bmt.get_ancestors(source_category, formatted=True, mixin=False))
+        # ...then check all the target categories against that source category set
+        return any([c in target_categories for c in source_category_set])
+
+    def testcase_node_found(self, target: str, identifiers: List[str], testcase: Dict, nodes: Dict) -> bool:
+        """
+        Check for presence of the target identifier, with expected categories, in the "nodes" catalog.
+        If the identifier is found, and at least one KG node category is the expected category or a proper subclass
+        category of the test testcase category, then return True; if the node is found but the testcase category is not
+        the expected category but is a subclass category of the KG node categories (i.e. KG node categories
+        are too general), then return False. If the identifier is NOT found in the nodes list or
+        there is no overlap in the (expected or parent) testcase and node categories, then return False.
 
         :param target: 'subject' or 'object'
         :param identifiers: List of node (CURIE) identifiers to be checked in the "nodes" catalog
-        :param case: Dict, full test case (to access the target node 'category')
+        :param testcase: Dict, full test testcase (to access the target node 'category')
         :param nodes: Dict, nodes category indexed by node identifiers.
-        :return:
+        :return: bool, True if feasible node identifier and category match; False otherwise
         """
         #
         #     "nodes": {
         #         "MONDO:0005148": {"name": "type-2 diabetes"},
         #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
         #     }
         #
 
         # Sanity check
         assert target in ["subject", "object"]
         for identifier in identifiers:
             if identifier in nodes.keys():
-                # Found the target node identifier,
-                # but is the expected category present?
+                # Found the target node identifier, but is the expected category present?
+                # For this comparison, we assume that a specified node category plus all its
+                # parent categories, may be used to match the test testcase specified category.
                 node_details = nodes[identifier]
+                test_case_category: str = testcase[f"{target}_category"]
                 if "categories" in node_details:
-                    category = case[f"{target}_category"]
-                    categories: List[str] = self.bmt.get_ancestors(category, formatted=True, mixin=False)
-                    if any([c in node_details["categories"] for c in categories]):
+                    if self.category_matched(
+                            source_categories=node_details["categories"],
+                            target_categories=[test_case_category]
+                    ):
+                        # The 'identifier' was present in the list of KG nodes, plus there was a match of the target
+                        # testcase category either exactly to a specified one of the indicated KG node categories or to
+                        # an ancestral ("parent") category of one of the node categories. This is a completely regular
+                        # result. For example, if a KG node return is "biolink:Gene", but the testcase query is only
+                        # expecting to see a "biolink:BiologicalEntity", however, since the identifier is matched
+                        # exactly, since the node match is good with greater categorical precision than expected.
+                        return True
+                    elif self.category_matched(
+                            source_categories=[test_case_category],
+                            target_categories=node_details["categories"]
+                    ):
+                        # The 'identifier' was present in the list of KG nodes;
+                        # however, there was likely only a more general ("parent-level") category match
+                        # of at least one of the KG node categories, to a parent category of the testcase category
+                        # (since the 'exact match' match scenario was handled above). This is a less precise
+                        # node match, hence we issue a warning. For example, maybe the KG node returned is only
+                        # tagged as "biolink:NamedThing" but we are looking for a testcase with "biolink:Gene".
+                        # Since the testcase identifier was matched exactly, we assume that the node is matched,
+                        # but just with less than desired data type categorical precision.
+                        self.report(
+                            code="warning.trapi.response.message.knowledge_graph.node.category.imprecise",
+                            identifier=identifier,
+                            expected_category=test_case_category,
+                            observed_categories=",".join(node_details["categories"])
+                        )
                         return True
 
-        # Target node identifier or categories is missing,
-        # or not annotated with the expected category?
+        # Target node identifier is missing from the list of KG nodes or categories is either missing
+        # or not annotated with any compatible category, hence, we deem the node effectively missing.
         return False
 
     @staticmethod
-    def case_edge_bindings(q_edge_ids: Tuple[str], target_edge_id: str, data: Dict) -> bool:
+    def testcase_edge_bindings(q_edge_ids: List[str], target_edge_id: str, data: Dict) -> bool:
         """
         Check if target query edge id and knowledge graph edge id are in specified edge_bindings.
         :rtype: object
-        :param q_edge_ids: Tuple[str], expected query edge identifiers in a matching result
+        :param q_edge_ids: List[str], expected query edge identifiers in a matching result
         :param target_edge_id:  str, expected knowledge edge identifier in a matching result
         :param data: TRAPI version-specific Response context from which the 'edge_bindings' may be retrieved
         :return: True, if found
         """
         edge_bindings: Dict = data["edge_bindings"]
         for bound_query_id, edge in edge_bindings.items():
             if bound_query_id in q_edge_ids:
@@ -470,34 +521,34 @@
                     # TRAPI schema validation actually
                     # catches missing id's, but sanity check...
                     if "id" in binding_details:
                         if target_edge_id == binding_details["id"]:
                             return True
         return False
 
-    def case_result_found(
+    def testcase_result_found(
             self,
             query_graph: Dict,
             subject_id: str,
             object_id: str,
             edge_id: str,
             results: List
     ) -> bool:
         """
-        Validate that test case S--P->O edge is found bound to the Results?
+        Validate that test testcase S--P->O edge is found bound to the Results?
         :param query_graph: Dict, query graph to which the results pertain
         :param subject_id: str, subject node (CURIE) identifier
         :param object_id:  str, subject node (CURIE) identifier
         :param edge_id:  str, subject node (CURIE) identifier
         :param results: List of (TRAPI-version specific) Result objects
-        :return: bool, True if case S-P-O edge was found in the results
+        :return: bool, True if testcase S-P-O edge was found in the results
         """
-        assert query_graph, "case_result_found() encountered an empty query graph"
+        assert query_graph, "testcase_result_found() encountered an empty query graph"
         q_edges: Dict = query_graph["edges"]
-        q_edge_ids = tuple(q_edges.keys())
+        q_edge_ids = list(q_edges.keys())
 
         result_found: bool = False
         result: Dict
 
         for result in results:
 
             # Node binding validation still currently same for recent TRAPI versions
@@ -569,15 +620,15 @@
                 #         }
                 #     ]
 
                 # result["analyses"] may be empty but prior TRAPI 1.4.0 schema validation ensures that
                 # the "analysis" key is at least present plus the objects themselves are 'well-formed'
                 analyses: List = result["analyses"]
                 for analysis in analyses:
-                    edge_id_found: bool = self.case_edge_bindings(q_edge_ids, edge_id, analysis)
+                    edge_id_found: bool = self.testcase_edge_bindings(q_edge_ids, edge_id, analysis)
                     if edge_id_found:
                         break
 
             else:
                 # TRAPI 1.3.0 or earlier?
                 #
                 # Then, the TRAPI 1.3.0 Message Results (referencing the
@@ -595,43 +646,43 @@
                 #                 # the edge binding key should be the query edge id
                 #                 # bounded edge "id" is from knowledge graph
                 #                 "treated_by": [{"id": "df87ff82"}]
                 #             }
                 #         }
                 #     ]
                 #
-                edge_id_found: bool = self.case_edge_bindings(q_edge_ids, edge_id, result)
+                edge_id_found: bool = self.testcase_edge_bindings(q_edge_ids, edge_id, result)
 
             if subject_id_found and object_id_found and edge_id_found:
                 result_found = True
                 break
 
         return result_found
 
-    def case_input_found_in_response(
+    def testcase_input_found_in_response(
             self,
-            case: Dict,
+            testcase: Dict,
             response: Dict
     ) -> bool:
         """
         Predicate to validate if test data test case specified edge is returned
         in the Knowledge Graph of the TRAPI Response Message. This method assumes
         that the TRAPI response is already generally validated as well-formed.
 
-        :param case: Dict, input data test case
+        :param testcase: Dict, input data test case
         :param response: Dict, TRAPI Response whose message ought to contain the test case edge
         :return: True if test case edge found; False otherwise
         """
         # sanity checks
-        assert case, "case_input_found_in_response(): Empty or missing test case data!"
-        assert response, "case_input_found_in_response(): Empty or missing TRAPI Response!"
-        assert "message" in response, "case_input_found_in_response(): TRAPI Response missing its Message component!"
+        assert testcase, "testcase_input_found_in_response(): Empty or missing test testcase data!"
+        assert response, "testcase_input_found_in_response(): Empty or missing TRAPI Response!"
+        assert "message" in response, "testcase_input_found_in_response(): TRAPI Response missing its Message component!"
 
         #
-        # case: Dict parameter contains something like:
+        # testcase: Dict parameter contains something like:
         #
         #     idx: 0,
         #     subject_category: 'biolink:SmallMolecule',
         #     object_category: 'biolink:Disease',
         #     predicate: 'biolink:treats',
         #     subject_id: 'CHEBI:3002',  # may have the deprecated key 'subject' here
         #     object_id: 'MESH:D001249', # may have the deprecated key 'object' here
@@ -640,15 +691,15 @@
         # the TRAPI Knowledge Graph, with a Result mapping?
         #
         message: Dict = response["message"]
 
         # Another sanity check - unlikely to be a problem since
         # TRAPI schema validation should have picked it up since
         # the TRAPI Message is "nullable: false" in the schema
-        assert message, "case_input_found_in_response(): Empty or missing TRAPI message component!"
+        assert message, "testcase_input_found_in_response(): Empty or missing TRAPI message component!"
 
         message_found: bool = False
         if "query_graph" not in message:
             # missing query graph allowed by the TRAPI schema but
             # the input test data edge is automatically deemed missing
             self.report(
                 code="error.trapi.response.message.query_graph.missing"
@@ -719,30 +770,30 @@
         # In the Knowledge Graph:
         #
         #     "nodes": {
         #         "MONDO:0005148": {"name": "type-2 diabetes"},
         #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
         #     }
         #
-        # Check for case 'subject_id' and 'object_id',
+        # Check for testcase 'subject_id' and 'object_id',
         # with expected categories, in nodes catalog
         nodes: Dict = knowledge_graph["nodes"]
-        subject_id = case["subject_id"] if "subject_id" in case else case["subject"]
+        subject_id = testcase["subject_id"] if "subject_id" in testcase else testcase["subject"]
         subject_aliases = get_aliases(subject_id)
-        if not self.case_node_found("subject", subject_aliases, case, nodes):
+        if not self.testcase_node_found("subject", subject_aliases, testcase, nodes):
             self.report(
                 code="error.trapi.response.message.knowledge_graph.node.missing",
                 identifier=subject_id,
                 context="subject"
             )
             return False
 
-        object_id = case["object_id"] if "object_id" in case else case["object"]
+        object_id = testcase["object_id"] if "object_id" in testcase else testcase["object"]
         object_aliases = get_aliases(object_id)
-        if not self.case_node_found("object", object_aliases, case, nodes):
+        if not self.testcase_node_found("object", object_aliases, testcase, nodes):
             self.report(
                 code="error.trapi.response.message.knowledge_graph.node.missing",
                 identifier=object_id,
                 context="object"
             )
             return False
 
@@ -753,27 +804,27 @@
         #             "subject": "CHEBI:6801",
         #             "predicate": "biolink:treats",
         #             "object": "MONDO:0005148"
         #         }
         #     }
         #
         # Check in the edges catalog for an edge containing
-        # the case 'subject_id', 'predicate' and 'object_id'
+        # the testcase 'subject_id', 'predicate' and 'object_id'
         edges: Dict = knowledge_graph["edges"]
 
-        predicate = case["predicate"] if "predicate" in case else case["predicate_id"]
+        predicate = testcase["predicate"] if "predicate" in testcase else testcase["predicate_id"]
         predicate_descendants: List[str]
         inverse_predicate_descendants: List[str] = list()  # may sometimes remain empty...
         if self.validate_biolink():
             predicate_descendants = self.bmt.get_descendants(predicate, formatted=True)
             inverse_predicate = self.get_inverse_predicate(predicate)
             if inverse_predicate:
                 inverse_predicate_descendants = self.bmt.get_descendants(inverse_predicate, formatted=True)
         else:
-            # simpler case in which we are ignoring deep Biolink Model validation
+            # simpler testcase in which we are ignoring deep Biolink Model validation
             predicate_descendants = [predicate]
 
         edge_id_match: Optional[str] = None
         subject_match: Optional[str] = None
         object_match: Optional[str] = None
         for edge_id, edge in edges.items():
             # Note: this edge search could be arduous on a big knowledge graph?
@@ -790,30 +841,30 @@
                 # observation of the inverse edge is also counted as a match?
                 subject_match = edge["subject"]
                 object_match = edge["object"]
                 edge_id_match = edge_id
                 break
 
         edge_id: str = \
-            f"{case['idx']}|" +\
-            f"({case['subject_id']}#{case['subject_category']})" + \
+            f"{testcase['idx']}|" +\
+            f"({testcase['subject_id']}#{testcase['subject_category']})" + \
             f"-[{predicate}]->" + \
-            f"({case['object_id']}#{case['object_category']})"
+            f"({testcase['object_id']}#{testcase['object_category']})"
 
         if edge_id_match is None:
             self.report(
                 code="error.trapi.response.message.knowledge_graph.edge.missing",
                 identifier=edge_id
             )
             return False
 
         results: List = message["results"]
-        if not self.case_result_found(query_graph, subject_match, object_match, edge_id_match, results):
+        if not self.testcase_result_found(query_graph, subject_match, object_match, edge_id_match, results):
             self.report(
                 code="error.trapi.response.message.result.missing",
                 identifier=edge_id
             )
             return False
 
-        # By this point, the case data assumed to be
+        # By this point, the testcase data assumed to be
         # successfully validated in the TRAPI Response?
         return True
```

### Comparing `reasoner_validator-4.2.0/reasoner_validator/versioning.py` & `reasoner_validator-4.2.1/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/reasoner_validator/versions.yaml` & `reasoner_validator-4.2.1/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/__init__.py` & `reasoner_validator-4.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.2.1/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.2.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_ontology.py` & `reasoner_validator-4.2.1/tests/test_ontology.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 from typing import Optional
 import pytest
 
 from reasoner_validator.utils.http import post_query
 from reasoner_validator.biolink.ontology import (
     ONTOLOGY_KP_TRAPI_SERVER,
-    NODE_NORMALIZER_SERVER
+    NODE_NORMALIZER_SERVER,
+    get_parent_concept
 )
 
 pytest_plugins = ('pytest_asyncio',)
 
 
 @pytest.mark.parametrize(
     "curie,category,result",
@@ -73,7 +74,32 @@
     j = {'curies': [curie]}
     result = post_query(url=NODE_NORMALIZER_SERVER, query=j, server="Post Node Normalizer Query")
     assert result
     assert curie in result
     assert "equivalent_identifiers" in result[curie]
     assert len(result[curie]["equivalent_identifiers"])
     assert category in result[curie]["type"]
+
+
+@pytest.mark.parametrize(
+    "curie,category,result",
+    [
+        (   # Query 0 - chemical compounds are NOT in an ontology hierarchy
+            "CHEMBL.COMPOUND:CHEMBL2333026",
+            "biolink:SmallMolecule",
+            None
+        ),
+        (   # Query 1 - MONDO disease terms are in an ontology term hierarchy
+            "MONDO:0011027",
+            "biolink:Disease",
+            "MONDO:0015967"
+        ),
+        (   # Query 2 - HP phenotype terms are in an ontology term hierarchy
+            "HP:0040068",  # "Abnormality of limb bone"
+            "biolink:PhenotypicFeature",
+            "HP:0000924"  # Abnormality of the skeletal system
+        )
+    ]
+)
+def test_get_parent_concept(curie: str, category: str, result: Optional[str]):
+    # Just use default Biolink Model release for this test
+    assert get_parent_concept(curie=curie, category=category, biolink_version=None) == result
```

### Comparing `reasoner_validator-4.2.0/tests/test_response_validator.py` & `reasoner_validator-4.2.1/tests/test_response_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
-from typing import Dict, Optional
+from typing import List, Dict, Optional
 from sys import stderr
 
 import logging
 
 from copy import deepcopy
 
 import pytest
@@ -1202,24 +1202,63 @@
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
     validator.check_compliance_of_trapi_response(response=response)
     validator.dump(file=stderr)
     print("\n"+"="*80+"\n", file=stderr)
 
 
 @pytest.mark.parametrize(
+    "source_categories,target_categories,outcome",
+    [
+        (   # query 0 - empty lists don't have anything to match?
+            [], [], False
+        ),
+        (   # query 1 - exact matches should be true
+            ["biolink:Gene"], ["biolink:Gene"], True
+        ),
+        (   # query 2 - biolink:Protein is **not** directly matched in the
+            #           'source' hierarchy (even though its parents could overlap)
+            ["biolink:Gene"], ["biolink:Drug"], False
+        ),
+        (   # query 3 - but a 'target' category list with at least one exact
+            #           match of category to source will also be matched,
+            #           even if other target entries don't match
+            ["biolink:Gene"], ["biolink:Gene", "biolink:Drug"], True
+        ),
+        (   # query 4 - 'target' category matches at least one
+            #           parent of the list of 'source' categories
+            ["biolink:Gene"], ["biolink:BiologicalEntity"], True
+        ),
+        (   # query 5 - a 'target' category list matches at least
+            #           one match to a parent of the list of the
+            #           'source' categories, will be matched,
+            #           even if other target entries don't match
+            #
+            ["biolink:Gene"], ["biolink:BiologicalEntity", "biolink:Drug"], True
+        )
+    ]
+)
+def test_category_matched(source_categories: List[str], target_categories: List[str], outcome: bool):
+    validator = TRAPIResponseValidator()
+    assert validator.category_matched(
+        source_categories,
+        target_categories,
+    ) is outcome
+
+
+@pytest.mark.parametrize(
     "case,response",
     [
         (dict(), {"empty": "nonsense"}),
         ({"empty": "nonsense"}, dict()),
     ]
 )
 def test_empty_case_input_found_in_response(case, response):
     validator = TRAPIResponseValidator()
     with pytest.raises(AssertionError):
-        validator.case_input_found_in_response(case, response)
+        validator.testcase_input_found_in_response(case, response)
 
 
 #
 # case: Dict parameter contains something like:
 #
 SAMPLE_TEST_CASE = {
     "idx": 0,
@@ -1454,9 +1493,9 @@
             },
             "error.trapi.response.message.result.missing"
         )
     ]
 )
 def test_case_input_found_in_response(case, response, code):
     validator = TRAPIResponseValidator()
-    assert not validator.case_input_found_in_response(case, response) if code else True
+    assert not validator.testcase_input_found_in_response(case, response) if code else True
     check_messages(validator, code)
```

### Comparing `reasoner_validator-4.2.0/tests/test_semver.py` & `reasoner_validator-4.2.1/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_trapi_versioning.py` & `reasoner_validator-4.2.1/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_validate.py` & `reasoner_validator-4.2.1/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_validation_report.py` & `reasoner_validator-4.2.1/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/tests/test_workflows.py` & `reasoner_validator-4.2.1/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.2.0/PKG-INFO` & `reasoner_validator-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.2.0
+Version: 4.2.1
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

