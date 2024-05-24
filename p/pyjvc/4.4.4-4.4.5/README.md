# Comparing `tmp/pyjvc-4.4.4.tar.gz` & `tmp/pyjvc-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvc-4.4.4.tar", last modified: Fri Apr 19 14:59:38 2024, max compression
+gzip compressed data, was "pyjvc-4.4.5.tar", last modified: Sat Apr 27 18:21:41 2024, max compression
```

## Comparing `pyjvc-4.4.4.tar` & `pyjvc-4.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.801500 pyjvc-4.4.4/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.4/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-19 14:59:38.801312 pyjvc-4.4.4/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.4/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.798757 pyjvc-4.4.4/jvc_projector/
--rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.4/jvc_projector/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)    10329 2024-04-19 14:59:00.000000 pyjvc-4.4.4/jvc_projector/command_runner.py
--rw-r--r--   0 ilan       (501) staff       (20)    10031 2024-04-08 21:43:07.000000 pyjvc-4.4.4/jvc_projector/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      250 2024-04-08 21:43:07.000000 pyjvc-4.4.4/jvc_projector/error_classes.py
--rw-r--r--   0 ilan       (501) staff       (20)    18249 2024-04-19 14:50:45.000000 pyjvc-4.4.4/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.801109 pyjvc-4.4.4/pyJVC.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 14:59:38.801542 pyjvc-4.4.4/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-19 14:59:34.000000 pyjvc-4.4.4/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.800769 pyjvc-4.4.4/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.4/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.4/tests/test_commander.py
--rw-r--r--   0 ilan       (501) staff       (20)     8923 2024-04-08 21:43:07.000000 pyjvc-4.4.4/tests/test_coordinator.py
--rw-r--r--   0 ilan       (501) staff       (20)    20373 2024-04-08 21:43:07.000000 pyjvc-4.4.4/tests/test_loop.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-27 18:21:41.838794 pyjvc-4.4.5/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.5/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-27 18:21:41.838578 pyjvc-4.4.5/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.5/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-27 18:21:41.836027 pyjvc-4.4.5/jvc_projector/
+-rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.5/jvc_projector/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10460 2024-04-27 18:05:18.000000 pyjvc-4.4.5/jvc_projector/command_runner.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10065 2024-04-27 18:09:10.000000 pyjvc-4.4.5/jvc_projector/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      250 2024-04-08 21:43:07.000000 pyjvc-4.4.5/jvc_projector/error_classes.py
+-rw-r--r--   0 ilan       (501) staff       (20)    18957 2024-04-27 18:16:51.000000 pyjvc-4.4.5/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-27 18:21:41.838362 pyjvc-4.4.5/pyJVC.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-27 18:21:41.000000 pyjvc-4.4.5/pyJVC.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-27 18:21:41.000000 pyjvc-4.4.5/pyJVC.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-27 18:21:41.000000 pyjvc-4.4.5/pyJVC.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-27 18:21:41.000000 pyjvc-4.4.5/pyJVC.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-27 18:21:41.838833 pyjvc-4.4.5/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-27 18:21:14.000000 pyjvc-4.4.5/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-27 18:21:41.838023 pyjvc-4.4.5/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.5/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.5/tests/test_commander.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8923 2024-04-08 21:43:07.000000 pyjvc-4.4.5/tests/test_coordinator.py
+-rw-r--r--   0 ilan       (501) staff       (20)    20373 2024-04-08 21:43:07.000000 pyjvc-4.4.5/tests/test_loop.py
```

### Comparing `pyjvc-4.4.4/LICENSE` & `pyjvc-4.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.4/PKG-INFO` & `pyjvc-4.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.4
+Version: 4.4.5
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.4/README.md` & `pyjvc-4.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.4/jvc_projector/command_runner.py` & `pyjvc-4.4.5/jvc_projector/command_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
                 data = await asyncio.wait_for(self.reader.read(1024), timeout=0.5)
                 if not data:
                     # If no data is received, the buffer is empty
                     break
             except asyncio.TimeoutError:
                 # If a timeout occurs, assume the buffer is empty and break the loop
                 break
-            except BrokenPipeError:
+            except BrokenPipeError as err:
                 # If a broken pipe error occurs, the connection is closed
-                raise ConnectionClosedError("Broken pipe")
+                raise ConnectionClosedError(err)
             except Exception as e:
                 # Handle any other exceptions that may occur during reading
                 self.logger.error("Error while clearing read buffer: %s", e)
                 break
 
     async def _do_command(
         self,
@@ -192,14 +192,17 @@
                     return msg, True
 
                 # have to read again to get the value
                 ref_msg = await self.reader.read(1000)
                 self.logger.debug("received ref_msg in _do_command: %s", ref_msg)
                 # msg = await self._check_received_msg(received_ack, ack_value, command_type)
                 self.logger.debug("finished reading ref_msg")
+               
+                # JVC seems to have a buffer bug with a lot of commands
+                await self.read_until_empty()
                 return ref_msg.replace(ack_value, b"")
 
             except socket.timeout as err:
                 error = f"Timed out. Command {final_cmd} may grayed out or cmd is running already."
                 self.logger.debug(err)
                 raise CommandTimeoutError(error) from err
```

### Comparing `pyjvc-4.4.4/jvc_projector/commands.py` & `pyjvc-4.4.5/jvc_projector/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,15 +397,15 @@
     power = b"PW", PowerModes, ACKs.power_ack
     power_status = b"PW", PowerModes, ACKs.power_ack
     # lens memory /installation mode commands
     installation_mode = b"INML", InstallationModes, ACKs.lens_ack
 
     # input commands
     input_mode = b"IP", InputModes, ACKs.input_ack
-
+    null = b"\x00\x00", None, None
     # status commands - Reference: ?
     # These should not be used directly
 
     current_output = b"IP"
     info = b"RC7374"
     remote = b"RC73"
```

### Comparing `pyjvc-4.4.4/jvc_projector/jvc_projector.py` & `pyjvc-4.4.5/jvc_projector/jvc_projector.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     LowLatencyModes,
     PowerStates,
     model_map,
 )
 from jvc_projector.error_classes import (
     CommandTimeoutError,
     ConnectionClosedError,
-    ShouldReconnectError,
 )
 
 
 @dataclass
 class JVCInput:
     """JVC Projector Input"""
 
@@ -165,17 +164,17 @@
             if not self.connection_open:
                 await self.open_connection()
 
             # clear the buffer
             await self.commander.read_until_empty()
 
             return
-        except ConnectionClosedError as e:
-            self.logger.error("Error resetting everything: %s", e)
-            raise
+        except ConnectionClosedError:
+            # set the connnection to closed
+            await self.close_connection()
         except Exception as e:
             self.logger.error("Error resetting everything: %s", e)
             return
 
     async def open_connection(self) -> bool:
         """Open a connection to the projector asynchronously"""
         # If the connection is already open, return True
@@ -258,16 +257,18 @@
                     return res
                 # this means stuff is actually broken
                 except (
                     ConnectionClosedError,
                     ConnectionRefusedError,
                     BrokenPipeError,
                 ) as err:
-                    self.logger.debug("Connection closed. Retry your command")
-                    raise ShouldReconnectError(err) from err
+                    self.logger.debug("exec command - %s", err)
+                    await self.close_connection()
+                    # should reconnect
+                    return None
                 # getting here means the command is not allowed
                 except CommandTimeoutError:
                     self.logger.debug(
                         "Command timed out. Very likely its not allowed to run (This is not a bug. JVC's fault)"
                     )
                     return None
             self.logger.error("Command failed after 3 retries")
@@ -278,18 +279,23 @@
         try:
             if self.writer:
                 self.writer.close()
                 await self.writer.wait_closed()
 
             self.logger.info("Connection closed")
         except BrokenPipeError:
-            self.logger.warning("Connection already closed - Broken pipe encountered")
+            self.logger.debug(
+                "Connection already closed - Broken pipe encountered. Moving on"
+            )
         except Exception as e:
-            self.logger.error("Error closing JVC Projector connection - %s", e)
+            self.logger.debug("Error closing JVC Projector connection - %s", e)
         finally:
+            self.logger.debug("Resetting connection values")
+            self.reader = None
+            self.writer = None
             self.commander.reader = self.reader
             self.commander.writer = self.writer
             self.connection_open = False
             self.attributes.connection_active = False
 
     async def power_on(
         self,
@@ -333,14 +339,28 @@
             except ValueError as err:
                 self.logger.error("Attribute not found - %s", err)
                 raise
             except AttributeError as err:
                 self.logger.error("tried to access name on non-enum: %s", err)
                 return ""
 
+    async def run_null_command(self) -> bool:
+        """
+        Run a null command to test the connection
+        """
+        async with self.lock:
+            # send a null command
+            self.writer.write(b"\x21\x89\x01\x00\x00\x0A")
+            await self.writer.drain()
+            # read the response
+            res = await self.reader.read(1000)
+            self.logger.debug("Null command response: %s", res)
+            # 0x06 0x89 0x01 0x00 0x00 0x0A
+            return res == b"\x06\x89\x01\x00\x00\x0A"
+        
     async def get_low_latency_state(self) -> str:
         """
         Get the current state of LL
         """
         return await self._get_attribute("low_latency")
 
     async def get_picture_mode(self) -> str:
```

### Comparing `pyjvc-4.4.4/pyJVC.egg-info/PKG-INFO` & `pyjvc-4.4.5/pyJVC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.4
+Version: 4.4.5
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.4/setup.py` & `pyjvc-4.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyjvc",
-    version="4.4.4",
+    version="4.4.5",
     author="iloveicedgreentea2",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pyjvc-4.4.4/tests/test_commander.py` & `pyjvc-4.4.5/tests/test_commander.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.4/tests/test_coordinator.py` & `pyjvc-4.4.5/tests/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.4/tests/test_loop.py` & `pyjvc-4.4.5/tests/test_loop.py`

 * *Files identical despite different names*

