# Comparing `tmp/sapiopycommons-32.0.0.24.5.tar.gz` & `tmp/sapiopycommons-32.0.1.24.5.tar.gz`

## Comparing `sapiopycommons-32.0.0.24.5.tar` & `sapiopycommons-32.0.1.24.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/callbacks/__init__.py
--rw-r--r--   0        0        0    43256 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/callbacks/callback_util.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/IndigoMolecules.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/datatype/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/datatype/attachment_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/__init__.py
--rw-r--r--   0        0        0    57198 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/experiment_handler.py
--rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/plate_designer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/complex_data_loader.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_bridge.py
--rw-r--r--   0        0        0    36746 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_data_handler.py
--rw-r--r--   0        0        0    25556 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_util.py
--rw-r--r--   0        0        0    24499 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_validator.py
--rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/__init__.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/aliases.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/custom_report_util.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/exceptions.py
--rw-r--r--   0        0        0    30126 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/popup_util.py
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/storage_util.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/time_util.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/multimodal/multimodal.py
--rw-r--r--   0        0        0    14787 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/multimodal/multimodal_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/processtracking/__init__.py
--rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/processtracking/endpoints.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/recordmodel/__init__.py
--rw-r--r--   0        0        0    39348 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/recordmodel/record_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/__init__.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/eln_rule_handler.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/on_save_rule_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/webhook/__init__.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/src/sapiopycommons/webhook/webhook_handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/_do_not_add_init_py_here
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/bio_reg_test.py
--rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/chem_test.py
--rw-r--r--   0        0        0  1669824 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/data_type_models.py
--rw-r--r--   0        0        0    10718 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/kappa.chains.fasta
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/mafft_test.py
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/tests/test.gb
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/LICENSE
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/README.md
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/pyproject.toml
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 sapiopycommons-32.0.0.24.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/callbacks/__init__.py
+-rw-r--r--   0        0        0    43256 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/callbacks/callback_util.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/chem/IndigoMolecules.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/chem/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/chem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/datatype/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/datatype/attachment_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/eln/__init__.py
+-rw-r--r--   0        0        0    57198 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/eln/experiment_handler.py
+-rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/eln/plate_designer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/complex_data_loader.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_bridge.py
+-rw-r--r--   0        0        0    36746 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_data_handler.py
+-rw-r--r--   0        0        0    25556 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_util.py
+-rw-r--r--   0        0        0    24499 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_validator.py
+-rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/__init__.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/aliases.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/custom_report_util.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/exceptions.py
+-rw-r--r--   0        0        0    30126 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/popup_util.py
+-rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/storage_util.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/time_util.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/multimodal/multimodal.py
+-rw-r--r--   0        0        0    14787 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/multimodal/multimodal_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/processtracking/__init__.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/processtracking/endpoints.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/recordmodel/__init__.py
+-rw-r--r--   0        0        0    39348 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/recordmodel/record_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/rules/__init__.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/rules/eln_rule_handler.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/rules/on_save_rule_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/webhook/__init__.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/src/sapiopycommons/webhook/webhook_handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/_do_not_add_init_py_here
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/bio_reg_test.py
+-rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/chem_test.py
+-rw-r--r--   0        0        0  1669824 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/data_type_models.py
+-rw-r--r--   0        0        0    10718 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/kappa.chains.fasta
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/mafft_test.py
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/tests/test.gb
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/LICENSE
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/README.md
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/pyproject.toml
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 sapiopycommons-32.0.1.24.5/PKG-INFO
```

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/callbacks/callback_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/callbacks/callback_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/IndigoMolecules.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/chem/IndigoMolecules.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/chem/Molecules.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/chem/Molecules.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/datatype/attachment_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/datatype/attachment_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/experiment_handler.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/eln/experiment_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/eln/plate_designer.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/eln/plate_designer.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/complex_data_loader.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/complex_data_loader.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_bridge.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_bridge.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_data_handler.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_data_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_validator.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_validator.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/files/file_writer.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/files/file_writer.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/aliases.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/aliases.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/custom_report_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/custom_report_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/exceptions.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/popup_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/popup_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/storage_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/storage_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/general/time_util.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/general/time_util.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/multimodal/multimodal.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/multimodal/multimodal.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/multimodal/multimodal_data.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/multimodal/multimodal_data.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/processtracking/endpoints.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/processtracking/endpoints.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/recordmodel/record_handler.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/recordmodel/record_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/eln_rule_handler.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/rules/eln_rule_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/rules/on_save_rule_handler.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/rules/on_save_rule_handler.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/src/sapiopycommons/webhook/webhook_handlers.py` & `sapiopycommons-32.0.1.24.5/src/sapiopycommons/webhook/webhook_handlers.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/tests/bio_reg_test.py` & `sapiopycommons-32.0.1.24.5/tests/bio_reg_test.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/tests/chem_test.py` & `sapiopycommons-32.0.1.24.5/tests/chem_test.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/tests/data_type_models.py` & `sapiopycommons-32.0.1.24.5/tests/data_type_models.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/tests/kappa.chains.fasta` & `sapiopycommons-32.0.1.24.5/tests/kappa.chains.fasta`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/tests/mafft_test.py` & `sapiopycommons-32.0.1.24.5/tests/mafft_test.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/tests/test.gb` & `sapiopycommons-32.0.1.24.5/tests/test.gb`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/LICENSE` & `sapiopycommons-32.0.1.24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/README.md` & `sapiopycommons-32.0.1.24.5/README.md`

 * *Files identical despite different names*

### Comparing `sapiopycommons-32.0.0.24.5/pyproject.toml` & `sapiopycommons-32.0.1.24.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopycommons"
-version='32.0.0.24.5'
+version='32.0.1.24.5'
 authors = [
     { name="Jonathan Steck", email="jsteck@sapiosciences.com" },
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Python API Utilities Package"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
-        'sapiopylib>=2024.4.23a188', 'databind>=4.5'
+        'sapiopylib>=2024.05.18.208', 'databind>=4.5'
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
```

### Comparing `sapiopycommons-32.0.0.24.5/PKG-INFO` & `sapiopycommons-32.0.1.24.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopycommons
-Version: 32.0.0.24.5
+Version: 32.0.1.24.5
 Summary: Official Sapio Python API Utilities Package
 Project-URL: Homepage, https://github.com/sapiosciences
 Author-email: Jonathan Steck <jsteck@sapiosciences.com>, Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Requires-Dist: databind>=4.5
-Requires-Dist: sapiopylib>=2024.4.23a188
+Requires-Dist: sapiopylib>=2024.05.18.208
 Description-Content-Type: text/markdown
 
 
 # sapiopycommons: Official Sapio Python API Utilities Package
 
 <div align="center"><a href="https://www.sapiosciences.com" target="_blank">
   <img src="https://s3.amazonaws.com/public.exemplareln.com/sapio-pylib/sapio-sciencesofficial-python-api-library.png" alt="Sapio Sciences"><br>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.3 Name: sapiopycommons Version: 32.0.0.24.5 Summary:
+Metadata-Version: 2.3 Name: sapiopycommons Version: 32.0.1.24.5 Summary:
 Official Sapio Python API Utilities Package Project-URL: Homepage, https://
 github.com/sapiosciences Author-email: Jonathan Steck
 sapiosciences.com>, Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Bio-
 Informatics Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.10 Requires-Dist: databind>=4.5 Requires-Dist:
-sapiopylib>=2024.4.23a188 Description-Content-Type: text/markdown #
+sapiopylib>=2024.05.18.208 Description-Content-Type: text/markdown #
 sapiopycommons: Official Sapio Python API Utilities Package
                                _[_S_a_p_i_o_ _S_c_i_e_n_c_e_s_]
 ----------------- [![PyPI Latest Release](https://img.shields.io/pypi/v/
 sapiopycommons.svg)](https://pypi.org/project/sapiopycommons/) [![License]
 (https://img.shields.io/pypi/l/sapiopycommons.svg)](https://github.com/
 sapiosciences/sapio-py-tutorials/blob/master/LICENSE) ## What is it?
 sapiopycommons is a utilities package, developed and maintained by Sapio
```

