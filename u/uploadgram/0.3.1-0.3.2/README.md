# Comparing `tmp/uploadgram-0.3.1.tar.gz` & `tmp/uploadgram-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadgram-0.3.1.tar", max compression
+gzip compressed data, was "uploadgram-0.3.2.tar", max compression
```

## Comparing `uploadgram-0.3.1.tar` & `uploadgram-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    34522 2024-04-15 13:05:00.860704 uploadgram-0.3.1/LICENSE
--rw-r--r--   0        0        0      412 2024-04-15 13:05:00.860704 uploadgram-0.3.1/README.md
--rw-r--r--   0        0        0     1757 2024-04-15 13:05:00.860704 uploadgram-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      878 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/__init__.py
--rw-r--r--   0        0        0     1920 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/config.py
--rw-r--r--   0        0        0     1167 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/get_config.py
--rw-r--r--   0        0        0     1208 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/humanbytes.py
--rw-r--r--   0        0        0     2772 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/progress.py
--rw-r--r--   0        0        0     1390 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/run_shell_command.py
--rw-r--r--   0        0        0     4292 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/shell.py
--rw-r--r--   0        0        0     1586 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/take_screen_shot.py
--rw-r--r--   0        0        0     1239 2024-04-15 13:05:00.864704 uploadgram-0.3.1/uploadgram/time_formatter.py
--rw-r--r--   0        0        0     7920 2024-04-15 13:05:00.864704 uploadgram-0.3.1/uploadgram/upload.py
--rw-r--r--   0        0        0     2083 2024-04-15 13:05:00.864704 uploadgram-0.3.1/uploadgram/uploadgram.py
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 uploadgram-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-05-25 02:11:25.512552 uploadgram-0.3.2/LICENSE
+-rw-r--r--   0        0        0      412 2024-05-25 02:11:25.512552 uploadgram-0.3.2/README.md
+-rw-r--r--   0        0        0     1761 2024-05-25 02:11:25.512552 uploadgram-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      878 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/__init__.py
+-rw-r--r--   0        0        0     1920 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/config.py
+-rw-r--r--   0        0        0     1167 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/get_config.py
+-rw-r--r--   0        0        0     1208 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/humanbytes.py
+-rw-r--r--   0        0        0     2772 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/progress.py
+-rw-r--r--   0        0        0     1390 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/run_shell_command.py
+-rw-r--r--   0        0        0     4292 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/shell.py
+-rw-r--r--   0        0        0     1586 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/take_screen_shot.py
+-rw-r--r--   0        0        0     1239 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/time_formatter.py
+-rw-r--r--   0        0        0     7920 2024-05-25 02:11:25.512552 uploadgram-0.3.2/uploadgram/upload.py
+-rw-r--r--   0        0        0     2086 2024-05-25 02:11:25.516552 uploadgram-0.3.2/uploadgram/uploadgram.py
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 uploadgram-0.3.2/PKG-INFO
```

### Comparing `uploadgram-0.3.1/LICENSE` & `uploadgram-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/pyproject.toml` & `uploadgram-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uploadgram"
-version = "0.3.1"
+version = "0.3.2"
 description ="Upload files to Telegram upto 4 GiB, from the Terminal"
 authors = ["Shrimadhav U K <uploADGRam@shrimadhavUK.me>"]
 homepage = "https://github.com/SpEcHiDe/UploadGram"
 repository = "https://github.com/SpEcHiDe/UploadGram"
 keywords = ["telegram-upload", "telegram", "upload", "video", "audio"]
 license = "AGPLv3"
 readme = "README.md"
@@ -23,16 +23,16 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.7,<4"
 python-dotenv = "0.10"
-pyrotgfork = "2.1.17"
-TgCrypto = "1.2.5"
+pyrotgfork = "2.1.32.1"
+PyTgCrypto = "1.2.7"
 hachoir = "3.1.1"
 tqdm = "4.62.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 isort = "^5.7.0"
 black = "^20.8b1"
```

### Comparing `uploadgram-0.3.1/uploadgram/__init__.py` & `uploadgram-0.3.2/uploadgram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """Top-level package for Uploadgram."""
 
 __author__ = """SpEcHIDe"""
 __email__ = "uploADGRam@shrimadhavUK.me"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
```

### Comparing `uploadgram-0.3.1/uploadgram/config.py` & `uploadgram-0.3.2/uploadgram/config.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/get_config.py` & `uploadgram-0.3.2/uploadgram/get_config.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/humanbytes.py` & `uploadgram-0.3.2/uploadgram/humanbytes.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/progress.py` & `uploadgram-0.3.2/uploadgram/progress.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/run_shell_command.py` & `uploadgram-0.3.2/uploadgram/run_shell_command.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/shell.py` & `uploadgram-0.3.2/uploadgram/shell.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/take_screen_shot.py` & `uploadgram-0.3.2/uploadgram/take_screen_shot.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/time_formatter.py` & `uploadgram-0.3.2/uploadgram/time_formatter.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/upload.py` & `uploadgram-0.3.2/uploadgram/upload.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.3.1/uploadgram/uploadgram.py` & `uploadgram-0.3.2/uploadgram/uploadgram.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         super().__init__(
             name="UploadGram",
             api_id=int(get_config("UG_TG_APP_ID")),
             api_hash=get_config("UG_TG_API_HASH"),
             parse_mode=ParseMode.HTML,
             sleep_threshold=int(get_config("UG_TG_ST", 10)),
             workers=int(get_config("UG_TG_WS", 10)),
-            max_concurrent_transmissions=int(get_config("UG_TG_MCTS", 4))
+            max_concurrent_transmissions=int(get_config("UG_TG_MCTS", 4)),
             no_updates=True,
             device_model="Samsung SM-G998B",
-            app_version="8.4.1 (2522)",
+            app_version="10.11.2 (4665)",
             system_version="SDK 31",
             lang_pack="",
             lang_code="en",
             system_lang_code="en",
             max_message_cache_size=int(get_config("UG_TG_MMC", 0)),
             max_business_user_connection_cache_size=int(get_config("UG_TG_MBUC", 0)),
             client_platform=ClientPlatform.ANDROID
```

### Comparing `uploadgram-0.3.1/PKG-INFO` & `uploadgram-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploadgram
-Version: 0.3.1
+Version: 0.3.2
 Summary: Upload files to Telegram upto 4 GiB, from the Terminal
 Home-page: https://github.com/SpEcHiDe/UploadGram
 License: AGPLv3
 Keywords: telegram-upload,telegram,upload,video,audio
 Author: Shrimadhav U K
 Author-email: uploADGRam@shrimadhavUK.me
 Requires-Python: >=3.7.7,<4
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: TgCrypto (==1.2.5)
+Requires-Dist: PyTgCrypto (==1.2.7)
 Requires-Dist: hachoir (==3.1.1)
-Requires-Dist: pyrotgfork (==2.1.17)
+Requires-Dist: pyrotgfork (==2.1.32.1)
 Requires-Dist: python-dotenv (==0.10)
 Requires-Dist: tqdm (==4.62.3)
 Project-URL: Repository, https://github.com/SpEcHiDe/UploadGram
 Description-Content-Type: text/markdown
 
 ## uploadgram
```

