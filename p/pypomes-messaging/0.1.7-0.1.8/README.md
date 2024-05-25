# Comparing `tmp/pypomes_messaging-0.1.7.tar.gz` & `tmp/pypomes_messaging-0.1.8.tar.gz`

## Comparing `pypomes_messaging-0.1.7.tar` & `pypomes_messaging-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/src/pypomes_messaging/__init__.py
--rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/src/pypomes_messaging/mq_publisher.py
--rw-r--r--   0        0        0    21138 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/src/pypomes_messaging/mq_subscriber.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/src/pypomes_messaging/publisher_pomes.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/src/pypomes_messaging/subscriber_pomes.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/README.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/src/pypomes_messaging/__init__.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/src/pypomes_messaging/mq_publisher.py
+-rw-r--r--   0        0        0    21150 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/src/pypomes_messaging/mq_subscriber.py
+-rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/src/pypomes_messaging/publisher_pomes.py
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/src/pypomes_messaging/subscriber_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 pypomes_messaging-0.1.8/PKG-INFO
```

### Comparing `pypomes_messaging-0.1.7/src/pypomes_messaging/__init__.py` & `pypomes_messaging-0.1.8/src/pypomes_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_messaging-0.1.7/src/pypomes_messaging/mq_publisher.py` & `pypomes_messaging-0.1.8/src/pypomes_messaging/mq_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pika
 import pika.frame as pika_frame
 import threading
 from logging import Logger
 from typing import Final
+from pika import SelectConnection
 from pika.channel import Channel
 from pika.connection import Connection
 from pika.exchange_type import ExchangeType
 from pika.spec import BasicProperties
 
 MQP_CONNECTION_OPEN: Final[int] = 1
 MQP_CONNECTION_CLOSED: Final[int] = 2
@@ -67,15 +68,15 @@
         self.msg_last_sent: int = 0
         self.logger: Logger = logger
         self.publish_interval: int = 1
 
         self.reconnect_delay: int = 0
         self.max_reconnect_delay: int = max_reconnect_delay
 
-        self.conn: Connection | None = None
+        self.conn: SelectConnection | None = None
         self.channel: Channel | None = None
 
         self.state: int = MQP_INITIALIZING
         self.state_msg: str = "Attenpting to instantiate the publisher"
 
         # structure ('n' is the sequential message number, int > 0):
         # <{ n: { "header": <str>,
@@ -113,15 +114,15 @@
 
             # initiate the IOLoop, blocking until it is interrupted
             self.conn.ioloop.start()
 
         if self.logger:
             self.logger.info("Finished")
 
-    def connect(self) -> Connection:
+    def connect(self) -> SelectConnection:
         """
         Connect with *RabbitMQ*, and return the connection identifier.
 
         When the connection is established, *on_connection_open* will be invooked by *pika*.
 
         :return: the connection obtained
         """
@@ -130,15 +131,15 @@
             #   url: <protocol>//<user>:<password>@<ip-address>
             first: int = self.mq_url.find("//")
             last = self.mq_url.find("@")
             if self.logger:
                 self.logger.info(f"Connecting with '{self.mq_url[0:first]}{self.mq_url[last:]}'")
 
         # obtain anf return the connection
-        return pika.SelectConnection(
+        return SelectConnection(
             pika.URLParameters(self.mq_url),
             on_open_callback=self.on_connection_open,
             on_open_error_callback=self.on_connection_open_error,
             on_close_callback=self.on_connection_closed)
 
     def on_connection_open(self, _connection: Connection) -> None:
         """
```

### Comparing `pypomes_messaging-0.1.7/src/pypomes_messaging/mq_subscriber.py` & `pypomes_messaging-0.1.8/src/pypomes_messaging/mq_subscriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.consumer_tag: str | None = None
         self.mq_url: str = mq_url
         self.msg_target: callable = msg_target
 
         self.state: int = MQS_INITIALIZING
         self.state_msg: str = "Attenpting to initialize the subscriber"
 
-        self.conn: Connection | None = None
+        self.conn: SelectConnection | None = None
         self.channel: Channel | None = None
         self.queue_name: str = queue_name
 
         # parameter for channel QOS - for higher yield in production, try higher values
         self.prefetch_count: int = 1
 
         if self.logger:
@@ -83,15 +83,15 @@
         Run the consumer, connecting it to *RabbitMQ*.
 
         The *IOLoop* is started, to block and allow the *SelectConnection* to operate.
         """
         self.conn = self.connect()
         self.conn.ioloop.start()
 
-    def connect(self) -> Connection:
+    def connect(self) -> SelectConnection:
         """
         Connect with *RabbitMQ*, returning the connection identifier.
 
         When connection is established, *on_connection_open* will be invoke by *pika*.
 
         :return: the connection obtained
         """
```

### Comparing `pypomes_messaging-0.1.7/src/pypomes_messaging/publisher_pomes.py` & `pypomes_messaging-0.1.8/src/pypomes_messaging/publisher_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         try:
             publisher.start()
         except Exception as e:
             errors.append(f"Error starting the publisher '{badge or __DEFAULT_BADGE}': "
                           f"{exc_format(e, sys.exc_info())}")
 
         # were there errors ?
-        if len(errors) == 0:
+        if not errors:
             # no, wait for the conclusion
             while publisher.get_state() == MQP_INITIALIZING:
                 time.sleep(0.001)
 
             # did connecting with the publisher fail ?
             if publisher.get_state() == MQP_CONNECTION_ERROR:
                 # yes, report the error
```

### Comparing `pypomes_messaging-0.1.7/src/pypomes_messaging/subscriber_pomes.py` & `pypomes_messaging-0.1.8/src/pypomes_messaging/subscriber_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         try:
             subscriber.start()
         except Exception as e:
             errors.append(f"Error starting the subscriber '{badge or __DEFAULT_BADGE}': "
                           f"{exc_format(e, sys.exc_info())}")
 
         # any errors ?
-        if len(errors) == 0:
+        if not errors:
             # no, wait for the conclusion
             while subscriber.consumer.get_state() == MQS_INITIALIZING:
                 time.sleep(0.001)
 
             # did connecting with the subscriber fail ?
             if subscriber.consumer.get_state() == MQS_CONNECTION_ERROR:
                 # yes, report the error
```

### Comparing `pypomes_messaging-0.1.7/LICENSE` & `pypomes_messaging-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_messaging-0.1.7/pyproject.toml` & `pypomes_messaging-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_messaging"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (message handling modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "asn1crypto>=1.5.1",
     "pip>=24.0",
     "pika>=1.3.2",
-    "pypomes_core>=0.7.0",
+    "pypomes_core>=1.0.7",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Messaging"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Messaging/issues"
```

### Comparing `pypomes_messaging-0.1.7/PKG-INFO` & `pypomes_messaging-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.3
 Name: pypomes_messaging
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (message handling modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Messaging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Messaging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: asn1crypto>=1.5.1
 Requires-Dist: pika>=1.3.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.7.0
+Requires-Dist: pypomes-core>=1.0.7
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

