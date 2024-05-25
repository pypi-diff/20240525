# Comparing `tmp/weallcode_robot-3.0.3.tar.gz` & `tmp/weallcode_robot-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weallcode_robot-3.0.3.tar", max compression
+gzip compressed data, was "weallcode_robot-3.1.0.tar", max compression
```

## Comparing `weallcode_robot-3.0.3.tar` & `weallcode_robot-3.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2351 2024-03-01 23:02:25.969975 weallcode_robot-3.0.3/README.md
--rw-r--r--   0        0        0     1332 2024-03-01 23:02:25.969975 weallcode_robot-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      168 2024-03-01 23:02:25.969975 weallcode_robot-3.0.3/weallcode_robot/__init__.py
--rw-r--r--   0        0        0     7000 2024-03-01 23:02:25.969975 weallcode_robot-3.0.3/weallcode_robot/commands.py
--rw-r--r--   0        0        0     3401 2024-03-01 23:02:25.969975 weallcode_robot-3.0.3/weallcode_robot/robot.py
--rw-r--r--   0        0        0     4948 2024-03-01 23:02:25.973975 weallcode_robot-3.0.3/weallcode_robot/robot_ui.py
--rw-r--r--   0        0        0      511 2024-03-01 23:02:25.973975 weallcode_robot-3.0.3/weallcode_robot/robotapp.py
--rw-r--r--   0        0        0     2614 2024-03-01 23:02:25.973975 weallcode_robot-3.0.3/weallcode_robot/utils.py
--rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 weallcode_robot-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2386 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/README.md
+-rw-r--r--   0        0        0     1332 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/weallcode_robot/__init__.py
+-rw-r--r--   0        0        0     7000 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/weallcode_robot/commands.py
+-rw-r--r--   0        0        0     3379 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/weallcode_robot/robot.py
+-rw-r--r--   0        0        0     5046 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/weallcode_robot/robot_ui.py
+-rw-r--r--   0        0        0      511 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/weallcode_robot/robotapp.py
+-rw-r--r--   0        0        0     2614 2024-05-25 12:08:54.559150 weallcode_robot-3.1.0/weallcode_robot/utils.py
+-rw-r--r--   0        0        0     3499 1970-01-01 00:00:00.000000 weallcode_robot-3.1.0/PKG-INFO
```

### Comparing `weallcode_robot-3.0.3/README.md` & `weallcode_robot-3.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,32 +32,32 @@
 robot.move(0, 0)            # Stop the robot
 robot.move(-100, -100)      # Move backward
 robot.wait(1)               # Wait for 1 second
 robot.move(0, 0)            # Stop the robot
 
 robot.led(0, 0, 0)          # Turn off the LED
 
-a = robot.set_key_binding('a').led(0, 0, 255, 1) # set LED color one button A
-w = robot.set_key_binding('w').move(100, 100)    # bind move forward to key W
+a = robot.setKeyBinding('a').led(0, 0, 255, 1) # set LED color one button A
+w = robot.setKeyBinding('w').move(100, 100)    # bind move forward to key W
 ```
 
 ## API
 
 ### Robot
 
 The `Robot` class is the main class to control the robot. Instantiate the class with the name of the robot.
 
 ```python
 robot = Robot("WAC")
 ```
 
 #### Methods
 
-- `led(r: int, g: int, b: int)`: Sets the LED color. Values should be integers between 0 and 255.
-- `move(right: int, left: int)`: Sets the motor speeds. Values should be integers between -100 and 100.
+- `led(red: int, green: int, blue: int, duration: int)`: Sets the LED color. Values should be integers between 0 and 255.
+- `move(left: int, right: int, duration: int)`: Sets the motor speeds. Values should be integers between -100 and 100.
 - `wait(duration: float)`: Adds a wait command with a given duration in seconds.
 - `run()`: Executes the commands in the order they were added.
 
 ## Development
 
 The package includes development dependencies:
```

### Comparing `weallcode_robot-3.0.3/pyproject.toml` & `weallcode_robot-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "weallcode_robot"
-version = "3.0.3"
+version = "3.1.0"
 description = "Micro:bit TinyBit BLE Python Library"
 license = "MIT"
 authors = [
     "Blaine Rothrock <blaine.p.rothrock@gmail.com>",
     "Ali Karbassi <ali@weallcode.org>",
 ]
 readme = "README.md"
@@ -34,15 +34,15 @@
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-bleak = "^0.20.1"
+bleak = "^0.22.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.1"
 isort = "^5.12.0"
 ruff = "^0.0.260"
 textual = "^0.52.1"
```

### Comparing `weallcode_robot-3.0.3/weallcode_robot/commands.py` & `weallcode_robot-3.1.0/weallcode_robot/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return self.queue.empty()
     
     def led(self, red, green, blue, duration: float = 0):
         self.put(LEDCommand(red, green, blue))
         self.wait(duration)
         return self
 
-    def move(self, right, left, duration: float = 0):
+    def move(self, left, right, duration: float = 0):
         self.put(MoveCommand(left, right))
         self.wait(duration)
         return self
 
     def stop(self, duration: float = 0):
         self.put(MoveCommand(0, 0))
         self.wait(duration)
```

### Comparing `weallcode_robot-3.0.3/weallcode_robot/robot.py` & `weallcode_robot-3.1.0/weallcode_robot/robot.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,39 +53,39 @@
         self.wait = self.main_queue.wait
         self.displayText = self.main_queue.displayText
         self.displayDots = self.main_queue.displayDots
         self.clearDisplay = self.main_queue.clearDisplay
         self.buzz = self.main_queue.buzz
         self.clear = self.main_queue.clear
 
-        self.button_a = DynamicObject()
-        self.button_a.led = self.button_a_queue.led
-        self.button_a.move = self.button_a_queue.move
-        self.button_a.stop = self.button_a_queue.stop
-        self.button_a.wait = self.button_a_queue.wait
-        self.button_a.displayText = self.button_a_queue.displayText
-        self.button_a.displayDots = self.button_a_queue.displayDots
-        self.button_a.clearDisplay = self.button_a_queue.clearDisplay
-        self.button_a.buzz = self.button_a_queue.buzz
-        self.button_a.clear = self.button_a_queue.clear
+        self.buttonA = DynamicObject()
+        self.buttonA.led = self.button_a_queue.led
+        self.buttonA.move = self.button_a_queue.move
+        self.buttonA.stop = self.button_a_queue.stop
+        self.buttonA.wait = self.button_a_queue.wait
+        self.buttonA.displayText = self.button_a_queue.displayText
+        self.buttonA.displayDots = self.button_a_queue.displayDots
+        self.buttonA.clearDisplay = self.button_a_queue.clearDisplay
+        self.buttonA.buzz = self.button_a_queue.buzz
+        self.buttonA.clear = self.button_a_queue.clear
 
-        self.button_b = DynamicObject()
-        self.button_b.led = self.button_b_queue.led
-        self.button_b.move = self.button_b_queue.move
-        self.button_b.stop = self.button_b_queue.stop
-        self.button_b.wait = self.button_b_queue.wait
-        self.button_b.displayText = self.button_b_queue.displayText
-        self.button_b.displayDots = self.button_b_queue.displayDots
-        self.button_b.clearDisplay = self.button_b_queue.clearDisplay
-        self.button_b.buzz = self.button_b_queue.buzz
-        self.button_b.clear = self.button_b_queue.clear
+        self.buttonB = DynamicObject()
+        self.buttonB.led = self.button_b_queue.led
+        self.buttonB.move = self.button_b_queue.move
+        self.buttonB.stop = self.button_b_queue.stop
+        self.buttonB.wait = self.button_b_queue.wait
+        self.buttonB.displayText = self.button_b_queue.displayText
+        self.buttonB.displayDots = self.button_b_queue.displayDots
+        self.buttonB.clearDisplay = self.button_b_queue.clearDisplay
+        self.buttonB.buzz = self.button_b_queue.buzz
+        self.buttonB.clear = self.button_b_queue.clear
         
         atexit.register(self.ui.run)
     
-    def set_key_binding(self, key) -> CommandQueue:
+    def setKeyBinding(self, key) -> CommandQueue:
         valid_keys = {
             'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm',
             'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
             '1', '2', '3', '4', '5', '6', '7', '8', '9', '0', 'space', 'enter',
             'up', 'down', 'left', 'right'
         }
```

### Comparing `weallcode_robot-3.0.3/weallcode_robot/robot_ui.py` & `weallcode_robot-3.1.0/weallcode_robot/robot_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,24 +77,18 @@
         self.query_one(RobotStatus).status = status
 
     def bind(self, key) -> CommandQueue:
         self.key_commands[key] = CommandQueue(f'{self.robot.display_name}-{key}')
         return self.key_commands[key]
 
     async def _connect_and_run(self):
-        scanner = BleakScanner()
         self.update_status(f'scanning for {self.robot.display_name} ...')
-        devices = await scanner.discover(timeout=2.0, return_adv=False)
+        device = await BleakScanner.find_device_by_name(self.robot.name, timeout=10.0)
 
         self.update_status(f'connecting to {self.robot.display_name} ...')
-        device = None
-        for d in devices:
-            if d.name is not None and d.name.lower() == self.robot.name:
-                device = d
-                break
 
         if device is None:
             self.update_status(f"device {self.robot.name} not found. Quit and try again.")
             return
 
         self.update_status(f"found device {device.name} at {device.address}")
         logging.debug(f"found device {device.name} at {device.address}")
@@ -125,25 +119,31 @@
 
         self.update_status('running ...')
 
         commands = copy.deepcopy(self.robot.commands).clear().clearDisplay()
 
         await self.execute(commands)
 
+        if self.robot.button_a_queue.empty() and self.robot.button_b_queue.empty() and not self.key_commands:
+            self.exit()
+
     async def execute(self, commands):     
         if self.running == 1: return
 
         self.running = 1
         while commands.empty() is False:
             command = await commands.get()
             # self.update_status(f"executing {command.__class__.__name__} ...")
             await command.execute(self.client)
 
-        self.update_status('idle')
-        self.running = 0
+        if not self.key_commands and self.robot.button_a_queue.empty() and self.robot.button_b_queue.empty():
+            return
+        else:
+            self.update_status('idle')
+            self.running = 0
 
     async def clear(self):
         self.running = 1
 
         commands = CommandQueue(f'{self.robot.display_name}-{key}').clear().clearDisplay()
         while commands.empty() is False:
             command = await commands.get()
```

### Comparing `weallcode_robot-3.0.3/weallcode_robot/utils.py` & `weallcode_robot-3.1.0/weallcode_robot/utils.py`

 * *Files identical despite different names*

### Comparing `weallcode_robot-3.0.3/PKG-INFO` & `weallcode_robot-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weallcode_robot
-Version: 3.0.3
+Version: 3.1.0
 Summary: Micro:bit TinyBit BLE Python Library
 Home-page: https://github.com/WeAllCode/tinybit-python
 License: MIT
 Author: Blaine Rothrock
 Author-email: blaine.p.rothrock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: bleak (>=0.20.1,<0.21.0)
+Requires-Dist: bleak (>=0.22.1,<0.23.0)
 Project-URL: Repository, https://github.com/WeAllCode/tinybit-python
 Description-Content-Type: text/markdown
 
 # Micro:bit TinyBit BLE Python Library
 
 A Python package to control a custom Robot V2 via Bluetooth Low Energy (BLE) communication. The package provides an API for controlling the robot's movements and LED colors.
 
@@ -59,32 +59,32 @@
 robot.move(0, 0)            # Stop the robot
 robot.move(-100, -100)      # Move backward
 robot.wait(1)               # Wait for 1 second
 robot.move(0, 0)            # Stop the robot
 
 robot.led(0, 0, 0)          # Turn off the LED
 
-a = robot.set_key_binding('a').led(0, 0, 255, 1) # set LED color one button A
-w = robot.set_key_binding('w').move(100, 100)    # bind move forward to key W
+a = robot.setKeyBinding('a').led(0, 0, 255, 1) # set LED color one button A
+w = robot.setKeyBinding('w').move(100, 100)    # bind move forward to key W
 ```
 
 ## API
 
 ### Robot
 
 The `Robot` class is the main class to control the robot. Instantiate the class with the name of the robot.
 
 ```python
 robot = Robot("WAC")
 ```
 
 #### Methods
 
-- `led(r: int, g: int, b: int)`: Sets the LED color. Values should be integers between 0 and 255.
-- `move(right: int, left: int)`: Sets the motor speeds. Values should be integers between -100 and 100.
+- `led(red: int, green: int, blue: int, duration: int)`: Sets the LED color. Values should be integers between 0 and 255.
+- `move(left: int, right: int, duration: int)`: Sets the motor speeds. Values should be integers between -100 and 100.
 - `wait(duration: float)`: Adds a wait command with a given duration in seconds.
 - `run()`: Executes the commands in the order they were added.
 
 ## Development
 
 The package includes development dependencies:
```

