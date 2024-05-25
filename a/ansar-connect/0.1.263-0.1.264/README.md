# Comparing `tmp/ansar_connect-0.1.263.tar.gz` & `tmp/ansar_connect-0.1.264.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.263.tar", last modified: Fri May 24 13:45:32 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.264.tar", last modified: Sat May 25 17:56:27 2024, max compression
```

## Comparing `ansar_connect-0.1.263.tar` & `ansar_connect-0.1.264.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:45:32.133383 ansar_connect-0.1.263/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.263/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-24 13:45:32.133383 ansar_connect-0.1.263/PKG-INFO
--rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.263/README.md
--rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-24 13:44:08.000000 ansar_connect-0.1.263/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-24 13:45:32.133383 ansar_connect-0.1.263/setup.cfg
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-24 13:44:00.000000 ansar_connect-0.1.263/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:45:32.129383 ansar_connect-0.1.263/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:45:32.129383 ansar_connect-0.1.263/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:45:32.129383 ansar_connect-0.1.263/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.263/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.263/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.263/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.263/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:45:32.133383 ansar_connect-0.1.263/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-24 13:45:29.000000 ansar_connect-0.1.263/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.263/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.263/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.263/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.263/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.263/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.263/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.263/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.263/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.263/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9715 2024-05-24 13:42:13.000000 ansar_connect-0.1.263/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.263/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.263/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.263/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42334 2024-05-19 21:19:26.000000 ansar_connect-0.1.263/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.263/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.263/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.263/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.263/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:45:32.133383 ansar_connect-0.1.263/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-24 13:45:32.000000 ansar_connect-0.1.263/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-24 13:45:32.000000 ansar_connect-0.1.263/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-24 13:45:32.000000 ansar_connect-0.1.263/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-24 13:45:32.000000 ansar_connect-0.1.263/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-24 13:45:32.000000 ansar_connect-0.1.263/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-24 13:45:32.000000 ansar_connect-0.1.263/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.264/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/PKG-INFO
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.264/README.md
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-24 13:44:08.000000 ansar_connect-0.1.264/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-24 13:44:00.000000 ansar_connect-0.1.264/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.264/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.264/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.264/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.264/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-25 17:56:24.000000 ansar_connect-0.1.264/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.264/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.264/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.264/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.264/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.264/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.264/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.264/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.264/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.264/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9715 2024-05-24 13:42:13.000000 ansar_connect-0.1.264/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.264/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.264/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.264/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42423 2024-05-25 17:54:22.000000 ansar_connect-0.1.264/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.264/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.264/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.264/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.264/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-25 17:56:27.532913 ansar_connect-0.1.264/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-25 17:56:27.000000 ansar_connect-0.1.264/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.263/LICENSE` & `ansar_connect-0.1.264/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/PKG-INFO` & `ansar_connect-0.1.264/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.263
+Version: 0.1.264
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.263/README.md` & `ansar_connect-0.1.264/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/pyproject.toml` & `ansar_connect-0.1.264/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/setup.py` & `ansar_connect-0.1.264/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.264/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.264/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.264/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.264/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/__init__.py` & `ansar_connect-0.1.264/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 89bdc5b5b108e39418b14f9b6dfde266733c1e0f
-Version: 0.1.262 (2024-05-25@01:45:29+NZST)
+Commit: 8882f193a8d2735e5e8b6a2203b52ca05f800335
+Version: 0.1.263 (2024-05-26@05:56:24+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.263/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.264/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/directory.py` & `ansar_connect-0.1.264/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.264/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.264/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/group_if.py` & `ansar_connect-0.1.264/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/grouping.py` & `ansar_connect-0.1.264/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/moving.py` & `ansar_connect-0.1.264/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/networking.py` & `ansar_connect-0.1.264/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.264/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/node.py` & `ansar_connect-0.1.264/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.264/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/procedure.py` & `ansar_connect-0.1.264/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/product.py` & `ansar_connect-0.1.264/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/socketry.py` & `ansar_connect-0.1.264/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1217,14 +1217,18 @@
 		pass
 
 # A network transport for the purpose of exchanging
 # messages between machines.
 
 def TcpStream_ReceiveBlock(self, stream, s):
 	try:
+		if stream.closing:
+			end_of_session(self, stream, s, 'receive on closing')
+			return
+
 		scrap = s.recv(TCP_RECV)
 		if not scrap:
 			end_of_session(self, stream, s, 'empty socket')
 			return
 
 		try:
 			stream.receive_and_route(scrap, self)
```

### Comparing `ansar_connect-0.1.263/src/ansar/connect/standard.py` & `ansar_connect-0.1.264/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/transporting.py` & `ansar_connect-0.1.264/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.264/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar/connect/wan.py` & `ansar_connect-0.1.264/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.263/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.264/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.263
+Version: 0.1.264
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.263/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.264/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

