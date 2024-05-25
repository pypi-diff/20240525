# Comparing `tmp/testcontainers-4.4.1.tar.gz` & `tmp/testcontainers-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.4.1.tar", max compression
+gzip compressed data, was "testcontainers-4.5.0.tar", max compression
```

## Comparing `testcontainers-4.4.1.tar` & `testcontainers-4.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11328 2024-05-14 07:49:02.803210 testcontainers-4.4.1/LICENSE.txt
--rw-r--r--   0        0        0     2042 2024-05-14 07:49:02.803210 testcontainers-4.4.1/README.md
--rw-r--r--   0        0        0      172 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13096 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0     2433 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     8875 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     6926 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-05-14 07:49:02.803210 testcontainers-4.4.1/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2591 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      978 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     1543 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/network.py
--rw-r--r--   0        0        0     2088 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4069 2024-05-14 07:49:02.807210 testcontainers-4.4.1/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3781 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     2492 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/cassandra/testcontainers/cassandra/__init__.py
--rw-r--r--   0        0        0     2736 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/chroma/testcontainers/chroma/__init__.py
--rw-r--r--   0        0        0     3030 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0      106 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2709 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/google/testcontainers/google/datastore.py
--rw-r--r--   0        0        0     2952 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3760 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3592 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2727 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/kafka/testcontainers/kafka/_redpanda.py
--rw-r--r--   0        0        0     4249 2024-05-14 07:49:02.807210 testcontainers-4.4.1/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     2042 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/memcached/testcontainers/memcached/__init__.py
--rw-r--r--   0        0        0     4116 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3017 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     2202 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     4984 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2811 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/nats/testcontainers/nats/__init__.py
--rw-r--r--   0        0        0     2782 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4109 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     2960 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/oracle-free/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     3984 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     5209 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/qdrant/testcontainers/qdrant/__init__.py
--rw-r--r--   0        0        0     2967 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-05-14 07:49:02.811210 testcontainers-4.4.1/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2761 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/registry/testcontainers/registry/__init__.py
--rw-r--r--   0        0        0     4272 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     1432 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/selenium/testcontainers/selenium/video.py
--rw-r--r--   0        0        0     2519 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/vault/testcontainers/vault/__init__.py
--rw-r--r--   0        0        0     5588 2024-05-14 07:49:02.815210 testcontainers-4.4.1/modules/weaviate/testcontainers/weaviate/__init__.py
--rw-r--r--   0        0        0     8834 2024-05-14 07:49:02.815210 testcontainers-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 testcontainers-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-05-25 19:37:09.791271 testcontainers-4.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-05-25 19:37:09.791271 testcontainers-4.5.0/README.md
+-rw-r--r--   0        0        0      172 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13448 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0     3157 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     8877 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     7503 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2591 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      979 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     1543 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/network.py
+-rw-r--r--   0        0        0     3108 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4069 2024-05-25 19:37:09.791271 testcontainers-4.5.0/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3781 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-05-25 19:37:09.791271 testcontainers-4.5.0/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3760 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     4249 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     2042 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/memcached/testcontainers/memcached/__init__.py
+-rw-r--r--   0        0        0     4116 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3017 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     4984 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2782 2024-05-25 19:37:09.795271 testcontainers-4.5.0/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4109 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2960 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3984 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5209 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2967 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     4272 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     1432 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/selenium/testcontainers/selenium/video.py
+-rw-r--r--   0        0        0     2519 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/vault/testcontainers/vault/__init__.py
+-rw-r--r--   0        0        0     5589 2024-05-25 19:37:09.799271 testcontainers-4.5.0/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8834 2024-05-25 19:37:09.803271 testcontainers-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 testcontainers-4.5.0/PKG-INFO
```

### Comparing `testcontainers-4.4.1/LICENSE.txt` & `testcontainers-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/README.md` & `testcontainers-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/core/testcontainers/compose/compose.py` & `testcontainers-4.5.0/core/testcontainers/compose/compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from dataclasses import dataclass, field, fields
+from dataclasses import asdict, dataclass, field, fields
 from functools import cached_property
 from json import loads
 from os import PathLike
+from platform import system
 from re import split
 from subprocess import CompletedProcess
 from subprocess import run as subprocess_run
 from typing import Callable, Literal, Optional, TypeVar, Union
 from urllib.error import HTTPError, URLError
 from urllib.request import urlopen
 
@@ -34,14 +35,22 @@
     """
 
     URL: Optional[str] = None
     TargetPort: Optional[str] = None
     PublishedPort: Optional[str] = None
     Protocol: Optional[str] = None
 
+    def normalize(self):
+        url_not_usable = system() == "Windows" and self.URL == "0.0.0.0"
+        if url_not_usable:
+            self_dict = asdict(self)
+            self_dict.update({"URL": "127.0.0.1"})
+            return PublishedPort(**self_dict)
+        return self
+
 
 OT = TypeVar("OT")
 
 
 def get_only_element_or_raise(array: list[OT], exception: Callable[[], Exception]) -> OT:
     if len(array) != 1:
         e = exception()
@@ -353,15 +362,15 @@
             The internal port to get the mapping for
 
         Returns
         -------
         str:
             The mapped port on the host
         """
-        return self.get_container(service_name).get_publisher(by_port=port).PublishedPort
+        return self.get_container(service_name).get_publisher(by_port=port).normalize().PublishedPort
 
     def get_service_host(
         self,
         service_name: Optional[str] = None,
         port: Optional[int] = None,
     ):
         """
@@ -375,22 +384,22 @@
             The internal port to get the host for
 
         Returns
         -------
         str:
             The hostname for the service
         """
-        return self.get_container(service_name).get_publisher(by_port=port).URL
+        return self.get_container(service_name).get_publisher(by_port=port).normalize().URL
 
     def get_service_host_and_port(
         self,
         service_name: Optional[str] = None,
         port: Optional[int] = None,
     ):
-        publisher = self.get_container(service_name).get_publisher(by_port=port)
+        publisher = self.get_container(service_name).get_publisher(by_port=port).normalize()
         return publisher.URL, publisher.PublishedPort
 
     @wait_container_is_ready(HTTPError, URLError)
     def wait_for(self, url: str) -> "DockerCompose":
         """
         Waits for a response from a given URL. This is typically used to block until a service in
         the environment has started and is responding. Note that it does not assert any sort of
```

### Comparing `testcontainers-4.4.1/core/testcontainers/core/config.py` & `testcontainers-4.5.0/core/testcontainers/core/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass, field
+from logging import warning
 from os import environ
 from os.path import exists
 from pathlib import Path
+from typing import Optional, Union
 
 MAX_TRIES = int(environ.get("TC_MAX_TRIES", 120))
 SLEEP_TIME = int(environ.get("TC_POOLING_INTERVAL", 1))
 TIMEOUT = MAX_TRIES * SLEEP_TIME
 
 RYUK_IMAGE: str = environ.get("RYUK_CONTAINER_IMAGE", "testcontainers/ryuk:0.7.0")
 RYUK_PRIVILEGED: bool = environ.get("TESTCONTAINERS_RYUK_PRIVILEGED", "false") == "true"
@@ -32,26 +34,42 @@
     for file in tc_files:
         with open(file) as contents:
             tuples = [line.split("=") for line in contents.readlines() if "=" in line]
             settings = {**settings, **{item[0].strip(): item[1].strip() for item in tuples}}
     return settings
 
 
+_WARNINGS = {"DOCKER_AUTH_CONFIG": "DOCKER_AUTH_CONFIG is experimental, see testcontainers/testcontainers-python#566"}
+
+
 @dataclass
 class TestcontainersConfiguration:
     max_tries: int = MAX_TRIES
     sleep_time: int = SLEEP_TIME
     ryuk_image: str = RYUK_IMAGE
     ryuk_privileged: bool = RYUK_PRIVILEGED
     ryuk_disabled: bool = RYUK_DISABLED
     ryuk_docker_socket: str = RYUK_DOCKER_SOCKET
     ryuk_reconnection_timeout: str = RYUK_RECONNECTION_TIMEOUT
     tc_properties: dict[str, str] = field(default_factory=read_tc_properties)
+    _docker_auth_config: Optional[str] = field(default_factory=lambda: environ.get("DOCKER_AUTH_CONFIG"))
+
+    @property
+    def docker_auth_config(self):
+        if "DOCKER_AUTH_CONFIG" in _WARNINGS:
+            warning(_WARNINGS.pop("DOCKER_AUTH_CONFIG"))
+        return self._docker_auth_config
+
+    @docker_auth_config.setter
+    def docker_auth_config(self, value: str):
+        if "DOCKER_AUTH_CONFIG" in _WARNINGS:
+            warning(_WARNINGS.pop("DOCKER_AUTH_CONFIG"))
+        self._docker_auth_config = value
 
-    def tc_properties_get_tc_host(self):
+    def tc_properties_get_tc_host(self) -> Union[str, None]:
         return self.tc_properties.get("tc.host")
 
     @property
     def timeout(self):
         return self.max_tries * self.sleep_time
```

### Comparing `testcontainers-4.4.1/core/testcontainers/core/container.py` & `testcontainers-4.5.0/core/testcontainers/core/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         return self._docker
 
     def get_logs(self) -> tuple[bytes, bytes]:
         if not self._container:
             raise ContainerStartException("Container should be started before getting logs")
         return self._container.logs(stderr=False), self._container.logs(stdout=False)
 
-    def exec(self, command) -> tuple[int, str]:
+    def exec(self, command) -> tuple[int, bytes]:
         if not self._container:
             raise ContainerStartException("Container should be started before executing a command")
         return self._container.exec_run(command)
 
     def _configure(self) -> None:
         # placeholder if subclasses want to define this and use the default start method
         pass
```

### Comparing `testcontainers-4.4.1/core/testcontainers/core/docker_client.py` & `testcontainers-4.5.0/core/testcontainers/core/docker_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import docker
 from docker.models.containers import Container, ContainerCollection
 from typing_extensions import ParamSpec
 
 from testcontainers.core.config import testcontainers_config as c
 from testcontainers.core.labels import SESSION_ID, create_labels
-from testcontainers.core.utils import default_gateway_ip, inside_container, setup_logger
+from testcontainers.core.utils import default_gateway_ip, inside_container, parse_docker_auth_config, setup_logger
 
 LOGGER = setup_logger(__name__)
 
 _P = ParamSpec("_P")
 _T = TypeVar("_T")
 
 
@@ -53,14 +53,17 @@
             os.environ["DOCKER_HOST"] = docker_host
             self.client = docker.from_env(**kwargs)
         else:
             self.client = docker.from_env(**kwargs)
         self.client.api.headers["x-tc-sid"] = SESSION_ID
         self.client.api.headers["User-Agent"] = "tc-python/" + importlib.metadata.version("testcontainers")
 
+        if docker_auth_config := get_docker_auth_config():
+            self.login(docker_auth_config)
+
     @_wrapped_container_collection
     def run(
         self,
         image: str,
         command: Optional[Union[str, list[str]]] = None,
         environment: Optional[dict] = None,
         ports: Optional[dict] = None,
@@ -179,10 +182,22 @@
             return url.hostname
         if inside_container() and ("unix" in url.scheme or "npipe" in url.scheme):
             ip_address = default_gateway_ip()
             if ip_address:
                 return ip_address
         return "localhost"
 
+    def login(self, docker_auth_config: str) -> None:
+        """
+        Login to a docker registry using the given auth config.
+        """
+        auth_config = parse_docker_auth_config(docker_auth_config)[0]  # Only using the first auth config
+        login_info = self.client.login(**auth_config._asdict())
+        LOGGER.debug(f"logged in using {login_info}")
+
 
 def get_docker_host() -> Optional[str]:
     return c.tc_properties_get_tc_host() or os.getenv("DOCKER_HOST")
+
+
+def get_docker_auth_config() -> Optional[str]:
+    return c.docker_auth_config
```

### Comparing `testcontainers-4.4.1/core/testcontainers/core/exceptions.py` & `testcontainers-4.5.0/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/core/testcontainers/core/generic.py` & `testcontainers-4.5.0/core/testcontainers/core/generic.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/core/testcontainers/core/labels.py` & `testcontainers-4.5.0/core/testcontainers/core/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def create_labels(image: str, labels: Optional[dict[str, str]]) -> dict[str, str]:
     if labels is None:
         labels = {}
     else:
         for k in labels:
             if k.startswith(TESTCONTAINERS_NAMESPACE):
-                raise ValueError("The org.testcontainers namespace is reserved for interal use")
+                raise ValueError("The org.testcontainers namespace is reserved for internal use")
 
     labels[LABEL_LANG] = "python"
     labels[LABEL_TESTCONTAINERS] = "true"
     labels[LABEL_VERSION] = importlib.metadata.version("testcontainers")
 
     if image == c.ryuk_image:
         return labels
```

### Comparing `testcontainers-4.4.1/core/testcontainers/core/network.py` & `testcontainers-4.5.0/core/testcontainers/core/network.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/core/testcontainers/core/utils.py` & `testcontainers-4.5.0/core/testcontainers/core/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import base64
+import json
 import logging
 import os
 import platform
 import subprocess
 import sys
+from collections import namedtuple
 
 LINUX = "linux"
 MAC = "mac"
 WIN = "win"
 
+DockerAuthInfo = namedtuple("DockerAuthInfo", ["registry", "username", "password"])
+
 
 def setup_logger(name: str) -> logging.Logger:
     logger = logging.getLogger(name)
     logger.setLevel(logging.INFO)
     handler = logging.StreamHandler()
     handler.setLevel(logging.INFO)
     logger.addHandler(handler)
@@ -73,7 +78,33 @@
 def raise_for_deprecated_parameter(kwargs: dict, name: str, replacement: str) -> dict:
     """
     Raise an error if a dictionary of keyword arguments contains a key and suggest the replacement.
     """
     if kwargs.pop(name, None):
         raise ValueError(f"Use `{replacement}` instead of `{name}`")
     return kwargs
+
+
+def parse_docker_auth_config(auth_config: str) -> list[DockerAuthInfo]:
+    """
+    Parse the docker auth config from a string.
+
+    Example:
+    {
+        "auths": {
+            "https://index.docker.io/v1/": {
+                "auth": "dXNlcm5hbWU6cGFzc3dvcmQ="
+            }
+        }
+    }
+    """
+    auth_info: list[DockerAuthInfo] = []
+    try:
+        auth_config_dict: dict = json.loads(auth_config).get("auths")
+        for registry, auth in auth_config_dict.items():
+            auth_str = auth.get("auth")
+            auth_str = base64.b64decode(auth_str).decode("utf-8")
+            username, password = auth_str.split(":")
+            auth_info.append(DockerAuthInfo(registry, username, password))
+        return auth_info
+    except (json.JSONDecodeError, KeyError, ValueError) as exp:
+        raise ValueError("Could not parse docker auth config") from exp
```

### Comparing `testcontainers-4.4.1/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.5.0/core/testcontainers/core/waiting_utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.5.0/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.5.0/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/cassandra/testcontainers/cassandra/__init__.py` & `testcontainers-4.5.0/modules/cassandra/testcontainers/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/chroma/testcontainers/chroma/__init__.py` & `testcontainers-4.5.0/modules/chroma/testcontainers/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.5.0/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.5.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/google/testcontainers/google/datastore.py` & `testcontainers-4.5.0/modules/google/testcontainers/google/datastore.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.5.0/modules/google/testcontainers/google/pubsub.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.5.0/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.5.0/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.5.0/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/kafka/testcontainers/kafka/_redpanda.py` & `testcontainers-4.5.0/modules/kafka/testcontainers/kafka/_redpanda.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.5.0/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.5.0/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/memcached/testcontainers/memcached/__init__.py` & `testcontainers-4.5.0/modules/memcached/testcontainers/memcached/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.5.0/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.5.0/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/mssql/testcontainers/mssql/__init__.py` & `testcontainers-4.5.0/modules/mssql/testcontainers/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/mysql/testcontainers/mysql/__init__.py` & `testcontainers-4.5.0/modules/mysql/testcontainers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/nats/testcontainers/nats/__init__.py` & `testcontainers-4.5.0/modules/nats/testcontainers/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.5.0/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.5.0/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.5.0/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/oracle-free/testcontainers/oracle/__init__.py` & `testcontainers-4.5.0/modules/oracle-free/testcontainers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.5.0/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/qdrant/testcontainers/qdrant/__init__.py` & `testcontainers-4.5.0/modules/qdrant/testcontainers/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.5.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.5.0/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/registry/testcontainers/registry/__init__.py` & `testcontainers-4.5.0/modules/registry/testcontainers/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.5.0/modules/selenium/testcontainers/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/selenium/testcontainers/selenium/video.py` & `testcontainers-4.5.0/modules/selenium/testcontainers/selenium/video.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/vault/testcontainers/vault/__init__.py` & `testcontainers-4.5.0/modules/vault/testcontainers/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.4.1/modules/weaviate/testcontainers/weaviate/__init__.py` & `testcontainers-4.5.0/modules/weaviate/testcontainers/weaviate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     Arguments:
         `image`
             Docker image to use with Weaviate container.
         `env_vars`
             Additional environment variables to include with the container, e.g. ENABLE_MODULES list, QUERY_DEFAULTS_LIMIT setting.
 
     Example:
-        This example shows how to start Weaviate container with defualt settings.
+        This example shows how to start Weaviate container with default settings.
 
         .. doctest::
 
             >>> from testcontainers.weaviate import WeaviateContainer
 
             >>> with WeaviateContainer() as container:
             ...     with container.get_client() as client:
             ...         client.is_live()
             True
 
-        This example shows how to start Weaviate container with additinal settings.
+        This example shows how to start Weaviate container with additional settings.
 
         .. doctest::
 
             >>> from testcontainers.weaviate import WeaviateContainer
 
             >>> with WeaviateContainer(
             ...     env_vars={
```

### Comparing `testcontainers-4.4.1/pyproject.toml` & `testcontainers-4.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.4.1"  # auto-incremented by release-please
+version = "4.5.0"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
     "David Ankin <daveankin@gmail.com>",
     "Vemund Santi <vemund@santi.no>"
 ]
```

### Comparing `testcontainers-4.4.1/PKG-INFO` & `testcontainers-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.4.1
+Version: 4.5.0
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

