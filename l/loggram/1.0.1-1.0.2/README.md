# Comparing `tmp/loggram-1.0.1.tar.gz` & `tmp/loggram-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggram-1.0.1.tar", last modified: Fri May 17 08:59:56 2024, max compression
+gzip compressed data, was "loggram-1.0.2.tar", last modified: Sat May 25 10:08:52 2024, max compression
```

## Comparing `loggram-1.0.1.tar` & `loggram-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 08:59:56.551856 loggram-1.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-02-22 08:02:12.000000 loggram-1.0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2767 2024-05-17 08:59:56.551856 loggram-1.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2308 2024-05-17 08:24:05.000000 loggram-1.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 08:59:56.547855 loggram-1.0.1/loggram/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       28 2024-05-16 21:28:17.000000 loggram-1.0.1/loggram/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1301 2024-05-17 08:27:23.000000 loggram-1.0.1/loggram/loggram.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-17 08:59:56.547855 loggram-1.0.1/loggram.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2767 2024-05-17 08:59:55.000000 loggram-1.0.1/loggram.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      219 2024-05-17 08:59:56.000000 loggram-1.0.1/loggram.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-17 08:59:55.000000 loggram-1.0.1/loggram.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2024-05-17 08:59:55.000000 loggram-1.0.1/loggram.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-05-17 08:59:55.000000 loggram-1.0.1/loggram.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-17 08:59:56.551856 loggram-1.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      685 2024-05-17 08:59:49.000000 loggram-1.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 10:08:52.270062 loggram-1.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-02-22 08:02:12.000000 loggram-1.0.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2767 2024-05-25 10:08:52.270062 loggram-1.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2308 2024-05-25 10:03:12.000000 loggram-1.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 10:08:52.270062 loggram-1.0.2/loggram/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       28 2024-05-16 21:28:17.000000 loggram-1.0.2/loggram/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1301 2024-05-17 08:27:23.000000 loggram-1.0.2/loggram/loggram.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-25 10:08:52.270062 loggram-1.0.2/loggram.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2767 2024-05-25 10:08:52.000000 loggram-1.0.2/loggram.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      219 2024-05-25 10:08:52.000000 loggram-1.0.2/loggram.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-25 10:08:52.000000 loggram-1.0.2/loggram.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2024-05-25 10:08:52.000000 loggram-1.0.2/loggram.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-05-25 10:08:52.000000 loggram-1.0.2/loggram.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-25 10:08:52.270062 loggram-1.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      685 2024-05-25 10:07:15.000000 loggram-1.0.2/setup.py
```

### Comparing `loggram-1.0.1/LICENSE` & `loggram-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loggram-1.0.1/PKG-INFO` & `loggram-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggram
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for sending logs to Telegram channels
 Home-page: https://github.com/Ilia-Abolhasani/loggram
 Author: Ilia Abolhasani
 Author-email: abolhasani.eliya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,22 +34,22 @@
    - Follow [this guide](https://core.telegram.org/bots#6-botfather) to create a new bot and obtain your bot token.
    - Add the bot to your desired channel or group and promote it as an admin.
 
 2. **Initialize LogGram:**
    Here's an example of how to use LogGram in your project:
 
     ```python    
-    from loggram import Telelog
+    from loggram import Loggram
 
     # Replace with your actual bot token and chat ID
     token = "YOUR_TELEGRAM_BOT_TOKEN"
     chat_id = "YOUR_TELEGRAM_CHAT_ID"
 
-    # Create an instance of Telelog
-    logger = Telelog(token, chat_id, verbose=True)
+    # Create an instance of Loggram
+    logger = Loggram(token, chat_id, verbose=True)
 
     # example
     try:
         1 / 0  # Code that raises an error
     except Exception as e:
         logger.send_traceback(str(e))
     ```
```

### Comparing `loggram-1.0.1/README.md` & `loggram-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,22 +20,22 @@
    - Follow [this guide](https://core.telegram.org/bots#6-botfather) to create a new bot and obtain your bot token.
    - Add the bot to your desired channel or group and promote it as an admin.
 
 2. **Initialize LogGram:**
    Here's an example of how to use LogGram in your project:
 
     ```python    
-    from loggram import Telelog
+    from loggram import Loggram
 
     # Replace with your actual bot token and chat ID
     token = "YOUR_TELEGRAM_BOT_TOKEN"
     chat_id = "YOUR_TELEGRAM_CHAT_ID"
 
-    # Create an instance of Telelog
-    logger = Telelog(token, chat_id, verbose=True)
+    # Create an instance of Loggram
+    logger = Loggram(token, chat_id, verbose=True)
 
     # example
     try:
         1 / 0  # Code that raises an error
     except Exception as e:
         logger.send_traceback(str(e))
     ```
```

### Comparing `loggram-1.0.1/loggram/loggram.py` & `loggram-1.0.2/loggram/loggram.py`

 * *Files identical despite different names*

### Comparing `loggram-1.0.1/loggram.egg-info/PKG-INFO` & `loggram-1.0.2/loggram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggram
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for sending logs to Telegram channels
 Home-page: https://github.com/Ilia-Abolhasani/loggram
 Author: Ilia Abolhasani
 Author-email: abolhasani.eliya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,22 +34,22 @@
    - Follow [this guide](https://core.telegram.org/bots#6-botfather) to create a new bot and obtain your bot token.
    - Add the bot to your desired channel or group and promote it as an admin.
 
 2. **Initialize LogGram:**
    Here's an example of how to use LogGram in your project:
 
     ```python    
-    from loggram import Telelog
+    from loggram import Loggram
 
     # Replace with your actual bot token and chat ID
     token = "YOUR_TELEGRAM_BOT_TOKEN"
     chat_id = "YOUR_TELEGRAM_CHAT_ID"
 
-    # Create an instance of Telelog
-    logger = Telelog(token, chat_id, verbose=True)
+    # Create an instance of Loggram
+    logger = Loggram(token, chat_id, verbose=True)
 
     # example
     try:
         1 / 0  # Code that raises an error
     except Exception as e:
         logger.send_traceback(str(e))
     ```
```

### Comparing `loggram-1.0.1/setup.py` & `loggram-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="loggram",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     install_requires=[
         'python-telegram-bot'        
     ],
     author="Ilia Abolhasani",
     author_email="abolhasani.eliya@gmail.com",
     description="A package for sending logs to Telegram channels",
```

