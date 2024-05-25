# Comparing `tmp/adb-tool-py-0.1.1.tar.gz` & `tmp/adb-tool-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb-tool-py-0.1.1.tar", last modified: Sat May 18 15:09:34 2024, max compression
+gzip compressed data, was "adb-tool-py-0.1.2.tar", last modified: Sat May 25 13:25:42 2024, max compression
```

## Comparing `adb-tool-py-0.1.1.tar` & `adb-tool-py-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-18 15:09:34.828373 adb-tool-py-0.1.1/
--rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/LICENSE
--rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/MANIFEST.in
--rw-r--r--   0 iuchi      (501) staff       (20)     1542 2024-05-18 15:09:34.828233 adb-tool-py-0.1.1/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)     1110 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/README.md
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-18 15:09:34.827407 adb-tool-py-0.1.1/adb_tool_py/
--rw-r--r--   0 iuchi      (501) staff       (20)      212 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/__init__.py
--rw-r--r--   0 iuchi      (501) staff       (20)     4502 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/adb_command.py
--rw-r--r--   0 iuchi      (501) staff       (20)      334 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/adb_device.py
--rw-r--r--   0 iuchi      (501) staff       (20)     8684 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/adb_image_cv.py
--rw-r--r--   0 iuchi      (501) staff       (20)    13311 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/adb_tool.py
--rw-r--r--   0 iuchi      (501) staff       (20)     8759 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/adb_view_tree.py
--rw-r--r--   0 iuchi      (501) staff       (20)     1170 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/command.py
--rw-r--r--   0 iuchi      (501) staff       (20)     3544 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/adb_tool_py/ui_node.py
-drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-18 15:09:34.828039 adb-tool-py-0.1.1/adb_tool_py.egg-info/
--rw-r--r--   0 iuchi      (501) staff       (20)     1542 2024-05-18 15:09:34.000000 adb-tool-py-0.1.1/adb_tool_py.egg-info/PKG-INFO
--rw-r--r--   0 iuchi      (501) staff       (20)      416 2024-05-18 15:09:34.000000 adb-tool-py-0.1.1/adb_tool_py.egg-info/SOURCES.txt
--rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-18 15:09:34.000000 adb-tool-py-0.1.1/adb_tool_py.egg-info/dependency_links.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       22 2024-05-18 15:09:34.000000 adb-tool-py-0.1.1/adb_tool_py.egg-info/requires.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-18 15:09:34.000000 adb-tool-py-0.1.1/adb_tool_py.egg-info/top_level.txt
--rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-18 15:09:34.828428 adb-tool-py-0.1.1/setup.cfg
--rw-r--r--   0 iuchi      (501) staff       (20)      872 2024-05-18 15:07:37.000000 adb-tool-py-0.1.1/setup.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-25 13:25:42.016247 adb-tool-py-0.1.2/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1068 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/LICENSE
+-rw-r--r--   0 iuchi      (501) staff       (20)       34 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/MANIFEST.in
+-rw-r--r--   0 iuchi      (501) staff       (20)     1542 2024-05-25 13:25:42.016116 adb-tool-py-0.1.2/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)     1110 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/README.md
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-25 13:25:42.015329 adb-tool-py-0.1.2/adb_tool_py/
+-rw-r--r--   0 iuchi      (501) staff       (20)      212 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/adb_tool_py/__init__.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     5126 2024-05-25 13:16:11.000000 adb-tool-py-0.1.2/adb_tool_py/adb_command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)      334 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/adb_tool_py/adb_device.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     9198 2024-05-25 13:22:15.000000 adb-tool-py-0.1.2/adb_tool_py/adb_image_cv.py
+-rw-r--r--   0 iuchi      (501) staff       (20)    13782 2024-05-25 13:22:24.000000 adb-tool-py-0.1.2/adb_tool_py/adb_tool.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     8759 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/adb_tool_py/adb_view_tree.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     1170 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/adb_tool_py/command.py
+-rw-r--r--   0 iuchi      (501) staff       (20)     3544 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/adb_tool_py/ui_node.py
+drwxr-xr-x   0 iuchi      (501) staff       (20)        0 2024-05-25 13:25:42.015911 adb-tool-py-0.1.2/adb_tool_py.egg-info/
+-rw-r--r--   0 iuchi      (501) staff       (20)     1542 2024-05-25 13:25:41.000000 adb-tool-py-0.1.2/adb_tool_py.egg-info/PKG-INFO
+-rw-r--r--   0 iuchi      (501) staff       (20)      416 2024-05-25 13:25:41.000000 adb-tool-py-0.1.2/adb_tool_py.egg-info/SOURCES.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)        1 2024-05-25 13:25:41.000000 adb-tool-py-0.1.2/adb_tool_py.egg-info/dependency_links.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       22 2024-05-25 13:25:41.000000 adb-tool-py-0.1.2/adb_tool_py.egg-info/requires.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       12 2024-05-25 13:25:41.000000 adb-tool-py-0.1.2/adb_tool_py.egg-info/top_level.txt
+-rw-r--r--   0 iuchi      (501) staff       (20)       38 2024-05-25 13:25:42.016286 adb-tool-py-0.1.2/setup.cfg
+-rw-r--r--   0 iuchi      (501) staff       (20)      872 2024-05-21 09:26:17.000000 adb-tool-py-0.1.2/setup.py
```

### Comparing `adb-tool-py-0.1.1/LICENSE` & `adb-tool-py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.1.1/PKG-INFO` & `adb-tool-py-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-tool-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: adb-tool-py is a tool for Android Debug Bridge (adb).
 Home-page: https://github.com/ShotaIuchi/adb-tool-py
 Author: Shota Iuchi
 Author-email: shotaiuchi.develop@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adb-tool-py-0.1.1/README.md` & `adb-tool-py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.1.1/adb_tool_py/adb_command.py` & `adb-tool-py-0.1.2/adb_tool_py/adb_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,32 @@
 
         :param device: An instance of AdbDevice.
         :return: The current instance of AdbCommand.
         """
         self.device = device
         return self
 
+    def is_connected(self) -> bool:
+        """
+        Checks if the target device is connected.
+
+        :return: True if the device is connected, False otherwise.
+        """
+        result = self.query('devices')
+        lines = result.stdout.splitlines()
+        devices = [line for line in lines if line.strip() and not line.startswith('List of devices attached')]
+        device_id = self.device.serial
+        if device_id is None:
+            return len(devices) == 1
+        else:
+            for device in devices:
+                if device_id in device:
+                    return True
+            return False
+
     def _base_cmd(self) -> list:
         """
         Constructs the base ADB command with the target device.
 
         :return: A list representing the base ADB command.
         """
         if self.device is None or self.device.serial is None:
```

### Comparing `adb-tool-py-0.1.1/adb_tool_py/adb_image_cv.py` & `adb-tool-py-0.1.2/adb_tool_py/adb_image_cv.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,29 @@
         try:
             with open(image_path, 'rb') as f:
                 self.content = f.read()
             self.content_cv = cv2.imdecode(np.frombuffer(self.content, np.uint8), -1)
         except Exception as e:
             raise RuntimeError("Failed to set capture from image path: " + str(e))
 
+    def save_capture(self, image_path: str) -> None:
+        """
+        Saves the current capture to a specified image file path.
+
+        :param image_path: Path to save the image file.
+        """
+        if self.content is None:
+            raise ValueError("Please run the capture method first.")
+
+        try:
+            with open(image_path, 'wb') as f:
+                f.write(self.content)
+        except Exception as e:
+            raise RuntimeError("Failed to save capture to image path: " + str(e))
+
     def check_image(self, image_path: str, index: int = 0, is_capture: bool = False, match_threshold: float = 0.99, merge_threshold: int = 10) -> bool:
         """
         Checks if the specified image is present on the screen.
 
         :param image_path: Path to the image file to search for.
         :param index: Index of the matching image rectangle to use, defaults to 0.
         :param is_capture: Whether to capture the screen before searching, defaults to False.
```

### Comparing `adb-tool-py-0.1.1/adb_tool_py/adb_tool.py` & `adb-tool-py-0.1.2/adb_tool_py/adb_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,22 @@
         """
         self.adb = adb_command
         if adb_command is None:
             self.adb = adb_tool.AdbCommand(adb, adb_tool.AdbDevice(serial))
         self.avt = adb_tool.AdbViewTree(self.adb)
         self.aic = adb_tool.AdbImageCV(self.adb)
 
+    def is_connected(self) -> bool:
+        """
+        Checks if the target device is connected.
+
+        :return: True if the device is connected, False otherwise.
+        """
+        return self.adb.is_connected()
+
     def query(self, cmd: str, stdout=subprocess.PIPE, stderr=subprocess.PIPE) -> subprocess.CompletedProcess:
         """
         Executes an ADB command and waits for it to complete.
 
         :param cmd: The command to execute.
         :param stdout: Standard output pipe, defaults to subprocess.PIPE.
         :param stderr: Standard error pipe, defaults to subprocess.PIPE.
@@ -140,14 +148,22 @@
 
     def capture_screenshot(self) -> None:
         """
         Captures the current screen of the connected Android device.
         """
         self.aic.capture()
 
+    def save_screenshot(self, image_path: str) -> None:
+        """
+        Saves the current screen capture to a specified image file path.
+
+        :param image_path: Path to save the image file.
+        """
+        self.aic.save_capture(image_path)
+
     def content_tree(self) -> ui_node.UINode:
         """
         Returns the root node of the captured UI hierarchy.
 
         :return: The root UINode.
         """
         return self.avt.content_tree
```

### Comparing `adb-tool-py-0.1.1/adb_tool_py/adb_view_tree.py` & `adb-tool-py-0.1.2/adb_tool_py/adb_view_tree.py`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.1.1/adb_tool_py/command.py` & `adb-tool-py-0.1.2/adb_tool_py/command.py`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.1.1/adb_tool_py/ui_node.py` & `adb-tool-py-0.1.2/adb_tool_py/ui_node.py`

 * *Files identical despite different names*

### Comparing `adb-tool-py-0.1.1/adb_tool_py.egg-info/PKG-INFO` & `adb-tool-py-0.1.2/adb_tool_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-tool-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: adb-tool-py is a tool for Android Debug Bridge (adb).
 Home-page: https://github.com/ShotaIuchi/adb-tool-py
 Author: Shota Iuchi
 Author-email: shotaiuchi.develop@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adb-tool-py-0.1.1/setup.py` & `adb-tool-py-0.1.2/setup.py`

 * *Files identical despite different names*

