# Comparing `tmp/smpclient-2.0.1.tar.gz` & `tmp/smpclient-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpclient-2.0.1.tar", max compression
+gzip compressed data, was "smpclient-3.0.0.tar", max compression
```

## Comparing `smpclient-2.0.1.tar` & `smpclient-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11421 2024-05-21 00:24:58.233728 smpclient-2.0.1/LICENSE
--rw-r--r--   0        0        0     2501 2024-05-21 00:24:58.233728 smpclient-2.0.1/README.md
--rw-r--r--   0        0        0     1822 2024-05-21 00:24:58.257728 smpclient-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     7260 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/__init__.py
--rw-r--r--   0        0        0      188 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/extensions/__init__.py
--rw-r--r--   0        0        0     2473 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/extensions/intercreate.py
--rw-r--r--   0        0        0     2836 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/generics.py
--rw-r--r--   0        0        0     8321 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/mcuboot.py
--rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/py.typed
--rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/__init__.py
--rw-r--r--   0        0        0      860 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/image_management.py
--rw-r--r--   0        0        0     1444 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/os_management.py
--rw-r--r--   0        0        0      494 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/shell_management.py
--rw-r--r--   0        0        0        0 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/user/__init__.py
--rw-r--r--   0        0        0      420 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/requests/user/intercreate.py
--rw-r--r--   0        0        0     2290 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/transport/__init__.py
--rw-r--r--   0        0        0     6845 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/transport/ble.py
--rw-r--r--   0        0        0     9663 2024-05-21 00:24:58.257728 smpclient-2.0.1/smpclient/transport/serial.py
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 smpclient-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11421 2024-05-25 19:36:59.439202 smpclient-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2501 2024-05-25 19:36:59.439202 smpclient-3.0.0/README.md
+-rw-r--r--   0        0        0     1879 2024-05-25 19:36:59.463202 smpclient-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7979 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/extensions/__init__.py
+-rw-r--r--   0        0        0     2473 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/extensions/intercreate.py
+-rw-r--r--   0        0        0     2014 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/generics.py
+-rw-r--r--   0        0        0     8321 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/mcuboot.py
+-rw-r--r--   0        0        0        0 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/py.typed
+-rw-r--r--   0        0        0        0 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/requests/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/requests/image_management.py
+-rw-r--r--   0        0        0     1229 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/requests/os_management.py
+-rw-r--r--   0        0        0      264 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/requests/shell_management.py
+-rw-r--r--   0        0        0        0 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/requests/user/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/requests/user/intercreate.py
+-rw-r--r--   0        0        0     2308 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/transport/__init__.py
+-rw-r--r--   0        0        0     6929 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/transport/ble.py
+-rw-r--r--   0        0        0    10385 2024-05-25 19:36:59.463202 smpclient-3.0.0/smpclient/transport/serial.py
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 smpclient-3.0.0/PKG-INFO
```

### Comparing `smpclient-2.0.1/LICENSE` & `smpclient-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smpclient-2.0.1/README.md` & `smpclient-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smpclient-2.0.1/pyproject.toml` & `smpclient-3.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1, <3.13"
 pyserial = "^3.5"
-smp = "^1.0.1"
+smp = "^1.0.3"
 intelhex = "^2.3.0"
 bleak = "^0.22.1"
+async-timeout = { version = "^4.0.3", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 black = "^23.11.0"
 flake8 = "^6.1.0"
 isort = "^5.12.0"
```

### Comparing `smpclient-2.0.1/smpclient/__init__.py` & `smpclient-3.0.0/smpclient/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 """Simple Management Protocol (SMP) Client."""
 
 from __future__ import annotations
 
+import asyncio
 import logging
 from hashlib import sha256
 from types import TracebackType
 from typing import AsyncIterator, Final, Tuple, Type, cast
 
 from pydantic import ValidationError
 from smp import header as smpheader
 from smp import message as smpmsg
 
 from smpclient.exceptions import SMPBadSequence, SMPUploadError
-from smpclient.generics import SMPRequest, TEr0, TEr1, TErr, TRep, error, flatten_error, success
+from smpclient.generics import SMPRequest, TEr0, TEr1, TRep, error, success
 from smpclient.requests.image_management import ImageUploadWrite
 from smpclient.requests.os_management import MCUMgrParametersRead
 from smpclient.transport import SMPTransport
 
+try:
+    from asyncio import timeout  # type: ignore
+except ImportError:  # backport for Python3.10 and below
+    from async_timeout import timeout  # type: ignore
+
 logger = logging.getLogger(__name__)
 
 
 class SMPClient:
     def __init__(self, transport: SMPTransport, address: str):
         """Create a client to the SMP server `address`, using `transport`."""
         self._transport: Final = transport
         self._address: Final = address
 
-    async def connect(self) -> None:
+    async def connect(self, timeout_s: float = 5.0) -> None:
         """Connect to the SMP server."""
-        await self._transport.connect(self._address)
+        await self._transport.connect(self._address, timeout_s)
         await self._initialize()
 
     async def disconnect(self) -> None:
         """Disconnect from the SMP server."""
         await self._transport.disconnect()
 
-    async def request(self, request: SMPRequest[TRep, TEr0, TEr1, TErr]) -> TRep | TErr:
+    async def request(self, request: SMPRequest[TRep, TEr0, TEr1]) -> TRep | TEr0 | TEr1:
         """Make an `SMPRequest` to the SMP server."""
 
         frame = await self._transport.send_and_receive(request.BYTES)
 
         header = smpheader.Header.loads(frame[: smpheader.Header.SIZE])
 
         if header.sequence != request.header.sequence:  # type: ignore
             raise SMPBadSequence("Bad sequence")
 
         try:
             return request._Response.loads(frame)  # type: ignore
         except ValidationError:
-            return flatten_error(  # type: ignore
-                request._ErrorV0.loads(frame)
-                if header.version == smpheader.Version.V0
-                else request._ErrorV1.loads(frame)
+            pass
+        try:
+            return request._ErrorV0.loads(frame)
+        except ValidationError:
+            pass
+        try:
+            return request._ErrorV1.loads(frame)
+        except ValidationError:
+            error_message = (
+                f"Response could not by parsed as one of {request._Response}, "
+                f"{request._ErrorV0}, or {request._ErrorV1}. {header=} {frame=}"
             )
+            logger.error(error_message)
+            raise ValidationError(error_message)
 
     async def upload(
         self, image: bytes, slot: int = 0, upgrade: bool = False
     ) -> AsyncIterator[int]:
         """Iteratively upload an `image` to `slot`, yielding the offset."""
 
         if self._transport.max_unencoded_size < 23:
@@ -176,15 +191,19 @@
             sha=request.sha,
             upgrade=request.upgrade,
         )
 
     async def _initialize(self) -> None:
         """Gather initialization information from the SMP server."""
 
-        mcumgr_parameters = await self.request(MCUMgrParametersRead())
-        if success(mcumgr_parameters):
-            logger.debug(f"MCUMgr parameters: {mcumgr_parameters}")
-            self._transport.initialize(mcumgr_parameters.buf_size)
-        elif error(mcumgr_parameters):
-            logger.error(f"MCUMgr parameters error: {mcumgr_parameters}")
-        else:
-            raise Exception("Unreachable")
+        try:
+            async with timeout(2):
+                mcumgr_parameters = await self.request(MCUMgrParametersRead())
+                if success(mcumgr_parameters):
+                    logger.debug(f"MCUMgr parameters: {mcumgr_parameters}")
+                    self._transport.initialize(mcumgr_parameters.buf_size)
+                elif error(mcumgr_parameters):
+                    logger.warning(f"Error reading MCUMgr parameters: {mcumgr_parameters}")
+                else:
+                    raise Exception("Unreachable")
+        except asyncio.TimeoutError:
+            logger.warning("Timeout waiting for MCUMgr parameters")
```

### Comparing `smpclient-2.0.1/smpclient/extensions/intercreate.py` & `smpclient-3.0.0/smpclient/extensions/intercreate.py`

 * *Files identical despite different names*

### Comparing `smpclient-2.0.1/smpclient/mcuboot.py` & `smpclient-3.0.0/smpclient/mcuboot.py`

 * *Files identical despite different names*

### Comparing `smpclient-2.0.1/smpclient/transport/__init__.py` & `smpclient-3.0.0/smpclient/transport/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Protocol
 
 
 class SMPTransport(Protocol):
     _smp_server_transport_buffer_size: int | None = None
     """The SMP server transport buffer size, in 8-bit bytes."""
 
-    async def connect(self, address: str) -> None:  # pragma: no cover
+    async def connect(self, address: str, timeout_s: float) -> None:  # pragma: no cover
         """Connect the `SMPTransport`."""
 
     async def disconnect(self) -> None:  # pragma: no cover
         """Disconnect the `SMPTransport`."""
 
     async def send(self, data: bytes) -> None:  # pragma: no cover
         """Send the encoded `SMPRequest` `data`."""
```

### Comparing `smpclient-2.0.1/smpclient/transport/ble.py` & `smpclient-3.0.0/smpclient/transport/ble.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import re
 from typing import Final, List
 from uuid import UUID
 
 from bleak import BleakClient, BleakGATTCharacteristic, BleakScanner
 from bleak.backends.device import BLEDevice
 from smp import header as smphdr
+from typing_extensions import override
 
 from smpclient.exceptions import SMPClientException
 from smpclient.transport import SMPTransport
 
 SMP_SERVICE_UUID: Final = UUID("8D53DC1D-1DB7-4CD3-868B-8A527460AA84")
 SMP_CHARACTERISTIC_UUID: Final = UUID("DA2E7828-FBCE-4E01-AE9E-261174997C48")
 
@@ -43,20 +44,21 @@
 
 class SMPBLETransport(SMPTransport):
     def __init__(self) -> None:
         self._buffer = bytearray()
         self._notify_condition = asyncio.Condition()
         logger.debug(f"Initialized {self.__class__.__name__}")
 
-    async def connect(self, address: str) -> None:
+    @override
+    async def connect(self, address: str, timeout_s: float) -> None:
         logger.debug(f"Scanning for {address=}")
         device: BLEDevice | None = (
-            await BleakScanner.find_device_by_address(address)  # type: ignore # upstream fix
+            await BleakScanner.find_device_by_address(address, timeout=timeout_s)
             if MAC_ADDRESS_PATTERN.match(address) or UUID_PATTERN.match(address)
-            else await BleakScanner.find_device_by_name(address)  # type: ignore # upstream fix
+            else await BleakScanner.find_device_by_name(address)
         )
 
         if type(device) is BLEDevice:
             self._client = BleakClient(device, services=(str(SMP_SERVICE_UUID),))
         else:
             raise SMPBLETransportDeviceNotFound(f"Device '{address}' not found")
 
@@ -86,27 +88,30 @@
 
             self._smp_characteristic = smp_characteristic
 
         logger.debug(f"Starting notify on {SMP_CHARACTERISTIC_UUID=}")
         await self._client.start_notify(SMP_CHARACTERISTIC_UUID, self._notify_callback)
         logger.debug(f"Started notify on {SMP_CHARACTERISTIC_UUID=}")
 
+    @override
     async def disconnect(self) -> None:
         logger.debug(f"Disonnecting from {self._client.address}")
         await self._client.disconnect()
         logger.debug(f"Disconnected from {self._client.address}")
 
+    @override
     async def send(self, data: bytes) -> None:
         logger.debug(f"Sending {len(data)} bytes, {self.mtu=}")
         for offset in range(0, len(data), self.mtu):
             await self._client.write_gatt_char(
                 self._smp_characteristic, data[offset : offset + self.mtu], response=False
             )
         logger.debug(f"Sent {len(data)} bytes")
 
+    @override
     async def receive(self) -> bytes:
         # Note: self._buffer is mutated asynchronously by this method and self._notify_callback().
         #       self._notify_condition is used to synchronize access to self._buffer.
 
         async with self._notify_condition:  # wait for the header
             logger.debug(f"Waiting for notify on {SMP_CHARACTERISTIC_UUID=}")
             await self._notify_condition.wait()
@@ -141,14 +146,15 @@
             self._buffer.extend(data)
             self._notify_condition.notify()
 
     async def send_and_receive(self, data: bytes) -> bytes:
         await self.send(data)
         return await self.receive()
 
+    @override
     @property
     def mtu(self) -> int:
         return self._smp_characteristic.max_write_without_response_size
 
     @staticmethod
     async def scan(timeout: int = 5) -> List[BLEDevice]:
         """Scan for BLE devices."""
```

### Comparing `smpclient-2.0.1/smpclient/transport/serial.py` & `smpclient-3.0.0/smpclient/transport/serial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """A serial SMPTransport."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import math
+import time
 from enum import IntEnum, unique
 from functools import cached_property
 from typing import Final
 
-from serial import Serial
+from serial import Serial, SerialException
 from smp import packet as smppacket
 from typing_extensions import override
 
 from smpclient.transport import SMPTransport
 
 logger = logging.getLogger(__name__)
 
@@ -34,14 +35,15 @@
         return 0
 
     return math.floor(3 / 4 * size) - 2
 
 
 class SMPSerialTransport(SMPTransport):
     _POLLING_INTERVAL_S = 0.005
+    _CONNECTION_RETRY_INTERVAL_S = 0.500
 
     class _ReadBuffer:
         """The state of the read buffer."""
 
         @unique
         class State(IntEnum):
             SMP = 0
@@ -92,25 +94,40 @@
             dsrdtr=dsrdtr,
             inter_byte_timeout=inter_byte_timeout,
             exclusive=exclusive,
         )
         self._buffer = SMPSerialTransport._ReadBuffer()
         logger.debug(f"Initialized {self.__class__.__name__}")
 
-    async def connect(self, address: str) -> None:
+    @override
+    async def connect(self, address: str, timeout_s: float) -> None:
         self._conn.port = address
         logger.debug(f"Connecting to {self._conn.port=}")
-        self._conn.open()
-        logger.debug(f"Connected to {self._conn.port=}")
+        start_time: Final = time.time()
+        while time.time() - start_time <= timeout_s:
+            try:
+                self._conn.open()
+                logger.debug(f"Connected to {self._conn.port=}")
+                return
+            except SerialException as e:
+                logger.debug(
+                    f"Failed to connect to {self._conn.port=}: {e}, "
+                    f"retrying in {SMPSerialTransport._CONNECTION_RETRY_INTERVAL_S} seconds"
+                )
+                await asyncio.sleep(SMPSerialTransport._CONNECTION_RETRY_INTERVAL_S)
 
+        raise TimeoutError(f"Failed to connect to {address=}")
+
+    @override
     async def disconnect(self) -> None:
         logger.debug(f"Disconnecting from {self._conn.port=}")
         self._conn.close()
         logger.debug(f"Disconnected from {self._conn.port=}")
 
+    @override
     async def send(self, data: bytes) -> None:
         logger.debug(f"Sending {len(data)} bytes")
         for packet in smppacket.encode(data, line_length=self.mtu):
             if len(packet) > self.mtu:  # pragma: no cover
                 raise Exception(
                     f"Encoded packet size {len(packet)} exceeds {self.mtu=}, this is a bug!"
                 )
@@ -119,14 +136,15 @@
 
         # fake async until I get around to replacing pyserial
         while self._conn.out_waiting > 0:
             await asyncio.sleep(SMPSerialTransport._POLLING_INTERVAL_S)
 
         logger.debug(f"Sent {len(data)} bytes")
 
+    @override
     async def receive(self) -> bytes:
         decoder = smppacket.decode()
         next(decoder)
 
         logger.debug("Waiting for response")
         while True:
             try:
@@ -227,24 +245,26 @@
                 # it's not necessarily SMP data
                 self._buffer.ser = self._buffer.smp[i_smp_end:]
 
                 self._buffer.state = SMPSerialTransport._ReadBuffer.State.SER
 
                 return out
 
+    @override
     async def send_and_receive(self, data: bytes) -> bytes:
         await self.send(data)
         return await self.receive()
 
+    @override
     @property
     def mtu(self) -> int:
         return self._mtu
 
-    @cached_property
     @override
+    @cached_property
     def max_unencoded_size(self) -> int:
         """The serial transport encodes each packet instead of sending SMP messages as raw bytes.
 
         The worst case size of an encoded SMP packet is:
         ```
         base64_cost(
             len(smp_message) + len(frame_length) + len(frame_crc16)
```

### Comparing `smpclient-2.0.1/PKG-INFO` & `smpclient-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: smpclient
-Version: 2.0.1
+Version: 3.0.0
 Summary: Simple Management Protocol (SMP) Client for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; python_version < "3.11"
 Requires-Dist: bleak (>=0.22.1,<0.23.0)
 Requires-Dist: intelhex (>=2.3.0,<3.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
-Requires-Dist: smp (>=1.0.1,<2.0.0)
+Requires-Dist: smp (>=1.0.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Simple Management Protocol (SMP) Client 
 
 `smpclient` implements the transport layer of the Simple Management Protocol.  This library can be
 used as a dependency in applications that use SMP over **serial (UART or USB)**, **Bluetooth (BLE)**,
 or **UDP** connections.  Some abstractions are provided for common routines like upgrading device
```

