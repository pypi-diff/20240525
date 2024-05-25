# Comparing `tmp/armis-1.0.21.tar.gz` & `tmp/armis-1.0.22.tar.gz`

## Comparing `armis-1.0.21.tar` & `armis-1.0.22.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 armis-1.0.21/requirements.txt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 armis-1.0.21/src/armis/__about__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 armis-1.0.21/src/armis/__init__.py
--rwxr-xr-x   0        0        0    53264 2020-02-02 00:00:00.000000 armis-1.0.21/src/armis/armiscloud.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_apicalls.py
--rwxr-xr-x   0        0        0     2088 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_boundaries.py
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_ceiling.py
--rwxr-xr-x   0        0        0      751 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_collectors.py
--rwxr-xr-x   0        0        0     2149 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_devices.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_fixture.py
--rwxr-xr-x   0        0        0     1163 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_integrations.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_notimplemented.py
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_objectcreation.py
--rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_sites.py
--rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_tagging.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 armis-1.0.21/tests/test_users.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 armis-1.0.21/.gitignore
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 armis-1.0.21/README.md
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 armis-1.0.21/pyproject.toml
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 armis-1.0.21/PKG-INFO
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 armis-1.0.22/CHANGELOG.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 armis-1.0.22/requirements.txt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 armis-1.0.22/src/armis/__about__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 armis-1.0.22/src/armis/__init__.py
+-rwxr-xr-x   0        0        0    63058 2020-02-02 00:00:00.000000 armis-1.0.22/src/armis/armiscloud.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_apicalls.py
+-rwxr-xr-x   0        0        0     2086 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_boundaries.py
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_ceiling.py
+-rwxr-xr-x   0        0        0      749 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_collectors.py
+-rwxr-xr-x   0        0        0     2155 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_devices.py
+-rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_fixture.py
+-rwxr-xr-x   0        0        0     1966 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_integrations.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_notimplemented.py
+-rwxr-xr-x   0        0        0     1644 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_objectcreation.py
+-rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_search.py
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_sites.py
+-rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_tagging.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 armis-1.0.22/tests/test_users.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 armis-1.0.22/.gitignore
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 armis-1.0.22/LICENSE.md
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 armis-1.0.22/README.md
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 armis-1.0.22/pyproject.toml
+-rw-r--r--   0        0        0     9544 2020-02-02 00:00:00.000000 armis-1.0.22/PKG-INFO
```

### Comparing `armis-1.0.21/src/armis/armiscloud.py` & `armis-1.0.22/src/armis/armiscloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/python3
 
 # SPDX-FileCopyrightText: 2024-present Matthew Lange <mmlange@gmail.com>
 # SPDX-License-Identifier: BSD-3-Clause
 
+from __future__ import annotations
+
 import contextlib
 import gzip
 import logging
-import logging.handlers
 import math
 import pathlib as pl
 import tempfile
 import warnings
+from typing import Union
 
 import httpx
 import msgspec
 import pendulum
 from furl import furl
 from tenacity import (
     Retrying,
@@ -136,29 +138,30 @@
         if tenant_hostname is None:
             raise ValueError("tenant_hostname is required")
 
         self.TENANT_BASE_URL = furl()
         self.TENANT_BASE_URL.scheme = "https"
         self.TENANT_BASE_URL.host = tenant_hostname
         self.TENANT_BASE_URL.path = "/api/"
+        self.log.debug("TENANT_BASE_URL=%s", str(self.TENANT_BASE_URL))
 
         # Note that if you're making multiple calls to decode, it's more efficient
         # to create a Decoder once and use the Decoder.decode method instead.
         self._json_decoder = msgspec.json.Decoder()
         self._json_encoder = msgspec.json.Encoder()
 
     # cleanup
     def __del__(self):
         # close all outstanding httpx connections
         with contextlib.suppress(Exception):
             self.httpx_client.close()
 
     @staticmethod
     def _ceiling_up(number, nearest: int):
-        if not isinstance(number, (int, float)):  # noqa: UP038
+        if not isinstance(number, (int, float)):
             raise ValueError("number " + str(number) + " is not an int or float")
         if nearest is None:
             raise ValueError("nearest was not provided")
 
         return math.ceil(number / nearest) * nearest
 
     def _get_httpx_client(self):
@@ -478,15 +481,15 @@
         self.log.debug("return text=%s", str(boundary_create.text))
         self.log.debug("status_code=%s", str(boundary_create.status_code))
 
         # when creating a boundary, you get 201 back if it was created
         if boundary_create.status_code != httpx.codes.CREATED:
             self.log.info("FAILED boundary create for name: %s", str(name))
             self.log.debug(boundary_create.text)
-            raise Exception("boundary update issue", boundary_create.text)
+            raise RuntimeError("boundary update issue", boundary_create.text)
 
         return self._json_decoder.decode(boundary_create.text)
 
     def delete_boundary(self, boundary_id: int) -> dict:
         """Delete a boundary given a boundary_id.
 
         Parameters
@@ -500,15 +503,15 @@
         """
         url = self.TENANT_BASE_URL / f"v1/boundaries/{boundary_id}/"
         self.log.debug("url=%s", str(url))
         boundary_delete = self._api_http_request(method="DELETE", url=url)
         if boundary_delete.status_code != httpx.codes.NO_CONTENT:
             self.log.critical("STATUS CODE != 204")
             self.log.critical("status_code=%s", str(boundary_delete.status_code))
-            raise Exception("boundary_delete issue", boundary_delete.text)
+            raise RuntimeError("boundary_delete issue", boundary_delete.text)
 
         if boundary_delete.status_code == httpx.codes.NO_CONTENT:
             return {"success": True}
         return {"success": False}
 
     def get_boundary(self, boundary_id: int) -> dict:
         """Get a boundary given a boundary_id.
@@ -664,15 +667,15 @@
         self.log.debug("status_code=%s", str(boundary_update.status_code))
         if boundary_update.status_code != httpx.codes.OK:
             self.log.info(
                 "FAILED boundary update for boundary_id: %s",
                 str(boundary_id),
             )
             self.log.debug(boundary_update.text)
-            raise Exception("boundary update issue", boundary_update.text)
+            raise RuntimeError("boundary update issue", boundary_update.text)
 
     def get_collector(self, collector_id: int) -> dict:
         """Get a collector given the collector_id.
 
         Parameters
         ----------
         collector_id: int
@@ -688,15 +691,15 @@
 
         self.log.info("collector_id=%s", str(collector_id))
         url = self.TENANT_BASE_URL / f"v1/collectors/{collector_id}/"
 
         self.log.debug("url=%s", str(url))
         collector_request = self._api_http_request(method="GET", url=url)
         if collector_request.status_code != httpx.codes.OK:
-            raise Exception("collector issue", collector_request.text)
+            raise RuntimeError("collector issue", collector_request.text)
 
         return self._json_decoder.decode(collector_request.text)["data"]
 
     def get_collectors(self) -> dict:
         """Get a dictionary of collectors.
 
         Returns
@@ -806,15 +809,15 @@
         if collector_update.status_code != httpx.codes.OK:
             self.log.info(
                 "FAILED collector rename for collector_id=%s, new_name=%s",
                 str(collector_id),
                 new_name,
             )
             self.log.debug(collector_update.text)
-            raise Exception("collector rename issue", collector_update.text)
+            raise RuntimeError("collector rename issue", collector_update.text)
 
         return self._json_decoder.decode(collector_update.text)
 
     def get_devices(self, **kwargs: dict) -> list:
         """Get devices from inventory matching ASQ.
 
         Parameters
@@ -1015,15 +1018,15 @@
         url.args["length"] = 1
         url.args["from"] = 0
         url.args["fields"] = "id"
         self.log.debug("url=%s", str(url))
 
         inventory_total_request = self._api_http_request(method="GET", url=url)
         if inventory_total_request.status_code != httpx.codes.OK:
-            raise Exception(
+            raise RuntimeError(
                 "inventory issue",
                 inventory_total_request.text,
             )  # pragma: no cover
 
         inventory_total = int(
             self._json_decoder.decode(inventory_total_request.text)["data"]["total"],
         )
@@ -1094,18 +1097,91 @@
             )
 
         self.log.debug("return text=%s", str(tag_device_update.text))
         self.log.debug("status_code=%s", str(tag_device_update.status_code))
         if tag_device_update.status_code != httpx.codes.OK:
             self.log.info("FAILED DEVICE TAG for device ID: %s", str(device_id))
             self.log.debug(tag_device_update.text)
-            raise Exception("tag_device_update issue", tag_device_update.text)
+            raise RuntimeError("tag_device_update issue", tag_device_update.text)
 
         return tag_device_update.text
 
+    def create_integration(self, **kwargs: dict) -> dict:
+        """Create an integration.
+
+        Parameters
+        ----------
+        collector_id : int
+            ID of the collector
+        integration_name : str
+            name of the integration
+        integration_type : str
+            the type of integration
+        integration_params : dict
+            integration-specific parameters
+
+        Returns
+        -------
+        status : dict
+            Status of action as returned by the cloud
+
+        Notes
+        -----
+        This method requires v2 of the API call which is only available in the
+        Armis Cloud version >=R-24.0.
+
+        Examples
+        --------
+        From the Armis online Swagger documentation, the payload looks like this:
+
+        ```
+        {
+            "collectorId": 1,
+            "instance": "My Integration",
+            "name": "SPAN/TAP",
+            "params": {"sniff_interface": "eno1"},
+        }
+        ```
+
+        """
+        collector_id = kwargs.get("collector_id", None)
+        integration_name = kwargs.get("integration_name", None)
+        integration_type = kwargs.get("integration_type", None)
+        integration_params = kwargs.get("integration_params", None)
+
+        if (
+            collector_id is None
+            or integration_name is None
+            or integration_params is None
+            or integration_type is None
+        ):
+            raise ValueError(
+                "no collector_id, integration_name, integrations_params, "
+                "or integration_type",
+            )
+
+        url = self.TENANT_BASE_URL / "v2/integrations/"
+
+        # from the Armis API documentation
+        integration_payload = {
+            "collectorId": collector_id,
+            "instance": integration_name,
+            "name": integration_type,
+            "params": integration_params,
+        }
+
+        self.log.debug("data to be posted=%s", str(integration_payload))
+        create_integration_request = self._api_http_request(
+            method="POST",
+            url=url,
+            json=integration_payload,
+        )
+
+        return self._json_decoder.decode(create_integration_request.text)
+
     def get_integration(self, integration_id: int):
         """Get an integration given an integration_id.
 
         Parameters
         ----------
         integration_id : int
             Desired integration_id
@@ -1136,15 +1212,15 @@
         if integration_details.status_code != httpx.codes.OK:
             self.log.critical("STATUS CODE=%s", integration_details.status_code)
             self.log.debug(
                 "status_code=%s",
                 str(integration_details.status_code),
             )
             self.log.debug("text=%s", integration_details.text)
-            raise Exception("integration_details issue", integration_details.text)
+            raise RuntimeError("integration_details issue", integration_details.text)
 
         integration = self._json_decoder.decode(integration_details.text)["data"][0]
         return integration  # noqa: RET504
 
     def get_integrations(self) -> dict:
         """Get a list of integrations.
 
@@ -1180,15 +1256,18 @@
             if integrations_details.status_code != httpx.codes.OK:
                 self.log.critical("STATUS CODE != 200")
                 self.log.critical(
                     "status_code=%s",
                     str(integrations_details.status_code),
                 )
                 self.log.critical("text=%s", integrations_details.text)
-                raise Exception("integrations_details issue", integrations_details.text)
+                raise RuntimeError(
+                    "integrations_details issue",
+                    integrations_details.text,
+                )
 
             for integration in self._json_decoder.decode(integrations_details.text)[
                 "data"
             ]["integrations"]:
                 integrationid = integration["id"]
                 integrations[integrationid] = integration
 
@@ -1216,14 +1295,215 @@
         """
         url = self.TENANT_BASE_URL / "v2/integrations/"
         url.args["length"] = 1
         self.log.debug("url=%s", str(url))
         count_request = self._api_http_request(method="GET", url=url)
         return int(self._json_decoder.decode(count_request.text)["data"]["total"])
 
+    def delete_integration(self, integration_id) -> dict:
+        """Delete an integration given the integration_id.
+
+        Parameters
+        ----------
+        integration_id : int
+            An integration_id to delete.
+
+        Returns
+        -------
+        delete_integration_result : dict
+            Result of the delete action, directly from the cloud.
+        """
+        url = self.TENANT_BASE_URL / f"v2/integrations/{integration_id}/"
+        self.log.debug("url=%s", url)
+        integration_delete = self._api_http_request(method="DELETE", url=url)
+        if integration_delete.status_code != httpx.codes.OK:
+            self.log.critical("STATUS CODE !=200")
+            self.log.critical("status_code=%s", str(integration_delete.status_code))
+            self.log.critical("text=%s", integration_delete.text)
+            raise RuntimeError("integration_details issue", integration_delete.text)
+
+        return self._json_decoder.decode(integration_delete.text)
+
+    def get_search(self, asq: str, **kwargs: dict) -> dict:
+        """Returns search result for given ASQ string.
+
+        Parameters
+        ----------
+        asq : str
+            ASQ search string
+        fields_wanted : list
+            List of fields wanted.
+
+        Returns
+        -------
+        records: list
+            Records matching ASQ
+
+        Notes
+        -----
+        This is different from the `get_devices` method, which only allows
+        you to retrieve devices.  This method allows you to retrieve data
+        with any valid ASQ, including records from `in:devices` queries.
+        """
+        get_search_start = pendulum.now()
+
+        self.log.info("asq=%s", asq)
+        fields_wanted: list = kwargs.get("fields_wanted", [])
+        if isinstance(fields_wanted, str):
+            fields_wanted = [fields_wanted]
+        self.log.info("fields_wanted=%s", str(",".join(fields_wanted)))
+
+        url = self.TENANT_BASE_URL / "v1/search/"
+        url.args["aql"] = asq
+        url.args["from"] = 0
+        url.args["length"] = self.ARMIS_API_PAGE_SIZE
+
+        if len(fields_wanted) > 0:
+            url.args["fields"] = ",".join(fields_wanted)
+
+        records = []
+        records_total = self.get_search_count(asq=asq)
+        remaining_time = -1
+
+        filenames = []
+        filenumber = 1
+
+        while url.args["from"] is not None:
+            self.log.info(
+                "fetching %s-%s of a total of %s",
+                str(url.args["from"]),
+                str(url.args["from"] + self.ARMIS_API_PAGE_SIZE),
+                str(records_total),
+            )
+            search_details = self._api_http_request(method="GET", url=url)
+
+            if search_details.status_code != httpx.codes.OK:
+                self.log.critical("STATUS CODE !=200")
+                self.log.critical("status_code=%s", str(search_details.status_code))
+                self.log.critical("text=%s", search_details.text)
+                self.log.critical("continuing")
+                continue
+
+            data = self._json_decoder.decode(search_details.text)
+            totalresults = data["data"]["total"]
+            if totalresults == 0:
+                return []
+
+            if len(data["data"]["results"]) > 0:
+                fetchedcolumns = list(data["data"]["results"][0].keys())
+                self.log.debug("Fetched columns=%s", str(fetchedcolumns))
+                setdiff = set(fields_wanted).difference(fetchedcolumns)
+                if len(setdiff) > 0:
+                    self.log.info(
+                        "Fields missing from wanted columns=%s",
+                        ",".join(list(setdiff)),
+                    )
+                    raise ValueError(
+                        "Fields wanted="
+                        + ",".join(fields_wanted)
+                        + "\nFields fetched="
+                        + ",".join(fetchedcolumns)
+                        + "\nFields missing from wanted columns="
+                        + ",".join(list(setdiff)),
+                    )
+            else:
+                self.log.debug("no data, data=%s", str(data))
+                return []
+
+            now = pendulum.now()
+            filename = pl.Path(
+                str(self.temporary_directory.name)
+                + "/"
+                + f"search_results_{now.float_timestamp}.json.gz",
+            )
+            self.log.info("search_results filename=%s", str(filename))
+            # using default zlib compression level (i.e. -1 AKA 6)
+            filename.write_bytes(gzip.compress(search_details.content))
+            filenames.append(filename)
+            filenumber += 1
+
+            now = pendulum.now()
+            self.log.debug("now=%s", str(now))
+            self.log.debug("get_search_start=%s", str(get_search_start))
+
+            elapsed_time = now.timestamp() - get_search_start.timestamp()
+            self.log.debug("elapsed_time=%s", str(elapsed_time))
+
+            if url.args["from"] > 0:
+                time_per_record = elapsed_time / url.args["from"]
+                self.log.debug("time_per_record=%s", str(time_per_record))
+
+                remaining_records = records_total - url.args["from"]
+                self.log.debug("remaining_records=%s", str(remaining_records))
+
+                remaining_time = remaining_records * time_per_record
+                self.log.debug("remaining_time=%s", str(remaining_time))
+
+            if remaining_time < 0:
+                estimated_end_time = now
+            else:
+                estimated_end_time = now.add(seconds=remaining_time)
+
+            self.log.info("estimated_end_time=%s", str(estimated_end_time))
+
+            url.args["from"] = data["data"]["next"]
+
+        # reproduce inventory here
+        for filename in filenames:
+            filename = pl.Path(filename)
+            self.log.info("reading filename=%s", str(filename.name))
+            j = self._json_decoder.decode(gzip.decompress(filename.read_bytes()))
+            self.log.info("appending %s records", str(len(j["data"])))
+            records.extend(j["data"]["results"])
+
+        self.log.debug("records size=%s", str(len(records)))
+
+        # clean up tmpdirectory
+        for filename in filenames:
+            filename = pl.Path(filename)
+            filename.unlink(missing_ok=True)
+
+        if len(records) > 0:
+            return records
+
+        return []
+
+    def get_search_count(self, asq: str) -> int:
+        """Get a count of records using ASQ.
+
+        Parameters
+        ----------
+        asq : str
+            ASQ to search for records.
+
+        Returns
+        -------
+        count: int
+            A count of records matching ASQ.
+        """
+        self.log.info("asq=%s", asq)
+        url = self.TENANT_BASE_URL / "v1/search/"
+
+        # Armis still calls this AQL in their API
+        url.args["aql"] = asq
+        url.args["length"] = 1
+        url.args["from"] = 0
+        url.args["fields"] = "id"
+        self.log.debug("url=%s", str(url))
+
+        search_total_request = self._api_http_request(method="GET", url=url)
+        if search_total_request.status_code != httpx.codes.OK:
+            raise RuntimeError("search retults issue", search_total_request.text)
+
+        search_total = int(
+            self._json_decoder.decode(search_total_request.text)["data"]["total"],
+        )
+        self.log.info("search_total=%s", str(search_total))
+        return search_total
+
     def get_sites(self) -> dict:
         """Get a list of sites.
 
         Returns
         -------
         sites : dict
             A dict of sites.
@@ -1283,15 +1563,15 @@
 
         site_request = self._api_http_request(method="GET", url=url)
         if site_request.status_code != httpx.codes.OK:
             self.log.critical("STATUS CODE !=200")
             self.log.critical("status_code=%s", str(site_request.status_code))
             self.log.critical("text=%s", site_request.text)
             self.log.critical("continuing")
-            raise Exception("dashboard http response !=200")
+            raise RuntimeError("dashboard http response !=200")
 
         if "data" in self._json_decoder.decode(site_request.text):
             return self._json_decoder.decode(site_request.text)["data"]
         return {}
 
     def delete_user(self, user_id_or_email):
         """Delete a user given the user_id or email.
@@ -1311,19 +1591,19 @@
 
         user_delete = self._api_http_request(method="DELETE", url=url)
         self.log.debug("return text=%s", str(user_delete.text))
         self.log.debug("status_code=%s", str(user_delete.status_code))
         if user_delete.status_code != httpx.codes.OK:
             self.log.info("FAILED USER UPDATE for user: %s", str(user_id_or_email))
             self.log.debug(user_delete.text)
-            raise Exception("delete user issue", user_delete.text)
+            raise RuntimeError("delete user issue", user_delete.text)
 
         return self._json_decoder.decode(user_delete.text)
 
-    def edit_user(self, user_id_or_email: str | int, **kwargs: dict) -> dict:
+    def edit_user(self, user_id_or_email: Union[str, int], **kwargs: dict) -> dict:
         """Edit a user given the user_id or email.
 
         Parameters
         ----------
         user_id_or_email : str|int
             user_id (int) or email (str) to change
         email : str
@@ -1373,15 +1653,15 @@
         if None in list(edit_user_dict.values()):
             need_data_from_cloud = True
 
         if need_data_from_cloud:
             try:
                 existinguser = self.get_user(user_id_or_email=user_id_or_email)
             except RuntimeError as e:
-                raise RuntimeError(e)
+                raise RuntimeError(e) from e
             for required_attribute in required_attributes:
                 if edit_user_dict[required_attribute] is None:
                     edit_user_dict[required_attribute] = existinguser[
                         required_attribute
                     ]
         for optional_attribute in optional_attributes:
             optional_attribute_value = kwargs.get(optional_attribute, None)
@@ -1397,15 +1677,15 @@
             json=edit_user_dict,
         )
         self.log.debug("return text=%s", str(user_update.text))
         self.log.debug("status_code=%s", str(user_update.status_code))
         if user_update.status_code != httpx.codes.OK:
             self.log.info("FAILED USER UPDATE for user: %s", str(user_id_or_email))
             self.log.debug(user_update.text)
-            raise Exception("edit user issue", user_update.text)
+            raise RuntimeError("edit user issue", user_update.text)
 
         return self._json_decoder.decode(user_update.text)
 
     def get_user(self, user_id_or_email, **kwargs):
         """Get a user by user_id or email.
 
         Parameters
@@ -1460,15 +1740,15 @@
         self.log.debug("url=%s", str(url))
         users_details = self._api_http_request(method="GET", url=url)
 
         if users_details.status_code != httpx.codes.OK:
             self.log.critical("STATUS CODE !=200")
             self.log.critical("status_code=%s", str(users_details.status_code))
             self.log.critical("text=%s", users_details.text)
-            raise Exception("users_details issue", users_details.text)
+            raise RuntimeError("users_details issue", users_details.text)
 
         users = {}
         data = self._json_decoder.decode(users_details.text)
         if "users" in data["data"]:
             for user in data["data"]["users"]:
                 users[user["id"]] = user
```

### Comparing `armis-1.0.21/tests/test_apicalls.py` & `armis-1.0.22/tests/test_apicalls.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.21/tests/test_boundaries.py` & `armis-1.0.22/tests/test_boundaries.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import random
 
 import pytest
 from test_fixture import armis_object
 
 
-@pytest.fixture()
+@pytest.fixture
 def boundaries(armis_object):
     return armis_object.get_boundaries()
 
 
 def test_get_boundaries(boundaries):
     assert len(list(boundaries.keys())) > 0
```

### Comparing `armis-1.0.21/tests/test_ceiling.py` & `armis-1.0.22/tests/test_ceiling.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.21/tests/test_collectors.py` & `armis-1.0.22/tests/test_collectors.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import random
 
 import pytest
 from test_fixture import armis_object
 
 
-@pytest.fixture()
+@pytest.fixture
 def collectors(armis_object):
     return armis_object.get_collectors()
 
 
 def test_get_collectors(armis_object, collectors):
     for _ in range(5):
         randomcollectorid = random.choice(list(collectors.keys()))
```

### Comparing `armis-1.0.21/tests/test_devices.py` & `armis-1.0.22/tests/test_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 import tenacity
 from test_fixture import armis_object
 
 
 @pytest.fixture(scope="module")
 def device_asq():
-    return 'in:devices timeFrame:"1 Minutes"'
+    return 'in:devices timeFrame:"10 Minutes"'
 
 
 def test_get_devices_count(armis_object, device_asq):
     x = armis_object.get_devices_count(
         asq=device_asq,
     )
     assert x >= 0
@@ -29,22 +29,22 @@
         armis_object.get_devices_count(asq="in:nothing")
 
 
 def test_get_devices(armis_object, device_asq):
     x = armis_object.get_devices(
         asq=device_asq,
     )
-    assert len(x) >= 0
+    assert len(x) > 0
 
 
 def test_get_devices_mismatched_fields(armis_object, device_asq):
     with pytest.raises(ValueError):
         armis_object.get_devices(
             asq=device_asq,
-            fields_wanted=["not", "valid", "fields"],
+            fields_wanted=["id", "not", "valid", "fields"],
         )
 
 
 def test_get_devices_ensure_fields_match(armis_object, device_asq):
     fields_wanted = [
         "id",
         "boundaries",
```

### Comparing `armis-1.0.21/tests/test_fixture.py` & `armis-1.0.22/tests/test_fixture.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/python3
 # ruff: noqa: F811,SLF001,D103
 import pathlib as pl
 
 import pytest
-from armis import ArmisCloud
 from dotenv import dotenv_values
 
+from armis import ArmisCloud
+
 envfile = pl.Path.home() / ".env"
 config = dotenv_values(envfile)
 
 
 @pytest.fixture(scope="module")
 def armis_object():
     if "TEST_ARMIS_TENANT_HOSTNAME" not in config:
```

### Comparing `armis-1.0.21/tests/test_integrations.py` & `armis-1.0.22/tests/test_integrations.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,7 +34,36 @@
     integrationid_invalid = random.randint(
         integration_ids[-1] * 2,
         integration_ids[-1] * 2222,
     )
 
     integration_invalid = armis_object.get_integration(integrationid_invalid)
     assert len(integration_invalid) == 0
+
+
+@pytest.fixture
+def integration(armis_object):
+    random_number = random.randint(0, 939393339)
+    random_name = f"Test Integration #{random_number}"
+    x = armis_object.create_integration(
+        collector_id=9157,
+        integration_name=random_name,
+        integration_type="SWITCH",
+        integration_params={"sniff_interface": "eno5"},
+    )
+    return x
+
+
+def test_create_integration(integration):
+    integration_id = integration["data"]["id"]
+    print("integration_id=", integration_id)
+
+    assert integration_id > 0
+
+
+def test_delete_integration(integration, armis_object):
+    integration_id = integration["data"]["id"]
+
+    print("deleting integration_id=", integration_id)
+    x = armis_object.delete_integration(integration_id)
+    print("x=", x)
+    assert x["success"] is True
```

### Comparing `armis-1.0.21/tests/test_objectcreation.py` & `armis-1.0.22/tests/test_objectcreation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/python3
 # ruff: noqa: F811,SLF001,D103
 import pathlib as pl
 
 import pytest
-from armis import ArmisCloud
 from dotenv import dotenv_values
 
+from armis import ArmisCloud
+
 
 @pytest.fixture(scope="module")
 def config():
     envfile = pl.Path.home() / ".env"
     config = dotenv_values(envfile)
     if "TEST_ARMIS_TENANT_HOSTNAME" not in config:
         pytest.skip("missing TEST_ARMIS_TENANT_HOSTNAME from env file")
```

### Comparing `armis-1.0.21/tests/test_tagging.py` & `armis-1.0.22/tests/test_tagging.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.21/tests/test_users.py` & `armis-1.0.22/tests/test_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import random
 
 import pytest
 from test_fixture import armis_object
 
 
-@pytest.fixture()
+@pytest.fixture
 def users(armis_object):
     return armis_object.get_users()
 
 
 def test_get_users(users):
     assert len(users) > 0
```

### Comparing `armis-1.0.21/.gitignore` & `armis-1.0.22/.gitignore`

 * *Files identical despite different names*

### Comparing `armis-1.0.21/pyproject.toml` & `armis-1.0.22/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 dynamic = [
     "version",
     "dependencies",
 ]
 description = "Connect and perform actions with the Armis cloud"
 readme = "README.md"
 requires-python = ">=3.8"
-license = "BSD-3-Clause"
+
+
 keywords = ["armis", "api", "development"]
 
 authors = [
   {name = "Matthew Lange", email = "mmlange@gmail.com" }
 ]
 maintainers = [
   {name = "Matthew Lange", email = "mmlange@gmail.com" }
@@ -58,14 +59,15 @@
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-cov",
   "python-dotenv"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest -rExXsP --cov=armis --cov-report html:.coverage_report/html {args:tests}"
+requpdate = "pur -r requirements.txt"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "private*",
@@ -77,32 +79,32 @@
   ".github",
   "mkdocs.yml",
 ]
 
 [publish.index]
 disable = true
 
-[tool.coverage.run]
-source_pkgs = ["armis", "tests"]
-branch = true
-parallel = true
-omit = [
-  "src/armis/__about__.py",
-]
-
-[tool.coverage.paths]
-armis = ["src/armis", "*/armis/src/armis"]
-tests = ["tests", "*/armis/tests"]
-
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+#[tool.coverage.run]
+#source_pkgs = ["armis", "tests"]
+#branch = true
+#parallel = true
+#omit = [
+#  "src/armis/__about__.py",
+#]
+
+#[tool.coverage.paths]
+#armis = ["src/armis", "*/armis/src/armis"]
+#tests = ["tests", "*/armis/tests"]
+
+#[tool.coverage.report]
+#exclude_lines = [
+#  "no cov",
+#  "if __name__ == .__main__.:",
+#  "if TYPE_CHECKING:",
+#]
 
 [tool.ruff]
 exclude = [
   ".bzr",
   ".direnv",
   ".eggs",
   ".git",
@@ -119,15 +121,15 @@
   "buck-out",
   "build",
   "dist",
   "node_modules",
   "venv",
   '__pycache__',
 ]
-target-version = "py311"
+target-version = "py38"
 
 
 [tool.ruff.lint]
 preview = true
 select = [
     "A", # flake8-builtins
     "AIR", # Airflow
@@ -214,7 +216,8 @@
 convention = "numpy"
 
 [tool.ruff.lint.pylint]
 max-locals = 30
 max-public-methods = 30
 max-branches = 15
 max-statements = 100
+
```

