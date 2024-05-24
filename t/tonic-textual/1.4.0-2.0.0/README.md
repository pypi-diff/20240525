# Comparing `tmp/tonic_textual-1.4.0.tar.gz` & `tmp/tonic_textual-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_textual-1.4.0.tar", max compression
+gzip compressed data, was "tonic_textual-2.0.0.tar", max compression
```

## Comparing `tonic_textual-1.4.0.tar` & `tonic_textual-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,40 @@
--rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-1.4.0/LICENSE
--rw-r--r--   0        0        0      972 2024-02-17 17:17:54.164871 tonic_textual-1.4.0/README.md
--rw-r--r--   0        0        0      598 2024-05-01 21:45:49.547180 tonic_textual-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       19 2024-05-01 21:45:49.547299 tonic_textual-1.4.0/tonic_textual/__init__.py
--rw-r--r--   0        0        0    17451 2024-05-01 21:45:49.547439 tonic_textual-1.4.0/tonic_textual/api.py
--rw-r--r--   0        0        0        0 2024-02-17 17:17:54.168806 tonic_textual-1.4.0/tonic_textual/classes/__init__.py
--rw-r--r--   0        0        0      789 2024-02-17 17:17:54.168921 tonic_textual-1.4.0/tonic_textual/classes/api_responses/redaction_response.py
--rw-r--r--   0        0        0      668 2024-02-23 23:38:13.865340 tonic_textual-1.4.0/tonic_textual/classes/api_responses/single_detection_result.py
--rw-r--r--   0        0        0      348 2024-02-17 17:17:54.169331 tonic_textual-1.4.0/tonic_textual/classes/custom_model.py
--rw-r--r--   0        0        0     8183 2024-05-01 21:45:49.547665 tonic_textual-1.4.0/tonic_textual/classes/dataset.py
--rw-r--r--   0        0        0     1633 2024-02-17 17:17:54.169557 tonic_textual-1.4.0/tonic_textual/classes/datasetfile.py
--rw-r--r--   0        0        0     4845 2024-05-01 21:45:49.547986 tonic_textual-1.4.0/tonic_textual/classes/httpclient.py
--rw-r--r--   0        0        0     1864 2024-05-01 21:45:49.548117 tonic_textual-1.4.0/tonic_textual/classes/tonic_exception.py
--rw-r--r--   0        0        0      121 2024-05-01 21:45:49.548424 tonic_textual-1.4.0/tonic_textual/enums/pii_state.py
--rw-r--r--   0        0        0        0 2024-02-17 17:17:54.170004 tonic_textual-1.4.0/tonic_textual/services/__init__.py
--rw-r--r--   0        0        0      610 2024-02-17 17:17:54.170141 tonic_textual-1.4.0/tonic_textual/services/dataset.py
--rw-r--r--   0        0        0      552 2024-02-17 17:17:54.170230 tonic_textual-1.4.0/tonic_textual/services/datasetfile.py
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 tonic_textual-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-2.0.0/LICENSE
+-rw-r--r--   0        0        0      979 2024-05-24 21:03:00.487683 tonic_textual-2.0.0/README.md
+-rw-r--r--   0        0        0      598 2024-05-24 21:03:00.489256 tonic_textual-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-24 21:03:00.490079 tonic_textual-2.0.0/tonic_textual/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:40:23.410925 tonic_textual-2.0.0/tonic_textual/classes/__init__.py
+-rw-r--r--   0        0        0      268 2024-05-24 21:03:00.490219 tonic_textual-2.0.0/tonic_textual/classes/api_responses/PaginationResponseModel
+-rw-r--r--   0        0        0     1817 2024-05-24 21:03:00.490506 tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/base_file.py
+-rw-r--r--   0        0        0     1224 2024-05-24 21:03:00.490739 tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/single_detection_result.py
+-rw-r--r--   0        0        0      405 2024-05-24 21:03:00.491133 tonic_textual-2.0.0/tonic_textual/classes/custom_model.py
+-rw-r--r--   0        0        0     9366 2024-05-24 21:03:00.491484 tonic_textual-2.0.0/tonic_textual/classes/dataset.py
+-rw-r--r--   0        0        0     1836 2024-05-24 21:03:00.491817 tonic_textual-2.0.0/tonic_textual/classes/datasetfile.py
+-rw-r--r--   0        0        0      130 2024-05-24 21:03:00.492019 tonic_textual-2.0.0/tonic_textual/classes/enums/docx_header_footer_type.py
+-rw-r--r--   0        0        0      211 2024-05-24 21:03:00.492357 tonic_textual-2.0.0/tonic_textual/classes/enums/file_type.py
+-rw-r--r--   0        0        0      263 2024-05-24 21:03:00.492503 tonic_textual-2.0.0/tonic_textual/classes/enums/pdf_content_type.py
+-rw-r--r--   0        0        0      225 2024-05-24 21:03:00.492644 tonic_textual-2.0.0/tonic_textual/classes/enums/pdf_table_cell_type.py
+-rw-r--r--   0        0        0      800 2024-05-24 21:03:00.492802 tonic_textual-2.0.0/tonic_textual/classes/file_content/base_document.py
+-rw-r--r--   0        0        0     2014 2024-05-24 21:03:00.493027 tonic_textual-2.0.0/tonic_textual/classes/file_content/content.py
+-rw-r--r--   0        0        0      587 2024-05-24 21:03:00.493272 tonic_textual-2.0.0/tonic_textual/classes/file_content/csv_document.py
+-rw-r--r--   0        0        0     1037 2024-05-24 21:03:00.493457 tonic_textual-2.0.0/tonic_textual/classes/file_content/docx_document.py
+-rw-r--r--   0        0        0     1489 2024-05-24 21:03:00.493714 tonic_textual-2.0.0/tonic_textual/classes/file_content/pdf_document.py
+-rw-r--r--   0        0        0      385 2024-05-24 21:03:00.493923 tonic_textual-2.0.0/tonic_textual/classes/file_content/raw_document.py
+-rw-r--r--   0        0        0      790 2024-05-24 21:03:00.494112 tonic_textual-2.0.0/tonic_textual/classes/file_content/xlsx_document.py
+-rw-r--r--   0        0        0     2148 2024-05-24 23:05:01.047399 tonic_textual-2.0.0/tonic_textual/classes/file_parse_result_diff_enumerator.py
+-rw-r--r--   0        0        0     5112 2024-05-24 22:11:30.124934 tonic_textual-2.0.0/tonic_textual/classes/httpclient.py
+-rw-r--r--   0        0        0    10406 2024-05-24 23:05:01.047617 tonic_textual-2.0.0/tonic_textual/classes/parse_api_responses/file_parse_result.py
+-rw-r--r--   0        0        0      514 2024-05-24 21:03:00.495403 tonic_textual-2.0.0/tonic_textual/classes/parse_api_responses/file_parse_results_diff.py
+-rw-r--r--   0        0        0     2148 2024-05-24 21:03:00.495592 tonic_textual-2.0.0/tonic_textual/classes/pipeline.py
+-rw-r--r--   0        0        0     1970 2024-05-24 21:03:00.495892 tonic_textual-2.0.0/tonic_textual/classes/pipeline_file_enumerator.py
+-rw-r--r--   0        0        0      873 2024-05-24 21:03:00.496090 tonic_textual-2.0.0/tonic_textual/classes/pipeline_run.py
+-rw-r--r--   0        0        0      947 2024-05-24 21:03:00.496385 tonic_textual-2.0.0/tonic_textual/classes/redact_api_responses/redaction_response.py
+-rw-r--r--   0        0        0     2373 2024-05-24 23:05:01.047866 tonic_textual-2.0.0/tonic_textual/classes/tonic_exception.py
+-rw-r--r--   0        0        0      123 2024-05-24 21:03:00.496930 tonic_textual-2.0.0/tonic_textual/enums/pii_state.py
+-rw-r--r--   0        0        0      711 2024-05-24 21:03:00.497143 tonic_textual-2.0.0/tonic_textual/generator_utils.py
+-rw-r--r--   0        0        0     2907 2024-05-24 21:03:00.497319 tonic_textual-2.0.0/tonic_textual/markdown_utils.py
+-rw-r--r--   0        0        0     2234 2024-05-24 21:03:00.497439 tonic_textual-2.0.0/tonic_textual/parse_api.py
+-rw-r--r--   0        0        0    19135 2024-05-24 21:03:00.497758 tonic_textual-2.0.0/tonic_textual/redact_api.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:40:23.412740 tonic_textual-2.0.0/tonic_textual/services/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-24 21:03:00.498153 tonic_textual-2.0.0/tonic_textual/services/dataset.py
+-rw-r--r--   0        0        0      771 2024-05-24 21:03:00.498415 tonic_textual-2.0.0/tonic_textual/services/datasetfile.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 tonic_textual-2.0.0/PKG-INFO
```

### Comparing `tonic_textual-1.4.0/LICENSE` & `tonic_textual-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.4.0/README.md` & `tonic_textual-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This library contains useful wrappers around the Tonic Textual API
 
 ## Usage
 
 Instantiate the API wrapper using the following code:
 
 ```
-from tonic_textual.api import TonicTextual
+from tonic_textual.redact_api import TonicTextual
 
 # Do not include trailing backslash in TONIC_URL
 api = TonicTextual(TONIC_TEXTUAL_URL, API_KEY)
 ```
 
 Once instantiated, the following endpoints are available for consumption. Note that available endpoints and response types are limited. Available fields may be severely limited compared to the current Tonic API.
```

### Comparing `tonic_textual-1.4.0/pyproject.toml` & `tonic_textual-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-textual"
-version = "1.4.0"
+version = "2.0.0"
 description = "Wrappers around the Tonic Textual API"
 authors = ["Adam Kamor <adam@tonic.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.tonic.ai/"
 keywords = ["tonic.ai", "tonic", "tonic textual"]
```

### Comparing `tonic_textual-1.4.0/tonic_textual/api.py` & `tonic_textual-2.0.0/tonic_textual/redact_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,61 +3,93 @@
 import os
 import requests
 
 from time import sleep
 from typing import List, Optional, Union, Dict
 from urllib.parse import urlencode
 
-from tonic_textual.classes.api_responses.single_detection_result import SingleDetectionResult
+from tonic_textual.classes.common_api_responses.single_detection_result import (
+    SingleDetectionResult,
+)
 from tonic_textual.classes.custom_model import CustomModel
 from tonic_textual.classes.httpclient import HttpClient
-from tonic_textual.classes.api_responses.redaction_response import RedactionResponse
+from tonic_textual.classes.redact_api_responses.redaction_response import (
+    RedactionResponse,
+)
 from tonic_textual.enums.pii_state import PiiState
 from tonic_textual.services.dataset import DatasetService
 from tonic_textual.services.datasetfile import DatasetFileService
 from tonic_textual.classes.dataset import Dataset
 from tonic_textual.classes.datasetfile import DatasetFile
-from tonic_textual.classes.tonic_exception import DatasetNameAlreadyExists, InvalidJsonForRedactionRequest, FileNotReadyForDownload
+from tonic_textual.classes.tonic_exception import (
+    DatasetNameAlreadyExists,
+    InvalidJsonForRedactionRequest,
+    FileNotReadyForDownload,
+)
+
 
 class TonicTextual:
-    '''Wrapper class for invoking Tonic Textual API
+    """Wrapper class for invoking Tonic Textual API
 
     Parameters
     ----------
     base_url : str
         The URL to your Tonic Textual instance. Do not include trailing backslashes.
     api_key : str
-        Your API token. This argument is optional. Instead of providing the API token here, it is recommended that you set the API key in your environment as the value of TONIC_TEXTUAL_API_KEY.
+        Your API token. This argument is optional. Instead of providing the API token
+        here, it is recommended that you set the API key in your environment as the
+        value of TONIC_TEXTUAL_API_KEY.
     verify: bool
-        Whether SSL Certification verification is performed.  This is enabled by default.
+        Whether SSL Certification verification is performed.  This is enabled by
+        default.
     Examples
     --------
     >>> TonicTextual("http://localhost:3000")
-    '''
-    def __init__(self, base_url : str, api_key: Optional[str] = None, verify: bool = True):
+    """
+
+    def __init__(
+        self, base_url: str, api_key: Optional[str] = None, verify: bool = True
+    ):
         if api_key is None:
             api_key = os.environ.get("TONIC_TEXTUAL_API_KEY")
             if api_key is None:
-                raise Exception("No API key provided. Either provide an API key, or set the API key as the value of the TONIC_TEXTUAL_API_KEY environment variable.")
+                raise Exception(
+                    "No API key provided. Either provide an API key, or set the API "
+                    "key as the value of the TONIC_TEXTUAL_API_KEY environment "
+                    "variable."
+                )
         self.api_key = api_key
         self.client = HttpClient(base_url, self.api_key, verify)
         self.dataset_service = DatasetService(self.client)
         self.datasetfile_service = DatasetFileService(self.client)
         self.verify = verify
 
     @staticmethod
-    def _validate_generator_options(generator_default: PiiState, generator_config: Dict[str, PiiState]) -> None:
-        invalid_pii_states = [v for v in list(generator_config.values()) if v not in PiiState._member_names_]
-        if(len(invalid_pii_states)>0):
-            raise Exception("Invalid configuration for generator_config. The allowed values are Off, Synthesis, and Redaction.")
+    def _validate_generator_options(
+        generator_default: PiiState, generator_config: Dict[str, PiiState]
+    ) -> None:
+        invalid_pii_states = [
+            v
+            for v in list(generator_config.values())
+            if v not in PiiState._member_names_
+        ]
+        if len(invalid_pii_states) > 0:
+            raise Exception(
+                "Invalid configuration for generator_config. The allowed values are "
+                "Off, Synthesis, and Redaction."
+            )
         if generator_default not in PiiState._member_names_:
-            raise Exception("Invalid option for generator_default. The allowed values are Off, Synthesis, and Redaction.")
-
-    def create_dataset(self, dataset_name:str):
-        """Creates a dataset. A dataset is a collection of 1 or more files for Tonic Textual to scan and redact.
+            raise Exception(
+                "Invalid option for generator_default. The allowed values are Off, "
+                "Synthesis, and Redaction."
+            )
+
+    def create_dataset(self, dataset_name: str):
+        """Creates a dataset. A dataset is a collection of 1 or more files for Tonic
+        Textual to scan and redact.
 
         Parameters
         -----
         dataset_name : str
             The name of the dataset. Dataset names must be unique.
 
 
@@ -73,249 +105,356 @@
         DatasetNameAlreadyExists
             Raised if a dataset with the same name already exists.
 
         """
         try:
             self.client.http_post("/api/dataset", data={"name": dataset_name})
         except requests.exceptions.HTTPError as e:
-            if e.response.status_code==409:
+            if e.response.status_code == 409:
                 raise DatasetNameAlreadyExists(e)
 
         return self.get_dataset(dataset_name)
 
     def delete_dataset(self, dataset_name: str):
-        params = { "datasetName": dataset_name}
-        self.client.http_delete("/api/dataset/delete_dataset_by_name?" + urlencode(params))
-
-
+        params = {"datasetName": dataset_name}
+        self.client.http_delete(
+            "/api/dataset/delete_dataset_by_name?" + urlencode(params)
+        )
 
-
-    def get_dataset(self, dataset_name : str) -> Dataset:
-        '''Gets the dataset for the specified dataset name.
+    def get_dataset(self, dataset_name: str) -> Dataset:
+        """Gets the dataset for the specified dataset name.
 
         Parameters
         ----------
         dataset_name : str
             The name of the dataset.
 
         Returns
         -------
         Dataset
 
         Examples
         --------
         >>> dataset = tonic.get_dataset("llama_2_chatbot_finetune_v5")
-        '''
+        """
         return self.dataset_service.get_dataset(dataset_name)
 
     def get_files(self, dataset_id: str) -> List[DatasetFile]:
         """
         Gets all of the files in the dataset.
 
         Returns
         ------
         List[DatasetFile]
         A list of all of the files in the dataset.
         """
         return self.datasetfile_service.get_files(dataset_id)
 
-    def unredact_bulk(self, redacted_strings: List[str], random_seed: Optional[int] = None) -> List[str]:
-            """Removes redaction from a list of strings. Returns the strings with the original values.
-
-            Parameters
-            ----------
-            redacted_strings : List[str]
-                The list of redacted strings from which to remove the redaction.
-
-            random_seed: Optional[int] = None
-                An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
-
-            Returns
-            -------
-            List[str]
-                The list of strings with the redaction removed.
-            """
-
-            if random_seed is not None:
-                additional_headers = {'textual-random-seed':str(random_seed)}
-            else:
-                additional_headers = {}
-                
-            response = self.client.http_post("/api/unredact", data=redacted_strings, additional_headers=additional_headers)
-            return response
-
-    def unredact(self, redacted_string: str, random_seed: Optional[int] = None) -> str:
-            """Removes the redaction from a provided string. Returns the string with the original values.
-
-            Parameters
-            ----------
-            redacted_string : str
-                The redacted string from which to remove the redaction.
-
-            random_seed: Optional[int] = None
-                An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
-            
-            Returns
-            -------
-            str
-                The string with the redaction removed.
-            """
-
-
-            if random_seed is not None:
-                additional_headers = {'textual-random-seed':str(random_seed)}
-            else:
-                additional_headers = {}
-                
-            response = self.client.http_post("/api/unredact", data=[redacted_string], additional_headers=additional_headers)
-
-            
-            return response
-
-    def redact(self, string: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
-            """Redacts a string. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
+    def unredact_bulk(
+        self, redacted_strings: List[str], random_seed: Optional[int] = None
+    ) -> List[str]:
+        """Removes redaction from a list of strings. Returns the strings with the
+        original values.
 
-            Parameters
-            ----------
-            string : str
-                The string to redact.
-
-            generator_config: Dict[str, PiiState]
-                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
-                Values must be one of "Redaction", "Synthesis", or "Off".
+        Parameters
+        ----------
+        redacted_strings : List[str]
+            The list of redacted strings from which to remove the redaction.
 
-            generator_default: PiiState = PiiState.Redaction
-                The default redaction used for all types not specified in generator_config.
-                Values must be one of "Redaction", "Synthesis", or "Off".
+        random_seed: Optional[int] = None
+            An optional value to use to override Textual's default random number
+            seeding.  Can be used to ensure that different API calls use the same or
+            different random seeds.
 
-            custom_models: List[str] = []
-                A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
+        Returns
+        -------
+        List[str]
+            The list of strings with the redaction removed.
+        """
 
-            random_seed: Optional[int] = None
-                An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+        if random_seed is not None:
+            additional_headers = {"textual-random-seed": str(random_seed)}
+        else:
+            additional_headers = {}
 
-            Returns
-            -------
-            RedactionResponse
-                The redacted string along with ancillary information.
+        response = self.client.http_post(
+            "/api/unredact",
+            data=redacted_strings,
+            additional_headers=additional_headers,
+        )
+        return response
 
-            Examples
-            --------
-                >>> textual.redact("John Smith is a person", generator_config= {"NAME_GIVEN": "Redaction"}, generator_default="Off") # only redacts NAME_GIVEN
+    def unredact(self, redacted_string: str, random_seed: Optional[int] = None) -> str:
+        """Removes the redaction from a provided string. Returns the string with the
+        original values.
 
-            """
+        Parameters
+        ----------
+        redacted_string : str
+            The redacted string from which to remove the redaction.
 
-            self._validate_generator_options(generator_default, generator_config)
-            endpoint = "/api/redact"
+        random_seed: Optional[int] = None
+            An optional value to use to override Textual's default random number
+            seeding.  Can be used to ensure that different API calls use the same or
+            different random seeds.
 
-            if random_seed is not None:
-                additional_headers = {'textual-random-seed':str(random_seed)}
-            else:
-                additional_headers = {}
-                
-            response = self.client.http_post(endpoint, data={"text": string, "generatorDefault": generator_default, "generatorConfig": generator_config, "customModels": custom_models}, additional_headers=additional_headers)
-            de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"]) for x in list(response["deIdentifyResults"])]
+        Returns
+        -------
+        str
+            The string with the redaction removed.
+        """
 
-            return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
+        if random_seed is not None:
+            additional_headers = {"textual-random-seed": str(random_seed)}
+        else:
+            additional_headers = {}
 
-    def llm_synthesis(self, string: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction) -> RedactionResponse:
-        """Deidentifies a string by redacting sensitive data and replacing these values with values generated by an LLM.
+        response = self.client.http_post(
+            "/api/unredact",
+            data=[redacted_string],
+            additional_headers=additional_headers,
+        )
+
+        return response
+
+    def redact(
+        self,
+        string: str,
+        generator_config: Dict[str, PiiState] = dict(),
+        generator_default: PiiState = PiiState.Redaction,
+        custom_models: List[str] = [],
+        random_seed: Optional[int] = None,
+    ) -> RedactionResponse:
+        """Redacts a string. Depending on the configured handling for each sensitive
+        data type, values can be either redacted, synthesized, or ignored.
 
         Parameters
         ----------
         string : str
-                The string to redact.
+            The string to redact.
 
         generator_config: Dict[str, PiiState]
-                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+            A dictionary of sensitive data entities. For each entity, indicates whether
+            to redact, synthesize, or ignore it.
+            Values must be one of "Redaction", "Synthesis", or "Off".
 
         generator_default: PiiState = PiiState.Redaction
             The default redaction used for all types not specified in generator_config.
+            Values must be one of "Redaction", "Synthesis", or "Off".
 
-       Returns
+        custom_models: List[str] = []
+            A list of custom model names to use to identify values to redact. To see the
+            list of custom models that you have access to, use the get_custom_models
+            function.
+
+        random_seed: Optional[int] = None
+            An optional value to use to override Textual's default random number
+            seeding. Can be used to ensure that different API calls use the same or
+            different random seeds.
+
+        Returns
         -------
-                The de-identified string
+        RedactionResponse
+            The redacted string along with ancillary information.
+
+        Examples
+        --------
+            >>> textual.redact(
+            >>>     "John Smith is a person",
+            >>>     generator_config={"NAME_GIVEN": "Redaction"},
+            >>>     generator_default="Off"
+            >>> ) # only redacts NAME_GIVEN
+
         """
+
         self._validate_generator_options(generator_default, generator_config)
-        endpoint = "/api/synthesis"
-        response = self.client.http_post(endpoint, data={"text": string, "generatorDefault": generator_default, "generatorConfig": generator_config})
+        endpoint = "/api/redact"
 
-        de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"]) for x in
-                         list(response["deIdentifyResults"])]
+        if random_seed is not None:
+            additional_headers = {"textual-random-seed": str(random_seed)}
+        else:
+            additional_headers = {}
+
+        response = self.client.http_post(
+            endpoint,
+            data={
+                "text": string,
+                "generatorDefault": generator_default,
+                "generatorConfig": generator_config,
+                "customModels": custom_models,
+            },
+            additional_headers=additional_headers,
+        )
+        de_id_results = [
+            SingleDetectionResult(
+                x["start"], x["end"], x["label"], x["text"], x["score"]
+            )
+            for x in list(response["deIdentifyResults"])
+        ]
+
+        return RedactionResponse(
+            response["originalText"],
+            response["redactedText"],
+            response["usage"],
+            de_id_results,
+        )
+
+    def llm_synthesis(
+        self,
+        string: str,
+        generator_config: Dict[str, PiiState] = dict(),
+        generator_default: PiiState = PiiState.Redaction,
+    ) -> RedactionResponse:
+        """Deidentifies a string by redacting sensitive data and replacing these values
+        with values generated by an LLM.
+
+         Parameters
+         ----------
+         string : str
+                 The string to redact.
+
+         generator_config: Dict[str, PiiState]
+                 A dictionary of sensitive data entities. For each entity, indicates
+                 whether to redact, synthesize, or ignore it.
 
-        return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
+         generator_default: PiiState = PiiState.Redaction
+             The default redaction used for all types not specified in generator_config.
 
-    def redact_json(self, json_data: Union[str, dict], generator_config:Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
-        """Redacts the values in a JSON blob. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
+        Returns
+         -------
+                 The de-identified string
+        """
+        self._validate_generator_options(generator_default, generator_config)
+        endpoint = "/api/synthesis"
+        response = self.client.http_post(
+            endpoint,
+            data={
+                "text": string,
+                "generatorDefault": generator_default,
+                "generatorConfig": generator_config,
+            },
+        )
+
+        de_id_results = [
+            SingleDetectionResult(
+                x["start"], x["end"], x["label"], x["text"], x["score"]
+            )
+            for x in list(response["deIdentifyResults"])
+        ]
+
+        return RedactionResponse(
+            response["originalText"],
+            response["redactedText"],
+            response["usage"],
+            de_id_results,
+        )
+
+    def redact_json(
+        self,
+        json_data: Union[str, dict],
+        generator_config: Dict[str, PiiState] = dict(),
+        generator_default: PiiState = PiiState.Redaction,
+        custom_models: List[str] = [],
+        random_seed: Optional[int] = None,
+    ) -> RedactionResponse:
+        """Redacts the values in a JSON blob. Depending on the configured handling for
+        each sensitive data type, values can be either redacted, synthesized, or
+        ignored.
 
         Parameters
         ----------
         json_string : Union[str, dict]
-            The JSON whose values will be redacted.  This can be either a JSON string or a Python dictionary
+            The JSON whose values will be redacted.  This can be either a JSON string
+            or a Python dictionary
 
         generator_config: Dict[str, PiiState]
-                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+            A dictionary of sensitive data entities. For each entity, indicates whether
+            to redact, synthesize, or ignore it.
 
         generator_default: PiiState = PiiState.Redaction
-                The default redaction used for all types not specified in generator_config.
+            The default redaction used for all types not specified in generator_config.
 
         custom_models: List[str] = []
-            A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
+            A list of custom model names to use to identify values to redact. To see
+            the list of custom models that you have access to, use the get_custom_models
+            function.
 
         random_seed: Optional[int] = None
-            An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+            An optional value to use to override Textual's default random number
+            seeding. Can be used to ensure that different API calls use the same or
+            different random seeds.
 
         Returns
         -------
         RedactionResponse
             The redacted string along with ancillary information.
         """
         self._validate_generator_options(generator_default, generator_config)
         endpoint = "/api/redact/json"
 
         if isinstance(json_data, str):
             json_text = json_data
         elif isinstance(json_data, dict):
             json_text = json.dumps(json_data)
         else:
-            raise Exception(f'redact_json must receive either a JSON blob as a string or dict().  You passed in type {type(json_data)} which is not supported')
-        payload = {"jsonText": json_text, "generatorDefault":generator_default, "generatorConfig": generator_config, "customModels": custom_models}
+            raise Exception(
+                "redact_json must receive either a JSON blob as a string or dict(). "
+                f"You passed in type {type(json_data)} which is not supported"
+            )
+        payload = {
+            "jsonText": json_text,
+            "generatorDefault": generator_default,
+            "generatorConfig": generator_config,
+            "customModels": custom_models,
+        }
 
         try:
             if random_seed is not None:
-                additional_headers = {'textual-random-seed':str(random_seed)}
+                additional_headers = {"textual-random-seed": str(random_seed)}
             else:
                 additional_headers = {}
-            response = self.client.http_post(endpoint, data=payload, additional_headers=additional_headers)
+            response = self.client.http_post(
+                endpoint, data=payload, additional_headers=additional_headers
+            )
         except requests.exceptions.HTTPError as e:
-             if e.response.status_code==400:
-                  raise InvalidJsonForRedactionRequest(e.response.text)
-             raise e
-
-        de_id_results = [SingleDetectionResult(x["start"], x["end"], x["label"], x["text"], x["score"], x["jsonPath"]) for x in list(response["deIdentifyResults"])]
-
-        return RedactionResponse(response["originalText"], response["redactedText"], response["usage"], de_id_results)
+            if e.response.status_code == 400:
+                raise InvalidJsonForRedactionRequest(e.response.text)
+            raise e
+
+        de_id_results = [
+            SingleDetectionResult(
+                x["start"], x["end"], x["label"], x["text"], x["score"], x["jsonPath"]
+            )
+            for x in list(response["deIdentifyResults"])
+        ]
+
+        return RedactionResponse(
+            response["originalText"],
+            response["redactedText"],
+            response["usage"],
+            de_id_results,
+        )
 
     def get_custom_models(self) -> List[CustomModel]:
         """Returns all of the custom models that the user owns.
 
         Returns
         -------
         List[CustomModel]
             A list of all of the custom models that the user owns.
         """
 
         with requests.Session() as session:
             response = self.client.http_get("/api/models", session=session)
             models: List[CustomModel] = []
             for model in response:
-                id = model['id']
-                name = model['name']
-                entities = model['entities']
-                entityNames = [entity['label'] for entity in entities]
+                id = model["id"]
+                name = model["name"]
+                entities = model["entities"]
+                entityNames = [entity["label"] for entity in entities]
                 models.append(CustomModel(id, name, entityNames))
 
             return models
 
     def start_file_redaction(self, file: io.IOBase, file_name: str) -> str:
         """
         Redact a provided file
@@ -331,62 +470,91 @@
         -------
         str
         The job id which can be used to download the redacted file once it is ready
 
         """
 
         files = {
-            'document': (None, json.dumps({"fileName": file_name, "csvConfig":{}, "datasetId":""}), 'application/json'),
-            'file': file
+            "document": (
+                None,
+                json.dumps({"fileName": file_name, "csvConfig": {}, "datasetId": ""}),
+                "application/json",
+            ),
+            "file": file,
         }
 
         response = self.client.http_post("/api/unattachedfile/upload", files=files)
 
-        return response['jobId']
+        return response["jobId"]
 
-    def download_redacted_file(self, job_id: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None, num_retries: int = 6) -> bytes:
+    def download_redacted_file(
+        self,
+        job_id: str,
+        generator_config: Dict[str, PiiState] = dict(),
+        generator_default: PiiState = PiiState.Redaction,
+        custom_models: List[str] = [],
+        random_seed: Optional[int] = None,
+        num_retries: int = 6,
+    ) -> bytes:
         """
         Download a redacted file
 
         Parameters
         --------
         job_id: str
             The ID of the redaction job
 
         generator_config: Dict[str, PiiState]
-                A dictionary of sensitive data entities. For each entity, indicates whether to redact, synthesize, or ignore it.
+            A dictionary of sensitive data entities. For each entity, indicates whether
+            to redact, synthesize, or ignore it.
 
         generator_default: PiiState = PiiState.Redaction
-                The default redaction used for all types not specified in generator_config.
+            The default redaction used for all types not specified in generator_config.
 
         custom_models: List[str] = []
-            A list of custom model names to use to identify values to redact. To see the list of custom models that you have access to, use the get_custom_models function.
+            A list of custom model names to use to identify values to redact. To see
+            the list of custom models that you have access to, use the get_custom_models
+            function.
 
         random_seed: Optional[int] = None
-            An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+            An optional value to use to override Textual's default random number
+            seeding. Can be used to ensure that different API calls use the same or
+            different random seeds.
 
         num_retries: int = 6
-            An optional value to specify how many times to attempt to download the file.  If a file is not yet ready for download, there will be a 10 second pause before retrying.  (The default value is 6)
+            An optional value to specify how many times to attempt to download the
+            file.  If a file is not yet ready for download, there will be a 10 second
+            pause before retrying. (The default value is 6)
 
         Returns
         -------
         bytes
             The redacted file as byte array
         """
         self._validate_generator_options(generator_default, generator_config)
         retries = 1
-        while(retries <= num_retries):
+        while retries <= num_retries:
             try:
                 if random_seed is not None:
-                    additional_headers = {'textual-random-seed':str(random_seed)}
+                    additional_headers = {"textual-random-seed": str(random_seed)}
                 else:
                     additional_headers = {}
-                return self.client.http_post_download_file(f"/api/unattachedfile/{job_id}/download", data={"generatorDefault": generator_default, "generatorConfig": generator_config, "customModels": custom_models}, additional_headers=additional_headers )
-                
-            
+                return self.client.http_post_download_file(
+                    f"/api/unattachedfile/{job_id}/download",
+                    data={
+                        "generatorDefault": generator_default,
+                        "generatorConfig": generator_config,
+                        "customModels": custom_models,
+                    },
+                    additional_headers=additional_headers,
+                )
+
             except FileNotReadyForDownload:
-                 retries = retries + 1
-                 if retries <= num_retries:
+                retries = retries + 1
+                if retries <= num_retries:
                     sleep(10)
 
-        retryWord = "retry" if num_retries==1 else "retries"
-        raise FileNotReadyForDownload(f"After {num_retries} {retryWord} the file is not yet ready for download.  This is likely due to a high service load.  Please try again later.")
+        retryWord = "retry" if num_retries == 1 else "retries"
+        raise FileNotReadyForDownload(
+            f"After {num_retries} {retryWord} the file is not yet ready for download. "
+            "This is likely due to a high service load. Please try again later."
+        )
```

### Comparing `tonic_textual-1.4.0/tonic_textual/classes/api_responses/single_detection_result.py` & `tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/single_detection_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,49 @@
 import json
-from typing import Optional
+from typing import Optional, Dict
+
 
 class SingleDetectionResult(dict):
-    def __init__(self, start: int, end: int, label: str, text: str, score: float, json_path: Optional[str]=None):
+    def __init__(
+        self,
+        start: int,
+        end: int,
+        label: str,
+        text: str,
+        score: float,
+        json_path: Optional[str] = None,
+    ):
         self.start = start
         self.end = end
         self.label = label
         self.text = text
         self.score = score
         self.jsonPath = json_path
         if json_path is None:
-            dict.__init__(self, start=start, end=end, label=label, text=text, score=score)
+            dict.__init__(
+                self, start=start, end=end, label=label, text=text, score=score
+            )
         else:
-            dict.__init__(self, start=start, end=end, label=label, text=text, score=score, json_path=json_path)
-            
+            dict.__init__(
+                self,
+                start=start,
+                end=end,
+                label=label,
+                text=text,
+                score=score,
+                json_path=json_path,
+            )
+
     def describe(self):
-        print(json.dumps(self))
+        return json.dumps(self.to_dict(), indent=2)
+
+    def to_dict(self) -> Dict:
+        out = {
+            "start": self.start,
+            "end": self.end,
+            "label": self.label,
+            "text": self.text,
+            "score": self.score,
+        }
+        if self.jsonPath is not None:
+            out["jsonPath"] = self.jsonPath
+        return out
```

### Comparing `tonic_textual-1.4.0/tonic_textual/classes/dataset.py` & `tonic_textual-2.0.0/tonic_textual/classes/dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import List, Dict, Optional
+from typing import List, Dict, Optional, Any
 import os
 import json
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 import requests.exceptions
 import requests
 import pandas as pd
@@ -27,20 +27,33 @@
 
     files: Dict
         Serialized DatasetFile objects representing the files in a dataset.
 
     client: HttpClient
         The HTTP client to use.
     """
-    def __init__(self, id: str, name: str, files: List[Dict], client: HttpClient):
+
+    def __init__(
+        self, id: str, name: str, files: List[Dict[str, Any]], client: HttpClient
+    ):
         self.id = id
         self.name = name
         self.client = client
         self.datasetfile_service = DatasetFileService(self.client)
-        self.files = [DatasetFile(f['fileId'],f['fileName'],f.get('numRows'),f['numColumns'], f['processingStatus'], f.get('processingError')) for f in files]
+        self.files = [
+            DatasetFile(
+                f["fileId"],
+                f["fileName"],
+                f.get("numRows"),
+                f["numColumns"],
+                f["processingStatus"],
+                f.get("processingError"),
+            )
+            for f in files
+        ]
 
         if len(self.files) > 0:
             self.num_columns = max([f.num_columns for f in self.files])
         else:
             self.num_columns = None
 
         self.num_rows_per_request = 1000
@@ -71,31 +84,59 @@
         DatasetFileMatchesExistingFile
             Returned if the file content matches an existing file.
 
         """
         if file_name is None:
             file_name = os.path.basename(file_path)
         file_size = os.path.getsize(file_path)
-        with open(file_path, 'rb') as f:
-            with tqdm(desc=f"[INFO] Uploading", total=file_size, unit="B", unit_scale=True, unit_divisor=1024) as t:
+        with open(file_path, "rb") as f:
+            with tqdm(
+                desc="[INFO] Uploading",
+                total=file_size,
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1024,
+            ) as t:
                 reader_wrapper = CallbackIOWrapper(t.update, f, "read")
 
                 files = {
-                    'document': (None, json.dumps({"fileName": file_name, "csvConfig":{}, "datasetId": self.id}), 'application/json'),
-                    'file': reader_wrapper
+                    "document": (
+                        None,
+                        json.dumps(
+                            {
+                                "fileName": file_name,
+                                "csvConfig": {},
+                                "datasetId": self.id,
+                            }
+                        ),
+                        "application/json",
+                    ),
+                    "file": reader_wrapper,
                 }
                 try:
-                    updated_dataset = self.client.http_post(f"/api/dataset/{self.id}/files/upload", files=files)
-                    #numRows is null when a file is first uploaded
+                    updated_dataset = self.client.http_post(
+                        f"/api/dataset/{self.id}/files/upload", files=files
+                    )
+                    # numRows is null when a file is first uploaded
                 except requests.exceptions.HTTPError as e:
-                    if e.response.status_code==409:
+                    if e.response.status_code == 409:
                         raise DatasetFileMatchesExistingFile(e)
                     else:
                         raise e
-        self.files = [DatasetFile(f['fileId'],f['fileName'],f.get('numRows'),f['numColumns'], f['processingStatus'], f.get('processingError')) for f in updated_dataset["files"]]
+        self.files = [
+            DatasetFile(
+                f["fileId"],
+                f["fileName"],
+                f.get("numRows"),
+                f["numColumns"],
+                f["processingStatus"],
+                f.get("processingError"),
+            )
+            for f in updated_dataset["files"]
+        ]
         self.num_columns = max([f.num_columns for f in self.files])
 
     def fetch_all_df(self) -> pd.DataFrame:
         """
         Fetches all of the data in the dataset as a pandas dataframe.
 
         Returns
@@ -104,22 +145,22 @@
             Dataset data in a pandas dataframe.
         """
         data = self._fetch_all()
 
         if self.num_columns is None:
             return pd.DataFrame()
 
-        #RAW file, not CSV
+        # RAW file, not CSV
         if self.num_columns == 0:
-            if len(data)==0:
+            if len(data) == 0:
                 return pd.DataFrame(columns=["text"])
             return pd.DataFrame(data, columns=["text"])
 
-        columns = ['col'+str(x) for x in range(self.num_columns)]
-        if len(data)==0:
+        columns = ["col" + str(x) for x in range(self.num_columns)]
+        if len(data) == 0:
             return pd.DataFrame(columns=columns)
         else:
             return pd.DataFrame(data, columns=columns)
 
     def fetch_all_json(self) -> str:
         """
         Fetches all of the data in the dataset as JSON.
@@ -140,76 +181,85 @@
         List[List[str]]
             The datset data.
         """
         response = []
         with requests.Session() as session:
             for file in self.files:
                 try:
-                    if file.num_columns==0:
-                        more_data = self.client.http_get_file(f"/api/dataset/{self.id}/files/{file.id}/get_data", session=session)
-                        response+=[[more_data]]
+                    if file.num_columns == 0:
+                        more_data = self.client.http_get_file(
+                            f"/api/dataset/{self.id}/files/{file.id}/get_data",
+                            session=session,
+                        )
+                        response += [[more_data]]
                     else:
-                        more_data = self.client.http_get(f"/api/dataset/{self.id}/files/{file.id}/get_data", session=session)
+                        more_data = self.client.http_get(
+                            f"/api/dataset/{self.id}/files/{file.id}/get_data",
+                            session=session,
+                        )
                         response += more_data
                 except requests.exceptions.HTTPError as e:
-                    if e.response.status_code==409:
+                    if e.response.status_code == 409:
                         continue
                     else:
                         raise e
             return response
 
     def get_processed_files(self) -> List[DatasetFile]:
         """
-        Gets all of the files in the dataset for which processing is complete. The data in these files is returned when data is requested.
+        Gets all of the files in the dataset for which processing is complete. The data
+        in these files is returned when data is requested.
 
         Returns
         ------
         List[DatasetFile]:
             The list of processed dataset files.
         """
-        return list(filter(lambda x: x.processing_status=="Completed" ,self.files))
+        return list(filter(lambda x: x.processing_status == "Completed", self.files))
 
     def get_queued_files(self) -> List[DatasetFile]:
         """
         Gets all of the files in the dataset that are waiting to be processed.
 
         Returns
         ------
         List[DatasetFile]:
             The list of dataset files that await processing.
         """
-        return list(filter(lambda x: x.processing_status=="Queued" ,self.files))
+        return list(filter(lambda x: x.processing_status == "Queued", self.files))
 
     def get_running_files(self) -> List[DatasetFile]:
         """
         Gets all of the files in the dataset that are currently being processed.
 
         Returns
         ------
         List[DatasetFile]:
             The list of files that are being processed.
         """
-        return list(filter(lambda x: x.processing_status=="Running" ,self.files))
+        return list(filter(lambda x: x.processing_status == "Running", self.files))
 
     def get_failed_files(self) -> List[DatasetFile]:
         """
-        Gets all of the files in dataset that encountered an error when they were processed. These files are effectively ignored.
+        Gets all of the files in dataset that encountered an error when they were
+        processed. These files are effectively ignored.
 
         Returns
         ------
         List[DatasetFile]:
             The list of files that had processing errors.
         """
-        return list(filter(lambda x: x.processing_status=="Failed" ,self.files))
+        return list(filter(lambda x: x.processing_status == "Failed", self.files))
 
     def _check_processing_and_update(self):
         """
-        Checks the processing status of the files in the dataset and updates the files list.
+        Checks the processing status of the files in the dataset and updates the files
+        list.
         """
-        if len(self.get_queued_files()+self.get_running_files()) > 0:
+        if len(self.get_queued_files() + self.get_running_files()) > 0:
             self.files = self.datasetfile_service.get_files(self.id)
 
     def describe(self):
         """
         Prints the dataset name, identifier, and the list of files.
 
         Examples
@@ -217,13 +267,21 @@
         >>> workspace.describe()
         Dataset: your_dataset_name [dataset_id]
         Number of Files: 2
         Number of Rows: 1000
         """
         self._check_processing_and_update()
 
-        print("Dataset: " + self.name + " [" + self.id + "]")
-        print("Number of Files: " + str(len(self.get_processed_files())))
-        print("Files that are waiting for processing: " + ", ".join([str((f.id,f.name)) for f in self.get_queued_files()+self.get_running_files()]))
-        print("Files that encountered errors while processing: " + ", ".join([str((f.id,f.name)) for f in self.get_failed_files()]))
-        print("Number of Rows: " + str(sum([x.num_rows if x.num_rows is not None else 0 for x in self.files])))
-        print("Number of rows fetched: " + str(self.total_rows_fetched))
+        files_waiting_for_proc = self.get_queued_files() + self.get_running_files()
+        files_with_error = self.get_failed_files()
+        number_rows = sum(
+            [x.num_rows if x.num_rows is not None else 0 for x in self.files]
+        )
+        result = f"Dataset: {self.name} [{self.id}]\n"
+        result += f"Number of Files: {len(self.get_processed_files())}\n"
+        result += "Files that are waiting for processing: "
+        result += f"{', '.join([str((f.id,f.name)) for f in files_waiting_for_proc])}\n"
+        result += "Files that encountered errors while processing: "
+        result += f"{', '.join([str((f.id,f.name)) for f in files_with_error])}\n"
+        result += f"Number of Rows: {number_rows}\n"
+        result += f"Number of rows fetched: {self.total_rows_fetched}"
+        return result
```

### Comparing `tonic_textual-1.4.0/tonic_textual/classes/datasetfile.py` & `tonic_textual-2.0.0/tonic_textual/classes/datasetfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Optional
+
+
 class DatasetFile:
     """
     Class to store the metadata for a dataset file.
 
     Parameters
     ----------
     id : str
@@ -13,32 +16,44 @@
     num_rows : long
         The number of rows in the dataset file.
 
     num_columns: int
         The number of columns in the dataset file.
 
     processing_status: string
-        The status of the dataset file in the processing pipeline. Possible values are 'Completed', 'Failed', 'Cancelled', 'Running', and 'Queued'.
-    
+        The status of the dataset file in the processing pipeline. Possible values are
+        'Completed', 'Failed', 'Cancelled', 'Running', and 'Queued'.
+
     processing_error: string
-        If the dataset file processing failed, a description of the issue that caused the failure.
+        If the dataset file processing failed, a description of the issue that caused
+        the failure.
 
     uploaded_timestamp: str
         Timestamp in UTC when dataset file was uploaded to the dataset.
     """
-    def __init__(self, id: str, name: str, num_rows: int, num_columns: int, processing_status: str, processing_error: str):
+
+    def __init__(
+        self,
+        id: str,
+        name: str,
+        num_rows: Optional[int],
+        num_columns: int,
+        processing_status: str,
+        processing_error: Optional[str],
+    ):
         self.id = id
         self.name = name
         self.num_rows = num_rows
         self.num_columns = num_columns
         self.processing_status = processing_status
         self.processing_error = processing_error
 
     def describe(self):
-        """Prints the dataset file metadata. Includes the identifier, file name, number of rows, and number of columns.
-        """
-        print("File: " + self.name + " [" + self.id + "]")
-        print("Number of rows: " + self.num_rows)
-        print("Number of columns: " + self.num_columns)
-        print("Status: " + self.processing_status)
-        if self.processing_status!="" and self.processing_error is not None:
-            print("Error: " + self.processing_error)
+        """Returns the dataset file metadata as string. Includes the identifier, file
+        name, number of rows, and number of columns."""
+        description = f"File: {self.name} [{self.id}]\n"
+        description += f"Number of rows: {self.num_rows}\n"
+        description += f"Number of columns: {self.num_columns}\n"
+        description += f"Status: {self.processing_status}\n"
+        if self.processing_status != "" and self.processing_error is not None:
+            description += f"Error: {self.processing_error}\n"
+        return description
```

### Comparing `tonic_textual-1.4.0/tonic_textual/classes/httpclient.py` & `tonic_textual-2.0.0/tonic_textual/classes/httpclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import requests
 from urllib3.exceptions import InsecureRequestWarning
 
-from tonic_textual.classes.tonic_exception import ErrorWhenDownloadFile, FileNotReadyForDownload, LicenseInvalid
+from tonic_textual.classes.tonic_exception import (
+    ErrorWhenDownloadFile,
+    FileNotReadyForDownload,
+    LicenseInvalid,
+)
+
+requests.packages.urllib3.disable_warnings(  # type: ignore
+    category=InsecureRequestWarning
+)
 
-requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
 class HttpClient:
     """Client used to handle requests to the Tonic Textual instance.
 
     Parameters
     ----------
     base_url : str
@@ -16,33 +23,42 @@
         The API token associated to use for the requests.
     verify : bool
         Whether SSL Certification verification is performed
     """
 
     def __init__(self, base_url: str, api_key: str, verify: bool):
         self.base_url = base_url
-        self.headers = {"Authorization": api_key, "User-Agent": "tonic-textual-python-sdk"}
+        self.headers = {
+            "Authorization": api_key,
+            "User-Agent": "tonic-textual-python-sdk",
+        }
         self.verify = verify
 
-    def http_get_file(self, url: str, session: requests.Session, params: dict={}) -> bytes:
+    def http_get_file(
+        self, url: str, session: requests.Session, params: dict = {}
+    ) -> str:
         """Makes a get request to get a file.
 
         Parameters
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.get request.
 
         """
-        res = session.get(self.base_url + url, params=params, headers=self.headers, verify=self.verify)
+        res = session.get(
+            self.base_url + url, params=params, headers=self.headers, verify=self.verify
+        )
         res.raise_for_status()
-        return res.content.decode('utf-8')
-    
-    def http_post_download_file(self, url: str, params: dict={}, data={}, additional_headers={}) -> bytes:
+        return res.content.decode("utf-8")
+
+    def http_post_download_file(
+        self, url: str, params: dict = {}, data={}, additional_headers={}
+    ) -> bytes:
         """Makes a POST request to download a file.
 
         Parameters
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
@@ -50,69 +66,80 @@
         data: dict
             Request body
         additionaHeaders: dict
             Additional HTTP request headers
         """
 
         res = requests.post(
-            self.base_url + url, params=params, json=data, headers=self.headers | additional_headers, verify=self.verify
+            self.base_url + url,
+            params=params,
+            json=data,
+            headers=self.headers | additional_headers,
+            verify=self.verify,
         )
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            if err.response.status_code==422:
+            if err.response.status_code == 422:
                 raise LicenseInvalid(err)
-            if err.response.status_code==409:
+            if err.response.status_code == 409:
                 raise FileNotReadyForDownload("File not yet ready for download")
-            if err.response.status_code==500:
-                raise ErrorWhenDownloadFile(err)            
+            if err.response.status_code == 500:
+                raise ErrorWhenDownloadFile(err)
             else:
-                raise err            
-        
+                raise err
+
         return res.content
 
-    def http_get(self, url: str, session: requests.Session, params: dict={}):
+    def http_get(self, url: str, session: requests.Session, params: dict = {}):
         """Makes a get request.
 
         Parameters
         ----------
         url : str
             URL to make the get request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.get request.
 
         """
-        res = session.get(self.base_url + url, params=params, headers=self.headers, verify=self.verify)
+        res = session.get(
+            self.base_url + url, params=params, headers=self.headers, verify=self.verify
+        )
         res.raise_for_status()
         return res.json()
 
     def http_post(self, url, params={}, data={}, files={}, additional_headers={}):
         """Make a post request.
 
         Parameters
         ----------
         url : str
             URL to make the post request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.post request.
         data: dict
             Passed as the data parameter of the requests.post request.
-        """           
+        """
 
         res = requests.post(
-            self.base_url + url, params=params, json=data, headers=self.headers | additional_headers, verify=self.verify, files=files
+            self.base_url + url,
+            params=params,
+            json=data,
+            headers=self.headers | additional_headers,
+            verify=self.verify,
+            files=files,
         )
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError as err:
-            if err.response.status_code==422:
+            if err.response.status_code == 422:
                 raise LicenseInvalid(err)
             else:
-                raise err            
-        
+                raise err
+
         return res.json()
 
     def http_put(self, url, params={}, data={}, files={}):
         """Makes a put request.
 
         Parameters
         ----------
@@ -120,16 +147,22 @@
             URL to make the put request. The URL is appended to self.base_url.
         params: dict
             Passed as the params parameter of the requests.put request.
         data: dict
             Passed as the data parameter of the requests.put request.
         """
         res = requests.put(
-            self.base_url + url, params=params, json=data, headers=self.headers, verify=self.verify
+            self.base_url + url,
+            params=params,
+            json=data,
+            headers=self.headers,
+            verify=self.verify,
         )
         res.raise_for_status()
         return res.json()
 
     def http_delete(self, url, params={}):
-        res = requests.delete(self.base_url + url, params = params, headers = self.headers, verify = self.verify)
+        res = requests.delete(
+            self.base_url + url, params=params, headers=self.headers, verify=self.verify
+        )
         res.raise_for_status()
         return res.json()
```

### Comparing `tonic_textual-1.4.0/tonic_textual/classes/tonic_exception.py` & `tonic_textual-2.0.0/tonic_textual/classes/tonic_exception.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,88 @@
 from requests.exceptions import HTTPError
 
+
 class DatasetNameAlreadyExists(Exception):
     """
-        Raised when there is an attempt to create a dataset with a name that already exists.
+    Raised when there is an attempt to create a dataset with a name that already exists.
     """
+
     def __init__(self, errors):
         # Call the base class constructor with the parameters it needs
-        super().__init__("The dataset name already exists. Dataset names must be unique. Choose a different name.")
+        super().__init__(
+            "The dataset name already exists. Dataset names must be unique. Choose a "
+            "different name."
+        )
         self.errors = errors
 
+
 class DatasetFileMatchesExistingFile(HTTPError):
     """
-        Raised when the content in a file to upload matches the content in an existing file in the dataset.
+    Raised when the content in a file to upload matches the content in an existing file
+    in the dataset.
     """
+
     def __init__(self, errors):
-        super().__init__(errors.response.content or "The file content matches content in an existing dataset file. Choose a different file.")
+        message = (
+            "The file content matches content in an existing dataset file. Choose a "
+            "different file."
+        )
+
+        super().__init__(errors.response.content or message)
         self.errors = errors
 
+
 class InvalidJsonForRedactionRequest(Exception):
     """
-        Raised when the JSON redaction request contains invalid JSON
+    Raised when the JSON redaction request contains invalid JSON
     """
+
     def __init__(self, msg):
         super().__init__(msg)
 
+
 class LicenseInvalid(HTTPError):
     """
-        Raised when either your license has expired OR you've exceeded your allowed word limit
+    Raised when either your license has expired OR you've exceeded your allowed word
+    limit
     """
+
     def __init__(self, errors):
-        super().__init__(str(errors.response.content) or "Invalid Textual license. Please reach out to textual@tonic.ai.")
+        super().__init__(
+            str(errors.response.content)
+            or "Invalid Textual license. Please reach out to textual@tonic.ai."
+        )
         self.errors = errors
 
+
 class FileNotReadyForDownload(Exception):
     """
-        Raised when you make a reques to download a file that is not yet ready for download
+    Raised when you make a reques to download a file that is not yet ready for download
     """
+
     def __init__(self, msg):
         super().__init__(msg)
 
+
 class ErrorWhenDownloadFile(HTTPError):
     """
-        Raised when server returns 500 when attempting to download file
+    Raised when server returns 500 when attempting to download file
     """
+
     def __init__(self, errors):
-        super().__init__("Either error occured while downloading file or the file redaction job was cancelled.")
+        super().__init__(
+            "Either error occured while downloading file or the file redaction job was "
+            "cancelled."
+        )
         self.errors = errors
-        
+
+class JobsNotSuccessful(HTTPError):
+    """
+    Raised when at least one of the jobs in the comparison has not completed successfully
+    """
+    def __init__(self, errors):
+        super().__init__(
+            "Both jobs must have completed successfully"
+        )
+        self.response = errors.response
+        self.request = errors.request
+
```

### Comparing `tonic_textual-1.4.0/PKG-INFO` & `tonic_textual-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-textual
-Version: 1.4.0
+Version: 2.0.0
 Summary: Wrappers around the Tonic Textual API
 Home-page: https://www.tonic.ai/
 License: MIT
 Keywords: tonic.ai,tonic,tonic textual
 Author: Adam Kamor
 Author-email: adam@tonic.ai
 Requires-Python: >=3.7,<4.0
@@ -12,29 +12,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: more-itertools (>=8.6.0,<9.0.0)
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Overview
 This library contains useful wrappers around the Tonic Textual API
 
 ## Usage
 
 Instantiate the API wrapper using the following code:
 
 ```
-from tonic_textual.api import TonicTextual
+from tonic_textual.redact_api import TonicTextual
 
 # Do not include trailing backslash in TONIC_URL
 api = TonicTextual(TONIC_TEXTUAL_URL, API_KEY)
 ```
 
 Once instantiated, the following endpoints are available for consumption. Note that available endpoints and response types are limited. Available fields may be severely limited compared to the current Tonic API.
```

