# Comparing `tmp/rumchat_actor-1.1.1.tar.gz` & `tmp/rumchat_actor-1.1.2.tar.gz`

## Comparing `rumchat_actor-1.1.1.tar` & `rumchat_actor-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    20770 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/src/rumchat_actor/__init__.py
--rw-r--r--   0        0        0    20588 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/src/rumchat_actor/common_commands.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 rumchat_actor-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    20787 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/src/rumchat_actor/__init__.py
+-rw-r--r--   0        0        0    20645 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/src/rumchat_actor/common_commands.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 rumchat_actor-1.1.2/PKG-INFO
```

### Comparing `rumchat_actor-1.1.1/.github/workflows/python-publish.yml` & `rumchat_actor-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.1.1/src/rumchat_actor/__init__.py` & `rumchat_actor-1.1.2/src/rumchat_actor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             self.stream_id = self.api_stream.stream_id
             self.stream_id_b10 = utils.stream_id_36_to_10(self.stream_id)
 
         #Get SSE chat and empty the mailbox
         self.ssechat = SSEChat(stream_id = self.stream_id)
         self.ssechat.clear_mailbox()
 
-        #Set browser profile directory of we have one
+        #Set browser profile directory if we have one
         options = webdriver.FirefoxOptions()
         if profile_dir:
             options.add_argument("-profile")
             options.add_argument(profile_dir)
 
         #Get browser
         self.browser = webdriver.Firefox(options = options)
@@ -303,15 +303,15 @@
 
         return self.__is_channel_stream
 
     @property
     def streamer_main_page_url(self):
         """The URL of the main page of the streamer"""
         if self.is_channel_stream:
-            return CHANNEL_URL.format(channel_name = self.streamer_channel)
+            return CHANNEL_URL.format(channel_name = self.streamer_channel.replace(" ", ""))
 
         return USER_URL.format(username = self.streamer_username)
 
     def get_sign_in_button(self):
         """Look for the sign in button"""
         try:
             return self.browser.find_element(By.CLASS_NAME, "chat--sign-in")
```

### Comparing `rumchat_actor-1.1.1/src/rumchat_actor/common_commands.py` & `rumchat_actor-1.1.2/src/rumchat_actor/common_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,29 +26,31 @@
 CLIP_BITRATE = "4.5M" #The bitrate to use when saving clips. Deprecating
 STREAM_QUALITIES = {"360p" : "1.2M", "720p" : "2.8M", "1080p" : "4.5M"} #Valid resolutions of a livestream and the bitrates they use / should be saved with
 NUM_TS_DOWNLOAD_TIME_CHECKS = 5 #How many times to test a TS chunk download to get its average download time
 TS_DOWNLOAD_SPEEDFACTOR_REQUIREMENT = 2 #TS chunks must be able to download this many times faster than their duration to be usable in a cache. Cannot be less than 1
 
 class TTSCommand(ChatCommand):
     """Text-to-speech command"""
-    def __init__(self, *args, name = "tts", voices = {}, **kwargs):
+    def __init__(self, *args, name = "tts", voices = {"default" : talkey.Talkey().say}, **kwargs):
         """Pass the same args and kwargs as ChatCommand, plus:
     voices: Dict of voice : say(text) callable"""
         super().__init__(*args, name = name, **kwargs)
         self.voices = voices
-        self.default_voice = talkey.Talkey()
+
+        #Get the default voice
+        self.default_voice = voices["default"]
 
     def speak(self, text, voice = None):
         """Speak text with voice"""
         if not voice:
-            self.default_voice.say(text)
+            self.default_voice(text)
 
         #Voice was not actually in our list of voices
         elif voice not in self.voices:
-            self.default_voice.say(voice + " " + text)
+            self.default_voice(voice + " " + text)
 
         else:
             self.voices[voice](text)
 
     def run(self, message):
         """Run the TTS"""
         segs = message.text.split()
```

### Comparing `rumchat_actor-1.1.1/LICENSE.txt` & `rumchat_actor-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.1.1/README.md` & `rumchat_actor-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rumchat_actor-1.1.1/pyproject.toml` & `rumchat_actor-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rumchat_actor"
-version = "1.1.1"
+version = "1.1.2"
 keywords = ["rumble", "chat", "livestream", "bot"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "Automatically interact with your Rumble livestream chats."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `rumchat_actor-1.1.1/PKG-INFO` & `rumchat_actor-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rumchat_actor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automatically interact with your Rumble livestream chats.
 Project-URL: Homepage, https://github.com/thelabcat/rum-chat-actor
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: bot,chat,livestream,rumble
 Classifier: Development Status :: 4 - Beta
```

