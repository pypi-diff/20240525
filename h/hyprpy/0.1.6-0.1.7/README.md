# Comparing `tmp/hyprpy-0.1.6.tar.gz` & `tmp/hyprpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprpy-0.1.6.tar", last modified: Sat May 11 11:58:40 2024, max compression
+gzip compressed data, was "hyprpy-0.1.7.tar", last modified: Sat May 25 12:10:45 2024, max compression
```

## Comparing `hyprpy-0.1.6.tar` & `hyprpy-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.294684 hyprpy-0.1.6/
--rw-r--r--   0 ulinja    (1000) users      (100)     1064 2023-08-14 03:22:15.000000 hyprpy-0.1.6/LICENSE
--rw-r--r--   0 ulinja    (1000) users      (100)     3410 2024-05-11 11:58:40.294684 hyprpy-0.1.6/PKG-INFO
--rw-r--r--   0 ulinja    (1000) users      (100)     2223 2024-05-11 11:55:20.000000 hyprpy-0.1.6/README.md
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.287684 hyprpy-0.1.6/hyprpy/
--rw-r--r--   0 ulinja    (1000) users      (100)      194 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/__init__.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.290684 hyprpy-0.1.6/hyprpy/components/
--rw-r--r--   0 ulinja    (1000) users      (100)    10332 2023-09-13 15:23:33.000000 hyprpy-0.1.6/hyprpy/components/__init__.py
--rw-r--r--   0 ulinja    (1000) users      (100)      434 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/components/common.py
--rw-r--r--   0 ulinja    (1000) users      (100)    11810 2024-05-11 11:35:10.000000 hyprpy-0.1.6/hyprpy/components/instances.py
--rw-r--r--   0 ulinja    (1000) users      (100)     2594 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/components/monitors.py
--rw-r--r--   0 ulinja    (1000) users      (100)     3478 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/components/windows.py
--rw-r--r--   0 ulinja    (1000) users      (100)     2410 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/components/workspaces.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.291684 hyprpy-0.1.6/hyprpy/data/
--rw-r--r--   0 ulinja    (1000) users      (100)     3092 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/data/__init__.py
--rw-r--r--   0 ulinja    (1000) users      (100)     5230 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/data/models.py
--rw-r--r--   0 ulinja    (1000) users      (100)      647 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/data/validators.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.293684 hyprpy-0.1.6/hyprpy/utils/
--rw-r--r--   0 ulinja    (1000) users      (100)        0 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/utils/__init__.py
--rw-r--r--   0 ulinja    (1000) users      (100)     4411 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/utils/assertions.py
--rw-r--r--   0 ulinja    (1000) users      (100)     2868 2023-08-14 16:23:04.000000 hyprpy-0.1.6/hyprpy/utils/shell.py
--rw-r--r--   0 ulinja    (1000) users      (100)     4090 2023-08-14 05:03:40.000000 hyprpy-0.1.6/hyprpy/utils/signals.py
--rw-r--r--   0 ulinja    (1000) users      (100)     9202 2023-08-15 17:45:43.000000 hyprpy-0.1.6/hyprpy/utils/sockets.py
-drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-11 11:58:40.293684 hyprpy-0.1.6/hyprpy.egg-info/
--rw-r--r--   0 ulinja    (1000) users      (100)     3410 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/PKG-INFO
--rw-r--r--   0 ulinja    (1000) users      (100)      584 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/SOURCES.txt
--rw-r--r--   0 ulinja    (1000) users      (100)        1 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/dependency_links.txt
--rw-r--r--   0 ulinja    (1000) users      (100)       16 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/requires.txt
--rw-r--r--   0 ulinja    (1000) users      (100)        7 2024-05-11 11:58:40.000000 hyprpy-0.1.6/hyprpy.egg-info/top_level.txt
--rw-r--r--   0 ulinja    (1000) users      (100)       81 2023-08-14 05:03:40.000000 hyprpy-0.1.6/pyproject.toml
--rw-r--r--   0 ulinja    (1000) users      (100)     1177 2024-05-11 11:58:40.295684 hyprpy-0.1.6/setup.cfg
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-25 12:10:45.509379 hyprpy-0.1.7/
+-rw-r--r--   0 ulinja    (1000) users      (100)     1064 2023-08-14 03:22:15.000000 hyprpy-0.1.7/LICENSE
+-rw-r--r--   0 ulinja    (1000) users      (100)     3410 2024-05-25 12:10:45.509379 hyprpy-0.1.7/PKG-INFO
+-rw-r--r--   0 ulinja    (1000) users      (100)     2223 2024-05-25 11:26:00.000000 hyprpy-0.1.7/README.md
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-25 12:10:45.499379 hyprpy-0.1.7/hyprpy/
+-rw-r--r--   0 ulinja    (1000) users      (100)      194 2023-08-14 05:03:40.000000 hyprpy-0.1.7/hyprpy/__init__.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-25 12:10:45.504378 hyprpy-0.1.7/hyprpy/components/
+-rw-r--r--   0 ulinja    (1000) users      (100)    10332 2023-09-13 15:23:33.000000 hyprpy-0.1.7/hyprpy/components/__init__.py
+-rw-r--r--   0 ulinja    (1000) users      (100)      434 2023-08-14 05:03:40.000000 hyprpy-0.1.7/hyprpy/components/common.py
+-rw-r--r--   0 ulinja    (1000) users      (100)    11810 2024-05-25 11:26:00.000000 hyprpy-0.1.7/hyprpy/components/instances.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     2594 2023-08-15 17:45:43.000000 hyprpy-0.1.7/hyprpy/components/monitors.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     3478 2023-08-15 17:45:43.000000 hyprpy-0.1.7/hyprpy/components/windows.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     2410 2023-08-15 17:45:43.000000 hyprpy-0.1.7/hyprpy/components/workspaces.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-25 12:10:45.506379 hyprpy-0.1.7/hyprpy/data/
+-rw-r--r--   0 ulinja    (1000) users      (100)     3092 2023-08-14 05:03:40.000000 hyprpy-0.1.7/hyprpy/data/__init__.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     5230 2023-08-15 17:45:43.000000 hyprpy-0.1.7/hyprpy/data/models.py
+-rw-r--r--   0 ulinja    (1000) users      (100)      647 2023-08-14 05:03:40.000000 hyprpy-0.1.7/hyprpy/data/validators.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-25 12:10:45.508378 hyprpy-0.1.7/hyprpy/utils/
+-rw-r--r--   0 ulinja    (1000) users      (100)        0 2023-08-14 05:03:40.000000 hyprpy-0.1.7/hyprpy/utils/__init__.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     4411 2023-08-15 17:45:43.000000 hyprpy-0.1.7/hyprpy/utils/assertions.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     2868 2023-08-14 16:23:04.000000 hyprpy-0.1.7/hyprpy/utils/shell.py
+-rw-r--r--   0 ulinja    (1000) users      (100)     4090 2024-05-25 11:25:05.000000 hyprpy-0.1.7/hyprpy/utils/signals.py
+-rw-r--r--   0 ulinja    (1000) users      (100)    10888 2024-05-25 12:02:57.000000 hyprpy-0.1.7/hyprpy/utils/sockets.py
+drwxr-xr-x   0 ulinja    (1000) users      (100)        0 2024-05-25 12:10:45.509379 hyprpy-0.1.7/hyprpy.egg-info/
+-rw-r--r--   0 ulinja    (1000) users      (100)     3410 2024-05-25 12:10:45.000000 hyprpy-0.1.7/hyprpy.egg-info/PKG-INFO
+-rw-r--r--   0 ulinja    (1000) users      (100)      584 2024-05-25 12:10:45.000000 hyprpy-0.1.7/hyprpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)        1 2024-05-25 12:10:45.000000 hyprpy-0.1.7/hyprpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)       16 2024-05-25 12:10:45.000000 hyprpy-0.1.7/hyprpy.egg-info/requires.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)        7 2024-05-25 12:10:45.000000 hyprpy-0.1.7/hyprpy.egg-info/top_level.txt
+-rw-r--r--   0 ulinja    (1000) users      (100)       81 2023-08-14 05:03:40.000000 hyprpy-0.1.7/pyproject.toml
+-rw-r--r--   0 ulinja    (1000) users      (100)     1177 2024-05-25 12:10:45.510378 hyprpy-0.1.7/setup.cfg
```

### Comparing `hyprpy-0.1.6/LICENSE` & `hyprpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/PKG-INFO` & `hyprpy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python bindings for the Hyprland compositor.
 Author: Julian Lobbes
 Author-email: julian@lobbes.dev
 Project-URL: repo, https://github.com/ulinja/hyprpy
 Project-URL: docs, https://hyprpy.lobbes.dev/
 Keywords: hyprland,wayland,compositor,window manager
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyprpy-0.1.6/README.md` & `hyprpy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/components/__init__.py` & `hyprpy-0.1.7/hyprpy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/components/instances.py` & `hyprpy-0.1.7/hyprpy/components/instances.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/components/monitors.py` & `hyprpy-0.1.7/hyprpy/components/monitors.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/components/windows.py` & `hyprpy-0.1.7/hyprpy/components/windows.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/components/workspaces.py` & `hyprpy-0.1.7/hyprpy/components/workspaces.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/data/__init__.py` & `hyprpy-0.1.7/hyprpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/data/models.py` & `hyprpy-0.1.7/hyprpy/data/models.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/data/validators.py` & `hyprpy-0.1.7/hyprpy/data/validators.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/utils/assertions.py` & `hyprpy-0.1.7/hyprpy/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/utils/shell.py` & `hyprpy-0.1.7/hyprpy/utils/shell.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/utils/signals.py` & `hyprpy-0.1.7/hyprpy/utils/signals.py`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/hyprpy/utils/sockets.py` & `hyprpy-0.1.7/hyprpy/utils/sockets.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,19 @@
     instance.event_socket.close()
 
     # Send a command
     instance.command_socket.send_command("dispatch", flags=["--single-instance"], args=["exec", "kitty"])
 """
 
 from abc import ABC
-from typing import List
+from os import getenv
 from pathlib import PosixPath
-import select, socket
+from typing import List
 import logging
+import select, socket
 
 from hyprpy.utils import assertions
 
 
 log = logging.getLogger(__name__)
 
 
@@ -50,27 +51,58 @@
 
     Provides attributes and methods common between :class:`~EventSocket`
     and :class:`~CommandSocket`.
 
     Upon initialization, the underlying :class:`~socket.socket` object is *not* created.
     Users must explicitly call :meth:`~AbstractSocket.connect` prior
     to using the :class:`~socket.socket`, and should call :meth:`~AbstractSocket.close`
-    aftwerwards.
+    afterwards.
     """
 
     def __init__(self, signature: str):
         assertions.assert_is_nonempty_string(signature)
         #: The Hyprland Instance Signature.
         self._signature: str = signature
         #: Filesystem path to the socket file.
         self._path_to_socket: PosixPath
         #: The underlying :class:`socket.socket` object.
         self._socket: socket.socket | None = None
 
 
+    @staticmethod
+    def _find_socket_base_directory() -> PosixPath:
+        """Finds the filesystem directory where the Hyprland socket files are located.
+
+        On older versions of Hyprland (pre v0.40.0), the base directory for socket files is located
+        at `/tmp/hypr/`, while newer versions place it at `$XDG_RUNTIME_DIR/hypr/`.
+        This method attempts to find the socket base directory for newer versions, falling back to
+        the legacy path, and raising an Error if neither can be located.
+
+        :return: Path to an existing base directory for Hyprland socket files.
+        :raises: :class:`RuntimeError` if the `/tmp/hypr` directory does not exist and `$XDG_RUNTIME_DIR`
+            is undefined.
+        :raises: :class:`FileNotFoundError` if neither `/tmp/hypr` nor `$XDG_RUNTIME_DIR/hypr` exist.
+        """
+
+        runtime_dir = getenv("XDG_RUNTIME_DIR", None)
+        base_dir_legacy = PosixPath("/tmp/hypr")
+        base_dir_newer = PosixPath(runtime_dir) / "hypr" if runtime_dir else None
+
+        if base_dir_newer and base_dir_newer.is_dir():
+            return base_dir_newer
+        if base_dir_legacy.is_dir():
+            return base_dir_legacy
+        if not base_dir_newer:
+            raise RuntimeError(
+                f"Failed to locate Hyprland socket base path: '{base_dir_legacy}' does not exist and " \
+                f"'$XDG_RUNTIME_DIR' is undefined!"
+            )
+        raise FileNotFoundError(f"Failed to locate Hyprland socket base path at '{base_dir_legacy}' or '{base_dir_newer}'.")
+
+
     def connect(self, timeout: int | float | None = 1) -> None:
         """Creates and connects the :class:`~socket.socket`.
 
         If a ``timeout`` is set, its value specifies the number of seconds to wait until
         the connection is established. If the connection cannot be established within the
         specified ``timeout`` period, a :class:`SocketError` is raised. The default
         ``timeout`` is 1 second.
@@ -135,14 +167,15 @@
         if not self._socket:
             raise SocketError("Attempted to wait for data on a socket which was not connected.")
 
         read_ready, _, _ = select.select([self._socket], [], [], timeout)
         if not read_ready:
             raise SocketError(f"Waiting socket timed out after {timeout} seconds.")
 
+
     def read(self) -> str:
         """Immediately retrieves all data from the :class:`~socket.socket` and returns it.
 
         :return: The data received from the :class:`~socket.socket` as a string. If the socket
             does not contain any data, returns an empty string.
         :raises: :class:`~SocketError` if the :class:`~socket.socket` is not connected.
         """
@@ -172,29 +205,33 @@
 
     This socket broadcasts events about the ongoing Hyprland session, such as
     windows or workspaces being created or destroyed.
     """
 
     def __init__(self, signature: str):
         super().__init__(signature)
-        self._path_to_socket = PosixPath(f"/tmp/hypr/{self._signature}/.socket2.sock")
+
+        socket_base_dir = self._find_socket_base_directory()
+        self._path_to_socket = socket_base_dir /self._signature / ".socket2.sock"
         if not self._path_to_socket.is_socket():
             raise FileNotFoundError(f"No socket found at {self._path_to_socket!r}.")
 
 
 class CommandSocket(AbstractSocket):
     """Interface to Hyprland's command socket.
 
     Provides the :meth:`CommandSocket.send_command` method, which can be used to send
     a wide range of commands, as explained in `the Hyprland wiki <https://wiki.hyprland.org/Configuring/Using-hyprctl>`_.
     """
 
     def __init__(self, signature: str):
         super().__init__(signature)
-        self._path_to_socket = PosixPath(f"/tmp/hypr/{self._signature}/.socket.sock")
+
+        socket_base_dir = self._find_socket_base_directory()
+        self._path_to_socket = socket_base_dir / self._signature / ".socket.sock"
         if not self._path_to_socket.is_socket():
             raise FileNotFoundError(f"No socket found at {self._path_to_socket!r}.")
 
 
     def send_command(self, command: str, flags: List[str] = [], args: List[str] = []) -> str:
         """Sends a command through the socket and returns the received response.
```

### Comparing `hyprpy-0.1.6/hyprpy.egg-info/PKG-INFO` & `hyprpy-0.1.7/hyprpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python bindings for the Hyprland compositor.
 Author: Julian Lobbes
 Author-email: julian@lobbes.dev
 Project-URL: repo, https://github.com/ulinja/hyprpy
 Project-URL: docs, https://hyprpy.lobbes.dev/
 Keywords: hyprland,wayland,compositor,window manager
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyprpy-0.1.6/hyprpy.egg-info/SOURCES.txt` & `hyprpy-0.1.7/hyprpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyprpy-0.1.6/setup.cfg` & `hyprpy-0.1.7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hyprpy
-version = 0.1.6
+version = 0.1.7
 description = Python bindings for the Hyprland compositor.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Julian Lobbes
 author_email = julian@lobbes.dev
 project_urls = 
 	repo = https://github.com/ulinja/hyprpy
```

