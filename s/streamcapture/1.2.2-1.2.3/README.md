# Comparing `tmp/streamcapture-1.2.2.tar.gz` & `tmp/streamcapture-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamcapture-1.2.2.tar", last modified: Fri Jan 27 11:24:43 2023, max compression
+gzip compressed data, was "streamcapture-1.2.3.tar", last modified: Sat May 25 14:07:17 2024, max compression
```

## Comparing `streamcapture-1.2.2.tar` & `streamcapture-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2023-01-27 11:24:43.758154 streamcapture-1.2.2/
--rw-r--r--   0 sebastienloisel   (502) staff       (20)     1074 2021-04-01 20:58:02.000000 streamcapture-1.2.2/LICENSE
--rw-r--r--   0 sebastienloisel   (502) staff       (20)     6755 2023-01-27 11:24:43.757895 streamcapture-1.2.2/PKG-INFO
--rw-r--r--   0 sebastienloisel   (502) staff       (20)     6231 2023-01-27 11:24:43.000000 streamcapture-1.2.2/README.md
--rw-r--r--   0 sebastienloisel   (502) staff       (20)       38 2023-01-27 11:24:43.758242 streamcapture-1.2.2/setup.cfg
--rw-r--r--   0 sebastienloisel   (502) staff       (20)      913 2023-01-27 11:24:34.000000 streamcapture-1.2.2/setup.py
-drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2023-01-27 11:24:43.752198 streamcapture-1.2.2/streamcapture/
--rw-r--r--   0 sebastienloisel   (502) staff       (20)     9310 2023-01-27 11:24:23.000000 streamcapture-1.2.2/streamcapture/__init__.py
-drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2023-01-27 11:24:43.754774 streamcapture-1.2.2/streamcapture.egg-info/
--rw-r--r--   0 sebastienloisel   (502) staff       (20)     6755 2023-01-27 11:24:43.000000 streamcapture-1.2.2/streamcapture.egg-info/PKG-INFO
--rw-r--r--   0 sebastienloisel   (502) staff       (20)      300 2023-01-27 11:24:43.000000 streamcapture-1.2.2/streamcapture.egg-info/SOURCES.txt
--rw-r--r--   0 sebastienloisel   (502) staff       (20)        1 2023-01-27 11:24:43.000000 streamcapture-1.2.2/streamcapture.egg-info/dependency_links.txt
--rw-r--r--   0 sebastienloisel   (502) staff       (20)        1 2021-03-25 19:13:52.000000 streamcapture-1.2.2/streamcapture.egg-info/not-zip-safe
--rw-r--r--   0 sebastienloisel   (502) staff       (20)       22 2023-01-27 11:24:43.000000 streamcapture-1.2.2/streamcapture.egg-info/requires.txt
--rw-r--r--   0 sebastienloisel   (502) staff       (20)       14 2023-01-27 11:24:43.000000 streamcapture-1.2.2/streamcapture.egg-info/top_level.txt
-drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2023-01-27 11:24:43.756297 streamcapture-1.2.2/test/
--rw-r--r--   0 sebastienloisel   (502) staff       (20)      389 2021-04-25 22:35:53.000000 streamcapture-1.2.2/test/test1.py
--rw-r--r--   0 sebastienloisel   (502) staff       (20)      269 2021-03-26 00:00:22.000000 streamcapture-1.2.2/test/test2.py
+drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2024-05-25 14:07:17.872031 streamcapture-1.2.3/
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)     1074 2021-04-01 20:58:02.000000 streamcapture-1.2.3/LICENSE
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)     6807 2024-05-25 14:07:17.871567 streamcapture-1.2.3/PKG-INFO
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)     6231 2024-05-25 14:07:17.000000 streamcapture-1.2.3/README.md
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)       38 2024-05-25 14:07:17.872127 streamcapture-1.2.3/setup.cfg
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      913 2023-02-13 16:04:06.000000 streamcapture-1.2.3/setup.py
+drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2024-05-25 14:07:17.865144 streamcapture-1.2.3/streamcapture/
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)     9356 2024-05-25 13:57:43.000000 streamcapture-1.2.3/streamcapture/__init__.py
+drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2024-05-25 14:07:17.871034 streamcapture-1.2.3/streamcapture.egg-info/
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)     6807 2024-05-25 14:07:17.000000 streamcapture-1.2.3/streamcapture.egg-info/PKG-INFO
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      397 2024-05-25 14:07:17.000000 streamcapture-1.2.3/streamcapture.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)        1 2024-05-25 14:07:17.000000 streamcapture-1.2.3/streamcapture.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)        1 2024-05-25 13:44:50.000000 streamcapture-1.2.3/streamcapture.egg-info/not-zip-safe
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)       22 2024-05-25 14:07:17.000000 streamcapture-1.2.3/streamcapture.egg-info/requires.txt
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)       14 2024-05-25 14:07:17.000000 streamcapture-1.2.3/streamcapture.egg-info/top_level.txt
+drwxr-xr-x   0 sebastienloisel   (502) staff       (20)        0 2024-05-25 14:07:17.870669 streamcapture-1.2.3/test/
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      389 2021-04-25 22:35:53.000000 streamcapture-1.2.3/test/test1.py
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      269 2021-03-26 00:00:22.000000 streamcapture-1.2.3/test/test2.py
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      429 2024-05-25 13:57:43.000000 streamcapture-1.2.3/test/test3.repeating.py
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      233 2024-05-25 13:57:43.000000 streamcapture-1.2.3/test/test4.fast_open_close.py
+-rw-r--r--   0 sebastienloisel   (502) staff       (20)      329 2024-05-25 13:57:43.000000 streamcapture-1.2.3/test/test5.multi_capture_to_same_buffer.py
```

### Comparing `streamcapture-1.2.2/LICENSE` & `streamcapture-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamcapture-1.2.2/PKG-INFO` & `streamcapture-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: streamcapture
-Version: 1.2.2
+Version: 1.2.3
 Summary: Capture output streams such as sys.stdout and sys.stderr.
 Home-page: https://github.com/sloisel/streamcapture
 Author: Sébastien Loisel
 Author-email: sloisel@gmail.com
 License: MIT
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/sloisel/streamcapture/blob/master/streamcapture.html
 Project-URL: Source, https://github.com/sloisel/streamcapture
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: pdoc3>=0.7
 
 
 ## streamcapture: capture the outputs of Python streams, such as sys.stdout and sys.stderr
 
 ### Author: Sébastien Loisel
 
 # Installation
```

### Comparing `streamcapture-1.2.2/README.md` & `streamcapture-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `streamcapture-1.2.2/setup.py` & `streamcapture-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent.absolute()
 long_description = Path(this_directory, 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='streamcapture',
     description='Capture output streams such as sys.stdout and sys.stderr.',
-    version='1.2.2',
+    version='1.2.3',
     packages=find_packages(),
     install_requires=['setuptools', 'pdoc3>=0.7'],
     python_requires='>=3',
     author='Sébastien Loisel',
     author_email='sloisel@gmail.com',
     zip_safe=False,
     url='https://github.com/sloisel/streamcapture',
```

### Comparing `streamcapture-1.2.2/streamcapture/__init__.py` & `streamcapture-1.2.3/streamcapture/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,35 +154,39 @@
 	def printer(self):
 		"""This is the thread that listens to the pipe output and passes it to the writer stream."""
 		try:
 			looping = True
 			while looping:
 				data = os.read(self.pipe_read_fd,100000)
 				foo = data.split(self.magic)
-				data = foo[0]
+
 				if len(foo)>=2:
 					looping = False
-				if len(data)==0:
-					break
-				self.write(data)
-				if self.echo:
-					os.write(self.dup_fd,data)
+
+				for segment in foo:
+					if len(segment) == 0:
+						# Pipe is closed
+						looping = False
+						break
+					self.write(segment)
+					if self.echo:
+						os.write(self.dup_fd,segment)
 		finally:
-			self.writer.close()
-			os.close(self.dup_fd)
 			os.close(self.pipe_read_fd)
 	def close(self):
 		"""When you want to "uncapture" a stream, use this method."""
 		if not self.active:
 			return
 		self.active = False
 		os.write(self.fd,self.magic)
+		self.thread.join()
 		os.dup2(self.dup_fd,self.fd)
 		os.close(self.pipe_write_fd)
-		self.thread.join()
+		os.close(self.dup_fd)
+
 	def __enter__(self):
 		return self
 	def __exit__(self,a,b,c):
 		self.close()
 
 class StreamCapture:
 	def __init__(self,stream,writer,echo=True,monkeypatch=None):
```

### Comparing `streamcapture-1.2.2/streamcapture.egg-info/PKG-INFO` & `streamcapture-1.2.3/streamcapture.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: streamcapture
-Version: 1.2.2
+Version: 1.2.3
 Summary: Capture output streams such as sys.stdout and sys.stderr.
 Home-page: https://github.com/sloisel/streamcapture
 Author: Sébastien Loisel
 Author-email: sloisel@gmail.com
 License: MIT
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/sloisel/streamcapture/blob/master/streamcapture.html
 Project-URL: Source, https://github.com/sloisel/streamcapture
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: pdoc3>=0.7
 
 
 ## streamcapture: capture the outputs of Python streams, such as sys.stdout and sys.stderr
 
 ### Author: Sébastien Loisel
 
 # Installation
```

